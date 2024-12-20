# bookhaven-part-b-readme

## Deployed URL Link (R10)

https://wslbookhaven.netlify.app/

## Github Organization & Repositories (R11)

https://github.com/Bookhaven-WSL

https://github.com/Bookhaven-WSL/bookhaven-part-a

https://github.com/Bookhaven-WSL/bookhaven-part-b-frontend

https://github.com/Bookhaven-WSL/bookhaven-part-b-backend

https://github.com/Bookhaven-WSL/bookhaven-part-b-readme

## Pages & Functionalities

#### Signup/Login Page
The user is able to enter their details to signup if a new user or login if returning user.

#### Read Page
One of two "bookshelf" pages. Allows user to look through books they have previously added to 'Read' from the Search page. The user can add a rating between 1-5 to each title using a selector. The user can also remove a title from this page.

#### To Be Read Page
The second "bookshelf" page functions similarly to the 'Read' page. The user can remove a title from this page or can chose to move it to the 'Read' bookshelf page.

#### Search Page
The user enter the name of a book in the search field. This will display books with this title as well as related titles. The user can chose the add a title to their 'Read' bookshelf or to their 'To Be Read' bookshelf.

#### Recommendations Page
The user can enter a genre in the search field to generate suggested books based on that genre. The user can then chose to add a book to their 'Read' or "To Be Read' bookshelves.

## Description of all libraries used in the application (CMP1003-1.2)

### Backend Libraries

#### Auth
##### Bcrypt
bcrypt is a library that assist handling passwords in a secure way. Its used in this application for hashing passwords storing a random generated "hashed" password from rather than the original password. It also has the ability to "add salt" which generates a random string to add to the stored password for an extra layer of security.

##### jsonwebtoken
This library was used for authentication, as it generates a unique web token and allows its verification. The token is passed through the URL header which allows the user access to proteceted routes. 
 
#### Database
##### mongoose
This application utilised the database MongoDB, or more accurately its cloud service, Atlas. We used mongoose as the library for Object Data Modelling, allowing us to construct Schemas, query the database, validate data, and handle relationships between models.

#### Configuration and Testing
##### Jest
jest is a straight out of the box and functional testing library developed by Facebook, popularly used on React applications. It has built in functions allowing organised test suites, and is easy to create mock up tests. It also provides an output of the code the testing covers.  

##### supertest
Often used in conjuction with jest on applications, supertest is a Node.js library utilised in testing of RESTFUl API's by simulating HTTP requests and checking responses. 

#### Development
##### nodemon
nodemon is an incredibly useful tool in the Node.js development environment, automatically restarting the file on change or error, circumventing the requirement to manually restart at each update. 

##### CORS
CORS or "Cross-origin Resource Sharing" is a feature for security that disables external domains that have not been authorised from accessing materials within the protected domain. 

### FrontEnd Libraries
##### axios
axios is Javascript library used in Node.js for making asynchronous HTTP requests. This application utilised axios for seamless integration of front and back end, which made requests to an external API to return JSON data. Axios also provided inbuilt error handling and logging, which was useful in development. 

##### vitest
vitest is framework within Javascript utilised for unit testing and popular for its speed and efficiency. Without the need for external dependencies and being completely ECMAScript capable, it helps write quick and useful tests for Javascript application. 


## Trello Screenshots (CMP1002-6.2, CMP1002-7.4)

### Sprint 2



#### Meeting 3



#### Meeting 4



### Sprint 3

#### Meeting 1



#### Meeting 2



#### Meeting 3



#### Meeting 4



## Deployed URLs (CMP1002-4.2)

https://wslbookhaven.netlify.app/

https://bookhaven-part-b-backend.onrender.com/

## Development Testing (CPM1002-5.1)



## Production Testing (CPM1002-5.2)
