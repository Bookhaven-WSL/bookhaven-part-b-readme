# T3A2-B Bookhaven

## Deployed URL Link (R10)

https://wslbookhaven.netlify.app/

## Github Organization & Repositories (R11)

https://github.com/Bookhaven-WSL

https://github.com/Bookhaven-WSL/bookhaven-part-a

https://github.com/Bookhaven-WSL/bookhaven-part-b-frontend

https://github.com/Bookhaven-WSL/bookhaven-part-b-backend

https://github.com/Bookhaven-WSL/bookhaven-part-b-readme

## Application Setup

A Database access has been created with the user details:
username: assessor_1
password: assessor1password

The below includes the varabiales for jwt secret key and database URL for the `.env`

JWT_SECRET_KEY=LouisWadeAndSophieAreTheBestDevelopersToHaveEverDoneItAtCoderAcademy

DATABASE_URL=mongodb+srv://assessor_1:assessor1password@bookhaven.zkbzo.mongodb.net/?retryWrites=true&w=majority&appName=BOOKHAVEN


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

Continuing on from T3A2-A, our team utilised a Trello based kanban board for project management. Some example cards along with the progress of the assignment can be seen below:

### Example Cards

![Example_Card_1](./docs/Trello/trello_card.png)

![Example_Card_2](./docs/Trello/Trello_Card2.png)

### Sprint 2

#### Meeting 3

![Sprint_2_Meeting_3](./docs/Trello/Trello_Sprint2_Meeting3.png)

#### Meeting 4

![Sprint2_Meeting_4](./docs/Trello/Trello_Sprint2_Meeting4.png)

### Sprint 3

#### Meeting 1

![Sprint3_Meeting_1](./docs/Trello/Trello_Sprint3_Meeting1.png)

#### Meeting 2

![Sprint3_Meeting_2](./docs/Trello/Trello_Sprint3_Meeting2.png)

#### Meeting 3

![Sprint3_Meeting_3](./docs/Trello/Trello_Sprint3_Meeting3.png)

#### Meeting 4

![Sprint3_Meeting_4](./docs/Trello/Trello_Sprint3_Meeting4.png)

## Deployed URLs (CMP1002-4.2)

https://wslbookhaven.netlify.app/

https://bookhaven-part-b-backend.onrender.com/

## Testing (CPM1002-5.1, CPM1002-5.2)

When conducting testing on this application, Insomnia was primarily utilised, with some use of the broswer console logs for production testing. See screenshots below:

### Development

![DEV/](./docs/Insomnia/DEV/DEV:.png)

![DEV/auth/signup](./docs/Insomnia/DEV/DEV:auth:signup.png)

![DEV/auth/login](./docs/Insomnia/DEV/DEV:auth:login.png)

![DEV/user/update](./docs/Insomnia/DEV/DEV:user:update.png)

![DEV/user/delete](./docs/Insomnia/DEV/DEV:user:delete.png)

![DEV/book](./docs/Insomnia/DEV/DEV:book.png)

![DEV/book/to-be-read](./docs/Insomnia/DEV/DEV:book:to-be-read.png)

![DEV/book/read](./docs/Insomnia/DEV/DEV:book:read.png)

![DEV/book/delete](./docs/Insomnia/DEV/DEV:book:delete.png)

![DEV/book/update](./docs/Insomnia/DEV/DEV:book:update.png)

![DEV/book/recommended](./docs/Insomnia/DEV/DEV:book:recommended.png)

![DEV/book/search-personal](./docs/Insomnia/DEV/DEV:book:search-personal.png)

![DEV/book/to-be-read](./docs/Insomnia/DEV/DEV:book:to-be-read.png)

![DEV/book/read_get](./docs/Insomnia/DEV/DEV:book:read_get.png)

![DEV/book/recommended_get](./docs/Insomnia/DEV/DEV:book:recommended_get.png)

![DEV/book/search-new](./docs/Insomnia/DEV/DEV:book:search-new.png)

### Production

![PROD/](./docs/Insomnia/PROD/PROD:.png)

![PROD/auth/signup](./docs/Insomnia/PROD/PROD:auth:signup.png)

![PROD/auth/login](./docs/Insomnia/PROD/PROD:auth:login.png)

![PROD/user/update](./docs/Insomnia/PROD/PROD:user:update.png)

![PROD/user/delete](./docs/Insomnia/PROD/PROD:user:delete.png)

![PROD/book](./docs/Insomnia/PROD/PROD:book.png)

![PROD/book/to-be-read](./docs/Insomnia/PROD/PROD:book:to-be-read.png)

![PROD/book/read](./docs/Insomnia/PROD/PROD:book:read.png)

![PROD/book/delete](./docs/Insomnia/PROD/PROD:book:delete.png)

![PROD/book/update](./docs/Insomnia/PROD/PROD:book:update.png)

![PROD/book/recommended](./docs/Insomnia/PROD/PROD:book:recommended.png)

![PROD/book/search-personal](./docs/Insomnia/PROD/PROD:book:search-personal.png)

## Part A content (R12)

# T3A2-A Bookhaven

### Created in collaboration by Sophie Woolford, Wade Venz & Louis Denman

## R1: Project Purpose & Description

As a group who thoroughly appreciates a good read, but are in a digital age where the physical form factor of information is becoming less common, we wanted somewhere that our reading history could be stored. A digital personal library, so to speak, is something that we envision as a benefit to those who read anywhere around the world. When we researched current applications that tried to bring this concept to life, however, none really ticked all the boxes for the casual book enjoyer. Goodreads, whilst being owned by Amazon, has seen little support or development over its lifetime and has a range of issues that arn't appreciated by its users. Bookworm, whilst being about community and connectedness between likeminded individuals, can create a competitiveness that takes the focus off the enjoyment of reading and instead highlight how many books someone has read. Storygraph delves deep into the data and trends of an individuals reading habits, Bookly focuses on building reading habits, Readerly focuses on the reviewing of books, the list goes on.

In summary, we found that there is a range of services out there for the casual reader, but none that keep it simple. None that keep it about the individual reader, and keep it simply about the books they have read and want to read. As a result, our team endevours to make the perfect, simple digital library web application that is built for the casual individual reader. The web app will be an aesthetically pleasing, responsive, and allow users to:

- Easily sign up & log in
- Create a list of books that the reader has read
- Create a list of books that the reader would like to read
- Allow the reader to search for books to add to the above two lists mentioned
- Allow the reader to put a simple rating on books they have read if they choose
- Display recommendations for the reader based on what they have read previously
- Allow the reader to add custom book entries
- Enable child accounts that stop the addition of inappropriate books

Our team is utilising the MERN stack (MongoDB, Express, React, Node) framework for the creation of our web app, along with a range of npm package dependancies including:
- Jsonwebtoken
- Dotenv
- Bcrypt
- Mongoose
- Cors
- Nodemon

For deployment, we will be using netlify for the front-end, along with render for the back-end. Project management is conducted on Trello, while version control is handled by Git and Github. Shared file storage is handled by Google Drive.

## R2: Dataflow Diagrams

Below are representations of data flow for the virtual bookshelf application, BookHaven. The diagrams are layers that build on the high level application architecture diagram, and utilise the notation standard of Yourdon and Coad(1), where external entites are represented in rectangles and processes in circles. 

### Virtual Bookshelf - Layer 1

![DFD Layer 1](./docs/Dataflow_and_Architecture/bookhaven_dfd_layer1.png)

### Auth Data Flow - Layer 2

##### Sign-up User

![Auth Signup Layer 2](./docs/Dataflow_and_Architecture/bookhaven_dfd_layer2_auth_signup.png)

1. A POST request is sent by the user to the `/auth/signup` endpoint with user information such as name, email & password. 
2. User details will be passed to a function to handle user registration. First user details will be validated for proper format and the email provided will be checked to verify that it is unique. The password will also be hashed for extra security.
3. If validation criteria is not met or the email is not unique, an error message will be sent back to the client. 
4. User will be saved with a userId, user details and the hashed password to the database.
5. User ID and email passed to a function to generate a JSON web token or JWT.
6. The JWT is passed back to the user on the front end to be stored and utilised for authentication. 




##### Login User

![Auth Login Layer 2](./docs/Dataflow_and_Architecture/bookhaven_dfd_layer2_auth_login.png)

1. A POST request sent to the `/auth/login` endpoint with email and password. 
2. Details are sent to Backend Server, where a function to handle login is located within the Auth controller. Details are initially checked against validation format, and if criteria isn/t met, an error message is sent back to the user. 
3. Email/userId is sent to be checked within the database for existing records using an async function
4. If email/userId exists within database records, the document with the user details and hashed password is sent back to the server for use within the handleLogin() function.
5. The hashed password received from the document retrieved is verified, if not verified, an error is sent back to the user. 
6. A JWT is generated via a function with userId and email passed as parameters.
7. The JWT is then returned to the user on the front end for storage, alongside the userId, the saved preferences for UI/UX and any permissions associated with that user. The JWT is sent as a header for all further user requests within the application until it expires as specified when the token is generated. 

### User Data Flow - Layer 2 **Optional Functionality** 

##### Update User

![Update user](./docs/Dataflow_and_Architecture/bookhaven_dfd_layer2_update_user.png)

1. PUT/PATCH requested by user, sent with a _id to server
2. Server receives request and validates, returning an error if occurs.
3. Query is sent to the database by the server to update data.
4. The database receives and executes the request sending a response.
5. Response is returned to user. The front end React app then saves the changes in state.  

##### Delete User

![Delete user](./docs/Dataflow_and_Architecture/bookhaven_dfd_layer2_delete_user.png)

1. DELETE requested by user, sent with a _id to server
2. Server receives request and validates, returning an error if occurs.
3. Query is sent to the database by the server to delete data.
4. The database receives and executes the request sending a response.
5. Response is returned to user. The front end React app then saves the changes in state.

### Bookshelf Interaction - Layer 2

##### Adding a new book to shelf

![Add a Book](./docs/Dataflow_and_Architecture/bookhaven_dfd_layer2_add_book.png)

1. The client decides to add a new book to virtual bookshelf by creating a search query.
2. A request will be sent to an external API asynchronously to search for a book that meets criteria inputted by user. Books can searched by title, author, or id's such as ISBN.
3.  If found in the API the book will be returned in JSON format, else an error will be caught. 
4. Error or book data is returned.
5. The details in the book record will be passed to another function that will handle its storage in the database. 
6. The book is saved to the database associated with the User collection.
7. The book is returned to the front end for the user and saved by the React app. 


##### Find a new book

![Find a book](./docs/Dataflow_and_Architecture/bookhaven_dfd_layer2_find_book.png)

1. GET request is triggered by user on front end and sent to the server. 
2. A function to handle to handle the fetch request receives the requests and handles validation. The server then sends a query to the API.
3. The API receives the request and returns an array of book objects based on parameters. 
4. The information is sent back to the front end for the user and saved by the React app for further interaction by the client, potentially to be added and saved to the database.  

##### Recommendations

![Recommended](./docs/Dataflow_and_Architecture/bookhaven_dfd_layer2_recommended.png)

1. A fetch request is triggered by user on the front end. 
2. A function to handle recommendations in the server receives the GET request. This function handles both async functions for database and API request. 
3.  This function handles the asynchronous call to the database to collect data from saved books utilising userId to collect associated book documents. 
4. Database receives the request and sends back an array of book objects.
5. The array of book objects is then sent to the handle recommends function to isolate query parameters for a request to the API, based on the data collected from the database.
6. The parameters from handle recommendation are sent to the second async function to request books from the API. 
7. The request is sent to the API to collect book data matching parameters.
8. Return an array of book objects to the server. 
9. The handle recommend function will further validate the data to be sent back to the front end.
10. A final array of book objects will be sent to the front end and saved in state. 

##### Update Book

![Update book](./docs/Dataflow_and_Architecture/bookhaven_dfd_layer2_update_book.png)

1. PUT/PATCH requested by user, sent with a _id to server
2. Server receives request and validates, returning an error if occurs.
3. Query is sent to the database by the server to update data.
4. The database receives and executes the request sending a response.
5. Response is returned to user. The front end React app then saves the changes in state. 

##### Delete Book

![Delete book](./docs/Dataflow_and_Architecture/bookhaven_dfd_layer2_delete_book.png)

1. DELETE requested by user, sent with a _id to server
2. Server receives request and validates, returning an error if occurs.
3. Query is sent to the database by the server to delete data.
4. The database receives and executes the request sending a response.
5. Response is returned to user. The front end React app then saves the changes in state


(1) Virtual Paradigm, 2024, sourced November 2024, https://online.visual-paradigm.com/knowledge/software-design/dfd-tutorial-yourdon-notation


## R3: Application Architechture Diagram

A high level diagram for the archtiecture of the application. 

![Architecture Diagram](./docs/Dataflow_and_Architecture/bookhaven_architecture_diagram.png)

## R4: User Stories

As recommended by the assessment criteria, the intial user story format used was the **As a [persona], I [want], so [that].**

To begin, an initial iteration of users stories was created to address the features that we intend to implement within the web app, as seen below:

*Iteration 1:*

- My name is Jill, and as someone who enjoys reading, I want to track which books I’ve read, so I can talk about it with other friends who like reading.
- My name is John, and as someone who reads here and there, I want to make a list of new books to read, so that I can get more into reading.
- My name is Jeff, and as someone who passionately reads, I want to be able to rate books that I’ve read before, so that I can see what I thought of each book.
- My name is Jack, and as someone who has a grandpa that loves reading, I want to be able to make a simple account for him that is easy to add books he’s read too, so that he can remember which ones he has read.
- My name is Janette, and as someone who likes reading to relax, I want to have new books recommended to me, so that I can find more books that are relaxing to read.
- My name is Jeremy, and as someone who has young children that enjoy reading, I want my kids not to be able to see books that are inappropriate, so that they then go read them and learn bad things.
- My name is Jesiah, and as someone who likes studying old texts, I want to be able to add custom books that otherwise wouldn’t show up.

This set of users stories addressed the functionality of the app, but would benfit from some further depth about the user, as well as specificity about what it is they want to achieve. As a result, the individual users were given some more depth and background:
- *Jill:* Jill is a 29 year old woman who has been a bookworm since she was a child. Whenever she has free time, her favorite activity is to go for a walk to the park or beach if she is nearby, and read her book for as long as she can. She moved away from her high-school friends who also enjoy reading, but catches up with them once or twice a year.
- *John:* John is a 31 year old man who works a hard labor job. He gets up early for work to provide for his wife and young child, but feels the effects of this work over the years starting to take effect on him. He has never been a big reader, but wants to start doing so consistently, as he is trying to read books on financial freedom and other finance/self-improvement topics.
- *Jeff:* Jeff is a 19 year old student who studies a bachelor of arts with a major in English literature. He thoroughly enjoys the process of analyzing/comparing different books and other written works. Whenever he sees his classmates or professor after class, he loves discussing personal takes on particular authors' pieces of work, and debating the quality of pieces that are covered in class.
- *Jack:* Jack is a 22 year old man who works hard to provide for himself and his grandparents, who have raised him for the better part of his life. He has never been a big reader himself, but his grandpa loves reading. Unfortunately, his grandpa in his old age has begun to have memory problems, and sometimes picks up books only to find that he has already read them and knows the story. Jack feels sorry for his grandpa, but doesn’t know a good system to help him.
- *Janette:* Janette is a 32 year old woman who was diagnosed with anxiety in her late 20s. Looking back, it was obvious this was the case, she despised having to go out of the house for anything; getting groceries; going to school or university; previous commutes to the office; even going to and from friends' places. These days she is able to work a remote job from the comfort of her own home, but when she does have to journey out on occasion, she reads to calm down before and after her journey.
- *Jeremy:* Jeremy is a 38 year old man who is the proud father of 1 boy and 2 girls under the age of 10. Like their parents, they all love reading, and go through lots of books in a year. Unfortunately, when Jeremy was younger he found some books that contained inappropriate content, of which took him a while to work through. He doesn’t want that to happen to his kids, but loathes the process of having to check through every book for any inappropriate content, given his busy schedule and the rate at which his children read.
- *Jesiah:* Jesiah is a 20 year old who loves history. During high-school, he would not do well in his other class, but in both modern and ancient history would score 100%. In particular he had a fascination for older literature and texts, and loves to study as much as he can get his hands on.

With the further persona development established, the user stories could be revised with more detail and depth, so that they become even more useful and clear:

*Iteration 2:*

- My name is Jill, and as someone who has enjoyed reading since childhood, I would like to be able to keep a record of all the previous books I have read, so that when I catch up with my childhood friends who also enjoyed reading we can talk about all the books we have read together.
- My name is John, and as someone who reads occasionally but is trying to get more consistent, I would like to be able to make a list of books that I want to read in the future, so that I can look at my list and stay motivated to keep reading the book that I am on and get excited for the books I plan to read next.
- My name is Jeff, and as a passionate reader who has read a large number of books and had a unique opinion on most of them, I would like to be able to create a rating for each book that I’ve read, so that I can easier recall my opinions of particular books and weigh in my opinions/thoughts in group discussions such as when I’m at book clubs or conventions.
- My name is Jack, and as someone who has a grandpa that loves reading, but is getting to an age where he struggles to use technology and remember some things, I would like to be able to make a simple account for my grandpa that he is able to easily use and log in to, so that he can have help remembering which books he has read and wants to read.
- My name is Janette, and as someone who has anxiety and doesn’t like browsing the library or being in public places for long amounts of time, I would like to have books be recommended to me based upon what I have read before, so that I know what books I am looking for before I go in the library and can make the trip as quick as possible.
- My name is Jeremey, and as someone who has children that are under 10 years of age and read lots for a hobby, I would like a type of account that does not allow books that aren't appropriate to be displayed for users to look at, so that my children do not find a book that I don’t check and it ends up being inappropriate.
- My name is Jesiah, and as someone who enjoys studying history and lots of ancient texts from different cultures, I would like to be able to make custom book entries that correspond with these texts that I study, so that I have a record of which texts I have read and intend to research in the future.


## R5: Wireframes
For the pages that store each collection of books - ‘Reads’ and ‘TBR’ (To Be Read) - that the user has saved, we wanted to emulate the appearance of bookshelves with the simplistic design, displaying the front cover of the books with minimal other information. To display more information about a book, the user clicks (mobile) or hovers over (desktop) the relevant book. This will display the book’s title and author, as well as the user’s rating on the ‘Reads’ page.

With the simplistic design of the pages that display the “bookshelves”, we decided to make separate pages for the ‘search‘ and ‘recommendations’ pages. This was because we wanted to display more information per book on these pages, so by making them separate we were able to keep the simplistic design of the “bookshelf pages.”
Once this decision was made we needed to add more buttons to the top of the page, and since this made the number of buttons four, we decided that a navigation bar was a better option, to keep the buttons organised. A search option was also added on the bar for the ‘Reads’ and ‘TBR’ pages so that a user quickly and easily can locate a book they have previously stacked there.

<details>
<summary>Mobile version</summary>

![Mobile - reads](./docs/Wireframes/Mobile%20-%20reads.png)
The menu button and enhancement glass will be static on the page so that the user can easily navigate to other pages of the app without having to scroll back to the top.

![Mobile - menu expanded](./docs/Wireframes/Mobile%20-%20menu%20expanded.png)
The menu expands over the top of the other elements on the page.

![Mobile - tbr](./docs/Wireframes/Mobile%20-%20tbr.png)
The stacking of the book covers represents the look of books on a shelf, keeping the interface clean and simple.

![Mobile - add](./docs/Wireframes/Mobile%20-%20add.png)
If no books have been added to the 'Reads' shelf, the below error message will be displayed.

![Mobile - recs](./docs/Wireframes/Mobile%20-%20recs.png)
This error message is displayed on the 'Reads' page if no books have been added to it, on the 'TBR' page if no books have been added to it, and on the 'recs' page if no books have been added to the 'Reads' page. An error message is also shown if the user searches for a book in the navbar integrated search bar that has not been added to a shelf.

![Mobile - error message](./docs/Wireframes/Mobile%20-%20error%20message.png)
Underneath the error message is a button that will redirect the user to the 'add' page, to prompt the user to add books, which will remove the error message.

![Mobile - sign up-in](./docs/Wireframes/Mobile%20-%20sign%20up-in.png)
</details>

<details>
<summary>Desktop version</summary>

![Desktop - reads](./docs/Wireframes/Desktop%20-%20reads.png)
The books are equally spaced across the page in rows of five.  This is to simulate the appearance of a bookshelf for the theme of the app. In the desktop version there is a navigation bar for the user to navigate between pages rather than a collapsible menu like on the mobile version. This allows a one-click path to the user's desired page.

![Desktop - title selected](./docs/Wireframes/Desktop%20-%20title%20selected.png)
On the desktop version, the user only needs to hover over a title to display more information, rather than clicking on it like in the mobile version. This is will allow a soft flow between selected titles.

![Desktop - search title](./docs/Wireframes/Desktop%20-%20search%20title.png)
The search bar is integrated into the navbar for a simplistic look, and only expands when the user clicks on the enhancement glass.

![Desktop - tbr](./docs/Wireframes/Desktop%20-%20tbr.png)
![Desktop - add](./docs/Wireframes/Desktop%20-%20add.png)
The add page prompts the user to search for a title using the search bar.

![Desktop - recs](./docs/Wireframes/Desktop%20-%20recs.png)
![Desktop - error message](./docs/Wireframes/Desktop%20-%20error%20message.png)
![Desktop - sign up-in](./docs/Wireframes/Desktop%20-%20sign%20up-in.png)
</details>

## R6: Project Management

For our team planning and management, we choose Trello as the tool of choice, tracking our agile fortnight long sprints. Within each sprint, we conducted 4 meetings/stand-ups (2 per week), and continued to communicate via discord in the meantime. Below is an example task card, along with the progression of our Trello board from the beginning to the end of T3A3 Part A:

### Card Example

![Card Example](./docs/Trello/CardExample.png)

### Sprint 1

#### Meeting 1

![Sprint 1, Meeting 1](./docs/Trello/Trello_Sprint1_Meeting1.png)

#### Meeting 2

![Sprint 1, Meeting 2](./docs/Trello/Trello_Sprint1_Meeting2.png)

#### Meeting 3

![Sprint 1, Meeting 3](./docs/Trello/Trello_Sprint1_Meeting3.png)

#### Meeting 4

![Sprint 1, Meeting 4](./docs/Trello/Trello_Sprint1_Meeting4.png)

### Sprint 2

#### Meeting 1

![Sprint 2, Meeting 1](./docs/Trello/Trello_Sprint2_Meeting1.png)

#### Meeting 2

![Sprint 2, Meeting 2](./docs/Trello/Trello_Sprint2_Meeting2.png)

