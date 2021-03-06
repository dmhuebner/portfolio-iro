---
layout: post
title: Open Chat
feature-img: "img/work_assets/open_chat/open_chat_header2.png"
thumbnail-path: "img/work_assets/open_chat/open_chat_thumbnail2.png"
short-description: Open Chat - Instant messaging app


---
**<a href="https://openchat.netlify.com/" target="_blank" style="font-size: 2rem;">Open Chat</a>**

#### **SUMMARY**

Open Chat is a simple instant messaging application built with *Angular.js* and *Firebase*. It uses the Firebase *AngularFire* module to provide a real-time backend with three-way data binding and includes user signup and authentication.

{:.center}
![]({{ site.baseurl }}/img/work_assets/open_chat/open_chat_thumbnail2.png)

#### **TECHNOLOGIES USED**

HTML5, CSS3, JavaScript, jQuery, Angular.js, Firebase, AngularFire, UI Bootstrap, Grunt, Git

#### **EXPLANATION**

The goal of this project was to create a simple instant messaging application with JavaScript, Angular.js, and Firebase that features three way data binding and real-time application updates without refreshing the page. It was created according to user stories provided in the <a href="http://bloc.io" target="_blank">Bloc</a> *Full Stack Developer* curriculum.

This is a simple but effective instant messaging application that can be expanded on and customized to create more robust chat applications. This project was created to practice and demonstrate my, *JavaScript*, *Angular.js*, *HTML*, and *CSS* proficiency as well as to gain more experience implementing a real-time database with *Firebase*. I used the Firebase *AngularFire* module to create three-way data binding between the HTML, JavaScript and Firebase database. This allows the application to show new instant message updates in real time without requiring the page to be refreshed.

Open Chat has a simple, mobile responsive design and utilizes *UI Bootstrap*'s Modal service in combination with *ngCookies* to require users to signup for a new account or login with an existing email/password pair before proceeding to select a chat room.

#### **PAGES**

##### **Login/SignUp Modals:**

Posting instant messages in any room requires a user to be logged in. Users who are not already logged in to Open Chat are initially presented with the Login Modal. The Login Modal allows a user to enter an email and password pair to login or they can click "Sign Up" to open the SignUp modal. A cookie is placed on a user's browser upon logging in to the website to keep track of the user's session.

{:.center}
![]({{ site.baseurl }}/img/work_assets/open_chat/open_chat_login_modal.png)

The Sign Up modal gathers a new user's username, email, and password and uses AngularFire's Authentication API to save them to the Firebase database. I created a user object in the Firebase database to associate the username with the correct Firebase user id. When a user logs in to Open Chat the username that is associated with their user id is populated in the top right and is displayed next to any messages they send. Both the Login and SignUp modal utilize *UI Bootstrap*'s Modal service ($uibModal).

{:.center}
![]({{ site.baseurl }}/img/work_assets/open_chat/open_chat_signup_modal.png)

Once a user is logged in, they can logout by clicking the "Logout" button in the top right. Logging out ends the user session and removes the login cookie from the user's browser.

##### **New Room Modal:**

Once a user logs into the application they will be able to choose a Room from the selection on the left. Additionally, they would be able to create new rooms by clicking the (you guessed it) "New Room" button. The New Room button triggers the New Room modal which also utilizes *UI Bootstrap*'s Modal service ($uibModal).

{:.center}
![]({{ site.baseurl }}/img/work_assets/open_chat/open_chat_new_room_modal.png)

Users can create public rooms that anyone can chat in or private rooms that only users they add by email can access.

{:.center}
![]({{ site.baseurl }}/img/work_assets/open_chat/open_chat_add_user.png)

##### **Mobile Responsive Design:**

This application was created with a mobile-first, responsive design using *Bootstrap*.

{:.center}
![]({{ site.baseurl }}/img/work_assets/open_chat/open_chat_mobile_view.png)

#### **SOLUTION**

Because this is an instant messaging application, it was imperative to write the app in a way that allowed asynchronous updates as users write new instant messages. Angular.js in combination with Firebase and AngularFire were an appropriate approach to achieving the three-way data binding functionality that any good instant messaging app should have.

Open Chat was designed and structured as a Single Page Application (SPA). I used the <a href="https://ui-router.github.io/ng1/" target="_blank">UI Router</a> Angular.js plugin to take advantage of the useful "sref" attribute directive as well as a few other useful features that it provides. I implemented the *ngCookies* module to keep track of user sessions as well as *UI Bootstrap* for certain UI components such as the login, signup and new room modals.

I created custom Angular Services and corresponding Controllers to handle the creation of new rooms and new messages. I implemented AngularFire's Authentication API in conjunction with a custom Account service to correlate AngularFire user IDs with usernames and emails stored in the Firebase database. I used the AngularFire module to read and write records to the Firebase database asynchronously.

#### **CONCLUSION**

This project allowed me to flex some of my JavaScript and Angular.js skills while allowing me to learn and implement several Angular modules such as *UI Bootstrap* and *ngCookies*. Using Firebase alongside *AngularFire* was a fitting solution to allow three-way data binding between the HTML, JavaScript, and Firebase database.

##### **NEXT STEPS**

In the future, if the application and user base were to grow, it would become increasingly important to establish logic that ensures only the most recent messages get loaded from the database upon selecting a room. This would decrease the application load time and help increase the scalability of the app.

If this application were to be used consistently by live users, there would need to be some additional logic that restricts users from making unlimited public rooms. This would help prevent the database from being overloaded by users creating too many public rooms.

It would be helpful to implement a search functionality to help users find rooms if the user base and database were to grow.

Additionally, it would be important to add functionality that allows users to edit their user information such as username, email, password, etc., as well as allow them to recover their forgotten password, etc.

#### View the Project:

**<a href="https://openchat.netlify.com/" target="_blank">Open Chat</a>**

##### GitHub Repo
<a href="https://github.com/dmhuebner/open-chat" target="_blank">open-chat repo</a>
