---
layout: post
title: NextTask
feature-img: "img/work_assets/nexttask/nexttask_header2.png"
thumbnail-path: "img/work_assets/nexttask/nexttask_thumbnail.png"
short-description: NextTask - Priority driven to-do lists


---
**<a href="https://nexttask.herokuapp.com/" target="_blank" style="font-size: 2rem;">NextTask</a>**

#### **SUMMARY**

NextTask is a simple to-do list (<a href="https://en.wikipedia.org/wiki/Single-page_application" target="_blank">SPA</a>) app built with *JavaScript*, *Angular.js* and *Firebase*. It uses the Firebase *AngularFire* module to provide a real-time backend with three-way data binding. It is designed to keep your to-do lists clean and realistic by removing tasks that are not completed within seven days. The idea is that if a task is not important enough to be completed within seven days, it does not belong on your to-do list. Expired tasks are still available under the Expired list, but they will be cleared from your Current list.

{:.center}
![]({{ site.baseurl }}/img/work_assets/nexttask/nexttask_thumbnail.png)

#### **TECHNOLOGIES USED**

JavaScript, jQuery, Angular.js, Firebase, HTML5, CSS3, AngularFire, UI Bootstrap, Node.js, Git

#### **EXPLANATION**

The goal of this project was to build a straightforward to-do list app that reduces the typical clutter that can build up in your to-do lists by automatically expiring tasks older than seven days. This keeps your to-do lists clean and realistic while still providing access to expired tasks in a separate tab.

{:.center}
![]({{ site.baseurl }}/img/work_assets/nexttask/nexttask_expired_tasks.png)

Once a user marks a task as completed, it can still be viewed under the Completed Tasks tab. Tasks can also be permanently removed from your Completed Tasks by hovering over them clicking "Remove".

{:.center}
![]({{ site.baseurl }}/img/work_assets/nexttask/nexttask_remove_tasks.png)

NextTask has a clean, mobile responsive design and uses *<a href="https://angular-ui.github.io/bootstrap/" target="_blank">UI Bootstrap</a>*'s Modal service as well as *<a href="https://github.com/firebase/firebaseui-web" target="_blank">FirebaseUI</a>* for user authentication.

#### **PAGES**

##### **Homepage:**

{:.center}
![]({{ site.baseurl }}/img/work_assets/nexttask/nexttask_homepage2.png)

##### **Sign In Modal:**

Users can either click "Sign In" to create a new free account with their email or sign in to an existing account to start creating new tasks.

{:.center}
![]({{ site.baseurl }}/img/work_assets/nexttask/nexttask_signin.png)

{:.center}
![]({{ site.baseurl }}/img/work_assets/nexttask/nexttask_signin2.png)

If there is no account associated with the user's email they will be prompted to create a new user account.

{:.center}
![]({{ site.baseurl }}/img/work_assets/nexttask/nexttask_signin3.png)

Once a user logs in they will be directed to the tasks index view where they can create new tasks, mark tasks as complete and view any expired or completed tasks.

Users can log out by clicking the "Logout" button in the top right. Logging out destroys the user session.

<!-- #### **SOLUTION** -->

#### **CONCLUSION**

This project allowed me to practice and demonstrate my programming and web development skills using JavaScript, Angular.js and Firebase as well as solve a problem that I often run into with many other to-do applications.

##### **NEXT STEPS**

The next steps for this project would be to implement a function that allows users to refresh an expired task and add it back to their Current Tasks list. Although I do love the simplicity of just having one list, it may be best to add the ability to make more than one list for users who may have that need.

#### View the Project:

**<a href="https://nexttask.herokuapp.com/" target="_blank">NextTask</a>**

##### GitHub Repo
<a href="https://github.com/dmhuebner/nexttask" target="_blank">NextTask repo</a>
