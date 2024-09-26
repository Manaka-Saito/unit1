# Project Unit 1: A simple calculator


# Citerion A: Planning

My client is suffering from leak of security information in his company. He needs stronger cybersecurity system for managing information.  


## Problem definition (Add more details to this context)

My client is the owner of luxury chain hotels and manages his clients’ information using each hotels’ websites. Over the past five years, there have been five phishing attacks and password attacks that violated client privacy. My client’s main concern is that employees use websites that can access all the passwords using a password that is open to everyone within the company. To protect the company’s credibility, my client wants to ensure that the system that allows access to client information is secure. (See the evidence of Consulation in the Appendix)

- client can enter the spesific room number that turns into the password
- wants to keep the password hidden
- wants to use different password per employees



## Proposed Solution

I am proposing to create a notepad which contains a secret function that is only revealed when a hidden code is entered. Once the correct secret code is typed into the notepad, it transfroms into the password manager that my client requires. This is an adequate solution for my client because it solves the problem or keeping password information both protected and hidden.


## Success Criteria

1. The notepad should accept user input to perform basic operations (adding memo, deleting memo and viewing memo).
   **[Issue Tackled]**: **: "employees use websites that can access all the passwords using a password that is open to everyone within the company."
   
2. The notepad should give appropriate feedback and treat with errors appropriately to prevent crashing.

3. If the user enters the secret code (username"hotel"), the program will change modes and act as a password manager. 
4. In password manager mode, the user should be able to perform basic operations (Creating password, viewing password, updating password, deleting password, and end the secret mode.) and treat with potential errors.
   
5. In password manager mode, the user should be able to:
   - Add a password (for a hotel).
   - View the stored passwords (only if they enter another secret code for this).

6. To prevent unwanted access, if the user enters a wrong secret code for viewing password over three times, the program will end. 

7. Save passwords permanently and securely using encryption and decryption.

8. Use the terminal to interact with the user.





# Criterion B: Design
### System Diagram
<img width="867" alt="Screenshot 2024-09-27 at 1 40 27" src="https://github.com/user-attachments/assets/43f5a9be-9f7e-4da3-8603-300bac54b17b">

### Flow diagrams for algorithms


<img width="518" alt="Screenshot 2024-09-27 at 6 46 43" src="https://github.com/user-attachments/assets/6e93b57b-ca26-4da5-bfd1-ef0487cce5db">
**Fig. 1** This is the flow diagram for generating a random password for the user using their preferances of how the password looks like. Parameters are lengths of passwords that the user choose, and symbols which indicates if the user wants to include symbols in it. Generated random characters for number of times of lengths of a password, and the output is returned.

<img width="645" alt="Screenshot 2024-09-27 at 7 46 23" src="https://github.com/user-attachments/assets/21e7e7bb-0f47-4384-8a98-7d5a56c26dd9">
<img width="719" alt="Screenshot 2024-09-27 at 7 48 52" src="https://github.com/user-attachments/assets/f1dd8c04-5b4e-4fc3-abd9-2340dce28a05">
<img width="737" alt="Screenshot 2024-09-27 at 7 49 11" src="https://github.com/user-attachments/assets/e7af4eae-c78b-46a0-a1b8-941135889f03">

**Fig. 2** This is the flow diagram to decide if the user wants to regenerate the password that the program generated with the style that the user chose before. Once the user decided to regenerate the password again for over three times, the user will be asked if they want to change the option she chose before or not in order to make it user friendly. 

<img width="608" alt="Screenshot 2024-09-27 at 6 33 40" src="https://github.com/user-attachments/assets/19f0369b-fa36-4631-b10b-db0858cf6038">
**Fig. 3** This is the flow diagram for the algorithm used to decrypt password, which is a parameter of a function. Shifting is used in the algorithms and all alphabet in both uppercase and lowercase and symbols are being shifted once this function is called via loop and if-statement. 


diagrams

### Data storage
diagrams
### Sketches of the application (wireframe diagrams)
diagrams


### Test plan


## Record of Tasks

| Task Number | Planned Action               | Planned Outcome                                                 | Time Estimated | Target Completion Date | Criterion |
|-------------|------------------------------|-----------------------------------------------------------------|----------------|------------------------|-----------|
| 1           | 1st. Meeting with the client | Obtained a problem definition, understand what the situation is | 10 min         | Sep 7                  | A         |
| 2           | 2nd. Proposing the idea      | Propose an idea for what to create to solve the problem         | 10 min         | Sep 7                  | A         |
| 3           | 3rd. Planning processes      |                                                                 |                |                        |           |
|             |                              |                                                                 |                |                        |           |
|             |                              |                                                                 |                |                        |           |
|             |                              |                                                                 |                |                        |           |
|             |                              |                                                                 |                |                        |           |
