# Project Unit 1: A notepad


# Criterion A: Planning

My client is suffering from leak of security information in his company. He needs stronger cybersecurity system for managing information.  


## Problem definition (Add more details to this context)

My client is the owner of luxury chain hotels and manages his clients’ information using each hotels’ websites. Over the past five years, there have been five phishing attacks and password attacks that violated client privacy. My client’s main concern is that employees use websites that can access all the passwords using a password that is open to everyone within the company. To protect the company’s credibility, my client wants to ensure that the system that allows access to client information is secure. (See the evidence of Consulation in the Appendix)


## Proposed Solution

I am proposing to create a notepad which contains a secret function that is only revealed when a hidden code is entered. Once the correct secret code is typed into the notepad, it transfroms into the password manager that my client requires. This is an adequate solution for my client because it solves the problem or keeping password information both protected and hidden.

## Rationale

I proposed to use terminal and python in this procedure. Python is user-friendly programming language and is globally used. In addition, Python allows developer to use their own software to develop the project. 
According to _12 reasons why you should learn Python_, "Python has several powerful applications integrated with other programming languages". Terminal is the platform that could be used directly from computers which allows wider users to use the application. According to _Why are the benefits of using Terminal?_ from Lenovo.com, "it provides a powerful and efficient way to interact with computers". 

## Success Criteria

1. The notepad should accept user input to perform basic operations (adding memo, deleting memo and viewing memo). 
   **[Issue Tackled]**: **: "employees use websites that can access all the passwords using a password that is open to everyone within the company."
   
2. The notepad should give appropriate feedback and treat with errors appropriately to prevent crashing.

3. If the user enters the secret code (username"hotel"), the program will change modes and act as a password manager. 
4. In password manager mode, the user should be able to perform basic operations (Creating password, viewing password, updating password, deleting password, and end the secret mode.) and treat with potential errors.
   - For creating password, user should be able to choose to get auto-generated strong password
   - Password created should be encrypted and be stored in the .csv file
   - Password created should be decrypted when the user ask for viewing mode

5. In password manager mode, the user should be able to:
   - Add a password (for a hotel).
   - View the stored passwords (only if they enter another secret code for this).

6. To prevent unwanted access, if the user enters a wrong secret code for viewing password over three times, the program will end. Also, make it invisible when user inputs the secret password to view the passowrd. 

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





### Test plan
| Test Number | Type of Test | Area Tested      | Process of Testing                                                                                                                                                                                                                                                                                                                                                    | Test Outcome                                                                                                                                                                                                                                     | Time Estimated | Target Completion Date | Criterion |
|-------------|--------------|------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|------------------------|-----------|
| 1           | Unit Testing | Greeting         | 1. Enter username for notepad                                                                                                                                                                                                                                                                                                                                         | Display the greeting statement and options that usrs can choose from.                                                                                                                                                                            | 10 min         | Sep 15                 | B         |
| 2           | Unit Testing | Notepad          | 1. Enter from 1 to 3 to decide which action to take (add, delete, and view) 2. If a valid number is entered, do action corresponds to  the number for user. If not, enter a number again. Display that the action is completed successfully. 3. Option of 'terminate' shows up as 4th option. If 4 entered, display greeting. If not,  loop the function as notepad.  | Confim that user can add, delete, view note, and terminate. If action completed,  it tells user that the action is successfully completed.  If the program get invalid input, display that the input is not valid and loop the notepad function. | 10 min         | Sep 16                 | B         |
| 3           | Unit Testing | Login            | 1. Enter secret password (name'hotel') 2. Enter username                                                                                                                                                                                                                                                                                                              | Change the mode to secret mode.                                                                                                                                                                                                                  | 10 min         | Sep 18                 |B          |
| 4           | Unit Testing | Password Manager | 1. Enter from 1 to 5 to decide which action to take (View, add, update, delete, and terminate) 2. If a valid number is entered, do action corresponds to the number for user. If not, enter a number again.  3. Loop the function as password manager.                                                                                                                | Confirm that user can use password manager as it is expected.                                                                                                                                                                                    | 10 min         | Sep 25                 |B          |


## Record of Tasks
| Task Number | Planned Action                                                             | Planned Outcome                                                                                                                                                                                                                                                                                                                                                     | Time Estimated | Target Completion Date | Criterion |
|-------------|----------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|------------------------|-----------|
| 1           | Meeting with the client                                                    | Obtained a problem definition, understand what the situation is.                                                                                                                                                                                                                                                                                                    | 10 min         | Sep 7                  | A         |
| 2           | Define a problem                                                           | See the situation of my client and have a clear understanding of a problem that the client has.                                                                                                                                                                                                                                                                     | 10 min         | Sep 7                  | A         |
| 3           | Create a system diagram                                                    | Make a system diagram to come up with the best choice for  which programming language to use, and ensure that user conveniently use the program.                                                                                                                                                                                                                    | 15 min         | Sep 20                 | B         |
| 4           | Proposing an idea  (Meet with the client)                                  | Propose an idea to the client how to solve the problem, and define a solid idea for developping the project. Get approval from                                                                                                                                                                                                                                      | 20 min         | Sep 11                 | A         |
| 5           | Success Criteria                                                           | Define the goals of the overall task to clarify the requirement  that I have to fulfill while developping the project to direct myself in a right way to satisfy my client.                                                                                                                                                                                         | 15 min         | Sep 11                 | A         |
| 6           | Create basic notepad  function                                             | Develop a basic function notepad: Adding, deleting, viewing, and  terminate) and ensure that it is user-friendly and treat with potential errors.                                                                                                                                                                                                                   | 60 min         | Sep 14                 | B         |
| 7           | Create a code for change mode  to secret mode                              | Write a code that allows user to go to the secret mode when they enter the secret password                                                                                                                                                                                                                                                                          | 10 min         | Sep 15                 | B         |
| 8           | Create main menu of  secret mode functions                                 | Develop functions to make secret mode work appropriately when  user changed the mode.                                                                                                                                                                                                                                                                               | 20 min         | Sep 17                 | B         |
| 9           | Create functions of basic secret mode                                      | Taking input from users, the project should work appropriately and give feedback. You should be able to add password which allows them to create their original password or let the program create one for them, update the password that already exists,  delete the password that exists, view the password stored (entering password is needed),  and terminate. | 150 min        | Sep 25                 | B         |
| 10          | Create functions of encryption  and decryption                             | Developing functions that enables the password to be stored securely, but also can be  shown.                                                                                                                                                                                                                                                                       | 40 min         | Sep 20                 | B         |
| 11          | Call the functions in the main file  to complete the project and test it.  | Using the functions developed, the project should be able to handle any situations and satisfy success criteria. Test it by running the code and revise whatever it not user-friendly or  not working.                                                                                                                                                              | 60 min         | Sep 21                 | A, B      |
| 12          | Check with Client                                                          | Check with my client if the project satisfies him. Explain how it satisfiees the success criteria, and ensure again if it works under his environment.                                                                                                                                                                                                              | 20 min         | Sep 25                 | A, B      |
| 13          | Revise code and finalize the project                                       | Based on the feedback that my client gave, revise code to make it better and finalize the project.                                                                                                                                                                                                                                                                  | 40 min         | Sep 26                 | A, B      |
| 14          | Submit the project to my client                                            | Meet with the client and submit the work.                                                                                                                                                                                                                                                                                                                           | 5 min          | Sep 26                 | A         |



# Criterion C

## Here is the video: 
