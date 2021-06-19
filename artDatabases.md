### Database Enhancements
For the database enhancements portion of my project, I decided to include a MongoDB Atlas interface that used the Express web application framework routing and Mongoose document-modeling. I determined that my project required three collections that would store the user’s credentials, their sleep journal entries, and their sleep goal entries. Each entry, or document, would store data types ranging from strings, numbers, and dates.

#### Object Data Modeling
As mentioned above, the username, sleep journal, and sleep goal included string, number, and date data types, but I also required rules that would govern the user’s inputs. I applied rules to each model field that included data types, required inputs, unique inputs, default values, min/max lengths, and timestamps. 
Example of Username field:
`username: { type: String, required: true, unique: true, minLength: 3, maxLength: 10 }, `

#### CRUD Operations
My project required the ability to CRUD or create, read, update, and delete data entries from the user. To achieve this functionality, HTTP (Hypertext Transfer Protocol) request methods such as *post*, *get*, and *delete* were used in conjunction with the request data of the user and response data in JSON (JavaScript Object Notation) format. Built-in MongoDB function such as `findById` or `findByIdAndDelete` were used with the corresponding HTTP request method and request parameters.

#### Routing
To make use of the document modeling and CRUD operation, I needed to route the user’s actions to the corresponding query parameters. I also endeavored to adhere to a RESTful or Representational State Transfer model with HTTP verbs and explicit URI (Uniform Resource Identifier) pathing naming conventions. Such routing paths as `router.route('/add').post((req, res)` or `app.use('/sleepgoals', sleepGoalRouter)` explicitly identify and explain the actions taking place.

### Justification
I decided to use MongoDB’s NoSQL (Not only Structured Query Language) format since my sleep-tracking application would utilize various data types and document-style description string inputs of varying lengths. Before starting this project, I considered implementing Structured Query Language or SQL, but decided against this format since this database format was restrictive when compared with NoSQL. The aim of using MongoDB routing, document modeling, and request methods was to demonstrate my comprehension of backend to frontend communication and database modeling. 

### Reflection
Looking back, I believe that utilizing a NoSQL database like MongoDB was advantageous because the database format offered me more flexibility in the data types and schema-less modeling that I could apply to my project. By selecting to use a NoSQL database like MongoDB, I found that a schema-less approach to storing user data in a less restrictive manner offers the ability to scale horizontally with ease.

[back](index.html)
