# twist
Fellow collaborators:  Shealan Clark, Jon Martin, Eric Webb, Alex Windhorst

The main learning objectives for this project were to apply what we learned about server-side programming, the Node.js environment and the Express framework from our prior two modules in CMST 335 Programming II to a real-world assignment.  This assignment was also an exercise in collaboration.  The predevelopment stage (all work from this can be found in the `_PREBUILD` directory) spanned about two-and-a-half weeks.  The actual development stage, from beginning work on the website within Express to deployment on Heroku, spanned about one month.

My contributions to the project were as follows:
- Transcribed/created admin and registrant use cases.
- Designed entity-relationship diagrams for the above use cases.
- Designed an updated blueprint of our desired database.
- Created template database on mongoDB Atlas.
- Created one model and edited schemas for data types.
- Began work on a script to populate our database with placeholder/dummy data (not implemented).
- Various formatting/OCD fixes wherever found.
- Preparation and deployment of the app on Heroku.  Can be found at https://twist-final-2019.herokuapp.com/

Difficulties that I ran into had primarily to do with learning more features of mongoDB Atlas, mostly the ability to manually edit data within the databases in the cluster, and syntax errors in the unused population script.  These were easily learned in the case of the former by experimentation, and fixed in the case of the latter by noting where the command-line interface pinpointed the errors.  A problem in the deployment stage was that nothing could be appended to a production database when configuration variables were set for this to happen.  This was rectified by removing the MONGODB_URI configuration variable from the settings on the application, causing the app to function normally.

Known incomplete features include:
- There is no error message for inputting incorrect credentials when attempting to log in.
- Registration and Admin/add-attendee cannot post new people to the database.
- Admin/edit-attendee likewise cannot post changes to the database.
- Admin/edit-speaker is partially functional--topic and topic description cannot be edited.
- Admin/edit-session returns a 'Not Found' error

If my cohort and I were to redo this project, I think establishing a means of communication between us sooner than we actually did, preferrably at the start of the pre-development portion of the assignment, would have allowed us to more easily work on this project outside of class.  Subsequently, we would finish pre-development quicker, thereby giving us more time to work in the development stage.  This extra time would then allow us to ultimately deploy and submit a more finished website application.
