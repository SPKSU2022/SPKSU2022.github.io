---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

## Abstract
Getting anyone motivated to complete chores can be a chore itself! To solve this issue, our team is using Dart and Flutter to build a desktop application that pits roommates, family members, and siblings against one another to complete chores for points. The purpose of this program is to simulate competition between users in order to motivate users to complete tasks amongst the living space.
To complete this task, our program will provide a place where users can create a family, create an account, join a family, create chores, complete chores, check chore history, view the family scoreboard, and view how many chores they have completed. Users will be able to change chore points based on difficulty, estimated time of completion, and priority. There will also be a way for users to check chore history in order to know which chores were completed by each person. The family will have a main homepage which will show the top three scores within the family, the chores with the highest priority, and the family ID in which users can share with one another to allow others to join the family.

### About
[About](about.markdown)

### Timeline
[Timeline](timeline.markdown)

### Scope
[Scope](scope.markdown)

### Backend
[Backend](backend.markdown)

### Frontend
[Frontend/UI](frontendUI.markdown)

### Source Control
[Source Control](sourceControl.markdown)

### Conclusion
[Conclusion](conclusion.markdown)



### Process and Methods Used
Our desktop application will use features within flutter such as integration with the recently released Amplify API integration with the desktop version of flutter. This integration allows us to take advantage of Amazon Web Services, specifically Amazon Cognito which allows secure account creation, two factor authentication, and account recovery. This is useful as our backend consists of Amazon RDS for our relational Database. By using RDS and Amplify Cognito, it will allow us to assign a family to users such that our database queries will only grab information related to the user’s family. Amplify also allows us to pull user information such as their names for various entries into our Database.
As for our UI, we will be using Flutter’s Material UI. It is Flutter’s default UI options that allow for extreme customizability and flexibility when building the application. The login screen will use Amplify’s API for the built in logic and UI. Once the user has logged in, the rest of the UI will be built by scratch and laid out to suit the functionality of the program. There will be 3 main screens, the homepage, scoreboard, and chore screen. All of which will help serve the function of the application.
Our queries to the database currently will use direct querying. In phase 2 of the program, we will implement Cognito’s authentication feature by switching the queries to AWS lambda and accessing them through calls to the AWS API Gateway. This is within phase 2 of the application due to the time constraints of the semester.
For source control, we have been using GitHub and following two main branch structure. There are two main branches, a main(Stable), and a main(development). The development branch stays ahead of the stable branch, but may encounter bugs and errors. Meanwhile the stable branch may be missing features, but each feature has been properly bug tested.


### Results/Findings
Setting up AWS Amplify with Flutter on desktop took lots of configuring and tweaking to work properly, but it will offer more functionality that otherwise would take longer to hand code. As for the RDS Database, our DB currently has 4 tables with the main route table being families. Each user will be attached to a family via the foreign key of family ID. Then each chore can be attached to a family via the foreign key of the family ID. Each piece of information regarding the family, chores, and members can be obtained through queries to the DB. 
Some struggles have been with error checking on user inputs. Certain inputs can cause the logic of the application to not work properly. To solve this we have used Regular Expressions and Flutter input formatters to limit what users are allowed to input into the program. This issue was originally not accounted for, but has taught us a great deal about error checking each step that users are allowed to take.
There are a lot of ideas we would like to implement, but as the project grows. New ideas can intersect with portions of the program that otherwise would’ve been overlooked. We are learning this and have shifted to separate widgets from one another in order to isolated sections of the program. This allows for easier bug testing and implementation.
  
### Conclusion
In conclusion, this project has challenged our abilities to balance planning and action. There are issues that arise only after beginning on the project and others that can be avoided with proper planning. To properly navigate this, we meet twice a week and maintain constant communication on which sections of the program each member is working on. This avoids conflicts in source code, while also providing what features are properly implemented. We have a great deal more to work on this project, but we are excited and eager to learn more about AWS, Flutter, and Dart.

