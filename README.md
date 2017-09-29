# Registration Resume Pro

## [Experience this app live on Heroku](https://registration-resume-pro.herokuapp.com/)
username: user, password: pass   

_Please note that Heroku can sometimes have an exceedingly slow response time at first, so if the welcome page doesn't load on the first try, it should on the second try.  After it 'wakes up' the pages should respond well._
***

Feel free to do whatever you want: add students or course, wipe all the tables, load dummy data, it's up to you!   
Note: the dummy data loader will only load if there are 20 or less persons in the person table, ie it will only load once.  If you wipe all the tables, it will allow you to load more dummy data.

This web app simulates an administrative student course and resume tool.  An admin user logs in and add students and courses.  A postgresql database is used to persist the data on Heroku.  There are five relational tables, all implemented using the Java persistence framework.  Students and Courses share a many to many relationship.. a student can be enrolled in many courses, and a course can have many registered students.

The admin can selectively remove students from a course, one or many at a time using HTML check boxes.  The admin may also simultaneously remove one or many courses from a students registration list.  The app also allows the user to create a Resume for each student, where numerous educational achievements, work experiences, and skills can all be entered.  A final resume is generated after the user enters at least one skill and one educational achievement.  Most database entities can be edited and removed at will, while all relationships are retained.

_One fun thing about this app_ is that there is button on the admin navbar to programmatically load 20 students with semi-random data... database assocations are made during this process.  An admin can also click a button to wipe all the data from every table.  This allows you to more easily test the functionality of the app, because you don't have to sit there and create a bunch of students, courses, add skills, etc.

It is responsive and mobile ready!
