# SQL-Lab

## Objective
I was tasked with using the SQL injection technique on a browser made for testing only. I had to utilize the sign in page to find any weaknesses and expose them. The site I was testing on is below in the image.
![image](https://github.com/user-attachments/assets/ef942d25-2047-4227-be21-8343895b8537)

### Skills Learned
-Knowledge on completing SQL injections
-Ability to spot vunerabilities on sites for injection
-Ways to prevent attacks like this in the code

### Tools Used
-A website made specifically for testing


## Steps
1.First I just attempted using admin as the user and random passwords to see if it would drop any clues on what to try next. Came up with nothing and tried puting an ' in the admin username to make it admin' and that's where I spot the weakness as it shows that was a syntax error when I tried signing in.
![Screenshot 2025-04-21 175020](https://github.com/user-attachments/assets/5b3dd4e6-2a58-4935-98a3-036e40c4b8c3)
<br>
2. Second I knew I was looking a query close to if not exactly like  SELECT * FROM user WHERE username = 'admin' AND password='password123', so I had to see if I could do anything to make the statement go through for the admin user regardless if I get the password right. Did this by making an OR statement in the username field where I would turn the first part of statement into WHERE username ='admin' OR '1'='1'. Still got an error, but I knew I was close.
![Screenshot 2025-04-21 175320](https://github.com/user-attachments/assets/35e92094-e315-4739-bd20-74ac79076b40)
![Screenshot 2025-04-21 175349](https://github.com/user-attachments/assets/b131ce81-87b3-442d-9fa5-735452124e3a)
![Screenshot 2025-04-21 175407](https://github.com/user-attachments/assets/b5ed4edb-9a3c-4ad4-99c8-a35f9e75cfd2)
![Screenshot 2025-04-21 175446](https://github.com/user-attachments/assets/83021e84-fc2a-4a77-8f7f-ef1d211be1ac)
