### Algorithms and Data Structures Enhancements
In my endeavor to demonstrate comprehension of algorithms and data structures, I determined that I needed to develop unique functions that utilized data structures to alter or modify user data. To achieve this, request and response data sent and received from either the MongoDB database or API calls required iteration and filtering of relevant data. This response data was either mapped or pushed to arrays that would then be displayed to the user. 

#### Exception Handling
In my journey through Southern New Hampshire University’s computer science program, I learned that exception handling assists with anomalies or unintended behaviors of programs. For example, since my sleep-tracking application required routes and connection with MongoDB, the addition of *then* and *catch* statements would either reroute the program’s behavior or prompt the user of the corresponding error(s) stemming from the response data of HTTP (Hypertext Transfer Protocol) request methods to the database.
Example of Exception Handling used within my program’s routing include:

`.then(() => res.json('Sleep Journal Updated!'))
 .catch(err => res.status(400).json('Error: ' + err));`
 
#### String Interpolation and Arrow Functions
Shortcuts provide the developer with the obvious time-saving attributes but also increases the readability of the source code. Such methods as string interpolation and arrow functions are two tactics used when developing the sleep-tracking application that I became very familiar with. While traditional functions and string formatting are included within my source code, I wanted to demonstrate comprehension of alternative approaches to formatting code.
String Interpolation Example:

``axios.get(`https://api.datamuse.com/words?rel_jjb=${encodeURIComponent(dreamWordParam)}`)``

####Array Manipulation
Several portions of my project included returning specific data from MongoDB with the aim of displaying that data to the user. To achieve this functionality, I decided to include arrow functions that would push specific elements from the user’s entries within MongoDB. By iterating over each element of the response data from MongoDB and storing that data in the empty array, I was able to display specific data to the user while excluding non-relevant response data.

`resData.forEach(element => {
            sleepDuration.push(element.duration)
            sleepDate.push(element.date)
          });  `
