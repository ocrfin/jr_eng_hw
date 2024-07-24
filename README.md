# Backend Engineering Homework  
  
Thank you for spending time with us in the previous interviews.  The next step in the process is a homework assignment designed to help us understand how you handle actual coding problems. We would like you to do this assignment, taking a maximum of 4 hours so we don’t eat up too much of your time.  Make sure to understand your solution as the next step in the process is deep diving on it.   
  
### Part 1: Get it working  
Since this is a vanilla Django Rest Framework application we will not be providing instructions on how to get it up and running. Additionally, there are issues with the application which you will need to find and fix before you can move onto part two.  The application needs to be functional when turned in.  
  
### Part 2: Managing users  
Currently, our application doesn't allow users to be added or deleted through the API. 
* Only staff users should be able to do this
* If someone deletes a user it should "soft delete", so instead of removing the record from the database it should simply be flagged as deleted.
* If a user is deleted it should be filtered from all views of any non-staff user
* If the user is staff the app should optionally display deleted users when they specificy a flag to the api endpoint
* This system needs to have tests.

### Part 3: Audit Log  
We are interested in seeing what was done in the system.  To this end we would like you to add a new feature which will store all API actions and allow us to view them through another API endpoint.

Requirements for the model:
* The action should be stored in the database
* It should have the user attached
* The model should record the model name, id, action taken (update, create, destroy), and timestamp
* Should only be visible to Staff.  No one should be able to add or edit through the API
* Tests should be included

### Bonus: Still have time?
Our test file had no tests before you added yours.  If you don't use up all four hours then show us your testing chops on the rest of the application. The goal here is to add testing so that as we add more to the application, we know the functionality didn't break.


## Deliverables
We would like you to create your own repo that has the finished homework assignment.  

## Questions?
We are happy to answer questions.  Just reach out to your recruiter to get in touch.
