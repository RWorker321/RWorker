###Software Design and Engineering Enhancements
<p>The categories of enhancements for this artifact included improving a piece of software, transferring a project into a different language, reverse engineering a piece of software for a different operating system, or expanding a project’s complexity. I selected to expand a project’s complexity by reworking and developing additional functionality to a MERN (MongoDB, Express, React, Node.js) STACK Exercise-Tracker created by Beau Carnes (2019).</p>

####Restructuring and Altering the Theme
The first enhancement was altering the overall theme of the project. I selected to migrate the exercise-tracking theme to a sleep-tracking theme. The exercise-tracking template included the ability to CRUD (create, read, update, and delete) user credentials and exercise descriptions. Since the template included usernames, I renamed the exercises collection to Sleep Journal and added a Sleep Goals collection within my MongoDB database.

####Sleep Metrics Line Chart
In order for the user to track their sleeping habits, I decided to expand the functionality of the sleep-tracking template with the addition of a line chart that tracked the sleep duration logged and date of entry logged within the user’s sleep journal. The first step was to install and import the “react-chartjs-2” library. The dataset applied to the line chart required creating a function responsible for HTTP (Hypertext Transfer Protocol) request method to the MongoDB Sleep Journal collection. I expand upon this functionality in the [Algorithms and Data Structures](./artAlgoDataStruct.html)  portion of my project.

####Dream Word Interpreter
I endeavored to add unique functionality and complexity to my project, so I decided to add a feature I have never seen before in a sleep-tracking application. This feature included the ability to review the sleep journal description entries, select and input a word into the “Dream Word Interpreter”, and return similar words so the user can attempt to decrypt their dream’s meaning. To accomplish this feature, I added a React component that displayed the user’s sleep journal description entries, prompted the user to input a word into the search bar, and returned a word from the [DataMuse]( https://www.datamuse.com/api/) API relating to the user’s selected word. 

####NASA Open API
To add more complexity to the application, the second enhancement was a React component with the functionality of an API (application programming interface) call to [NASA’s Astronomy Picture of the Day] (https://apod.nasa.gov/apod/astropix.html). With the help of a tutorial from the YouTube channel Kapehe _ok (2020), I was able to create a React component that would return a new astronomy-related image each day with a description of the image.

###Justification
The aim with reworking and adding React components with unique functionality and complexity and hosting this project on my ePortfolio was to demonstrate that I could migrate, design, and engineer a project template into an application that fits the user’s requirements. I also endeavored to demonstrate that I could develop unique functionality that is practical and easily accessible. 

###Reflection
Looking back after reworking the initial exercise-tracking template into a sleep-tracking application with complex and unique functionality, I found that the iterative approach to designing and developing projects has many advantages. These advantages include the ability to test and interact with semi-functional components early in the development process and determine if the project’s working prototype is moving closer towards the desired end goal.

####Resources:
Carnes, B. (2019, June 25). Learn the MERN Stack – Full Tutorial (MongoDB, Express, React, Node.js). [Video File]. YouTube. https://www.youtube.com/watch?v=7CqJlxBYj-M
Kapehe _ok. (2020, May 13). Make a Stellar React + NASA API App. [Video File]. YouTube. https://www.youtube.com/watch?v=H1nENYv-r_w&ab_channel=Kapehe_ok
