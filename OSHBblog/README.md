# BULIDING A COMMUNITY

Our project helps provide a repository of knowledge for everyone. OSBH aims to provide individuals with array of books, articles and tutorials at their fingertips. Our team members are Philip Ukanwoke, David Okolie and myself. David was in charge of the frontend. Philip handled the testing aspect of the web app and I handle the business logic of things. As an engineering problem, we wanted to build a community for individuals with similar interest to come together, hangout and share ideas. 
During the early days of whiteboarding, we all had different project ideas, as well as possible solutions to these problems. After a few back and forth, we finally we decide to come up with three major metrics for choosing a project. 
1.	We must be able to reach a working MVP by the end of the 3weeks given by the ALX Software engineering program.
2.	This project should try as much as possible to include each other’s ideas or proposed functionality, without overcomplicating the entire project.
3.	It must be a project that promotes the sense of community.
and Voila, OSBH was born.

### Project Result
![authUser](https://user-images.githubusercontent.com/26916048/230170897-54db4301-f545-49db-a5f8-efbb0e5e46dd.PNG)

For the Frontend we chose to use [Bootstrap](https://getbootstrap.com/docs/5.0/getting-started/introduction/). We opted for bootstrap because of the speed it provides during rapid full stack development.
For the backend, we used a Django which is a python framework for web development.  Considering we just finished the [Airbnb Clone](https://github.com/rotex5/AirBnB_clone_v4) project using [Flask](https://flask.palletsprojects.com/en/2.2.x/), trying out [Django](https://www.djangoproject.com/start/) was a way for us to test the waters and solidify our understanding of Python. It should also be noted that we chose Django over Flask because it’s a very good tool for rapid development.
#### Feature: 
* Third Party Sign Up/Login authentication for GitHub using allAuth. 
* The website is responsive and compatible with mobile. This means users can access the project from a mobile view.
* Pagination based on number of books listed at a time.

### Technical challenge
We realized that it's important to understand how the test database works and how to properly set up test data. Because we encountered errors with persistence of our test setup data, the database was not being accessible and the data not being persisted as expected
We initially assumed that the database was being written to, but it turned out that the test database was created at runtime and destroyed after the test was completed. This resulted in data not being persisted and not being accessible during runtime.
To solve this error, our team did more research and discovered that the --keepdb flag could be used to keep the test database and make the data accessible even after runtime. With this flag, we were able to view the data in the test database after runtime.

Additionally, our team used a connection to access the content of the test database. This connection was obtained using the django.db.connections object, which provides a dictionary-like interface to all defined database connections. We used this connection to perform queries and retrieve data from the test database during the execution of our tests. 
We also ensured that the data being persisted and the logic being used to create or fetch the data were all in the same scope. This helped to ensure that the test database was being written to and data being retrieved from the correct location.

In conclusion, the error related to persistence of test set up data was resolved by using the --keepdb flag to keep the test database and a connection to access the content of the database at runtime. It was also important to ensure that the data being persisted and the logic being used to create or fetch the data were in the same scope to avoid any issues related to accessing the correct location. These steps helped to ensure that the test set up data was properly persisted and accessible during runtime, resulting in a more efficient testing process.

### What I Learnt.
Django is a very powerful web framework. I may have used Django once or twice before, but damn, this project really got me into the gutters. I even discovered [HTMX](https://htmx.org/).  Htmx allows you to access AJAX, CSS Transitions, WebSockets and Server Sent Events directly in HTML, using attributes, so you can build modern user interfaces with the simplicity and power of hypertext. Very wonderful tool I might say.  As an engineer, this project made me understand the importance of RTFM (Hhehehheehe).  I do agree that going through the official Docs can be stressful, but sometimes you end us stumbling on treasure trovers that can help you right now and in the future. 
SideNote: I might have helped out with some parts of the frontend…But I am definitely a backend… :rofl: :rofl: :rofl:

### Where do we go from here.
We consider this project to a very interesting one with real world applications. Hence, we have chosen to continue to build on this. Adding more functionalities while we make it accessible to the public. We hope to foster a community of like-minded individuals who can come together to relax, have fun and share ideas. 

### About Me
I am a passionate web developer and a fan of the [Mugiwara Pirates](https://onepiece.fandom.com/wiki/Straw_Hat_Pirates) 😜. Just trying to make the world a better place one key stroke at a time. Check me out on [github](https://github.com/rotex5). You can also connect with me on [LinkedIn](http://www.linkedin.com/in/davidson-ogaraku-a9547aa7).
