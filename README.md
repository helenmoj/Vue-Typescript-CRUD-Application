# Vue-Typescript-CRUD-Application


 * Introduction
I followed the following tutorial:

https://bezkoder.com/vue-js-node-js-express-mysql-crud-example/
A Vue.js Typescript CRUD Application to consume REST APIs, display and modify data using Vue, Vue Router, Axios & Bootstrap.


 * Requirements

Each Tutorial has id, title, description, published status.
We can create, retrieve, update, delete Tutorials.
There is a Search bar for finding Tutorials by title.

Methods	Urls	Actions
POST	/api/tutorials	create new Tutorial
GET	/api/tutorials	retrieve all Tutorials
GET	/api/tutorials/:id	retrieve a Tutorial by :id
PUT	/api/tutorials/:id	update a Tutorial by :id
DELETE	/api/tutorials/:id	delete a Tutorial by :id
DELETE	/api/tutorials	delete all Tutorials
GET	/api/tutorials?title=[keyword]	find all Tutorials which title contains keyword


The App component is a container with router-view. It has navbar that links to routes paths.

– TutorialsList component gets and displays Tutorials.
– Tutorial component has form for editing Tutorial’s details based on :id.
– AddTutorial component has form for submission new Tutorial.

– These Components call TutorialDataService methods which use axios to make HTTP requests and receive responses. 


 * Installation

We’ve set our app running at port 8081.

Run Vue Typescript App
You can run our App with command: npm run serve.
If the process is successful, open Browser with Url: http://localhost:8081/ and check it.



 * Technology

vue: 2.6.11
vue-router: 3.1.6
axios: 0.19.2
vue-class-component 7.2.3
vue-property-decorator 8.4.1

– package.json contains main modules: vue, vue-router, vue-class-component, axios.
– There are 3 components: TutorialsList, Tutorial, AddTutorial.
– router/index.ts defines routes for each component.
– http-common.ts initializes axios with HTTP base Url and headers.
– TutorialDataService has methods for sending HTTP requests to the Apis.
– vue.config.js configures port for this Vue Client.






