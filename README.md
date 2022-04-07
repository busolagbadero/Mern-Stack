# Mern-Stack
First step was to create a virtual server with Ubuntu Server OS.
![instance ubuntu](https://user-images.githubusercontent.com/94229949/162083495-4f338211-5218-4212-a274-fc21a16f43ab.png)
I used mobaxterm to connect to EC2 Instances.
I Created a new directory for my To-Do project called Todo.went ahead to initialise my project using  npm init, a new file named package.json was created.


The next step ,i installed Expressjs with command npm install express. I then went ahead to create a file called index.js.

installed dotenv module and  my next step was to write into the index.js file with command vim index.js where i input and save code.


i put in the Ip address of the instance on browser
![installed expressjs  browser](https://user-images.githubusercontent.com/94229949/162085376-2565b653-871d-4578-ac43-d0be77aeee9e.png)


To create my To-do app , App task needs to be associated with some particular endpoint and will use different standard HTTP request methods like POST,GET and DELETE for each task, I  created routes that will define various endpoints that the To-do app will depend on.

I created a folder called routes and  a file called api.js in routes directory.

I opened api.js to input and save code for the app.

I installed a database called mangodb to store data.I created a model to define the database schema which is important to define the fields stored in each Mongodb document. 

To create a Schema and a model, i installed mongoose which is a Node.js package that makes working with mongodb easier.i ran three commands mkdir models && cd models && touch todo.js and then VI into todo.js to input and save code.

I updated the api.js in routes directory with my code.

I added the connection string to access the database 
![mangodb database](https://user-images.githubusercontent.com/94229949/162091938-9918cfb3-818e-4d9d-818f-f43920aad454.png)

To start the server ,I ran command node index.js 
![database connected](https://user-images.githubusercontent.com/94229949/162092296-19167678-a1bd-42f8-b071-57f29fc65bd4.png)

To Test Backend Code without Frontend ,I installed  Postman .
![get postman](https://user-images.githubusercontent.com/94229949/162092735-cb7eaba8-f522-44ef-9780-97f142100f71.png)
![real get postman](https://user-images.githubusercontent.com/94229949/162092807-37fc0b43-70bf-450d-8763-f79e6d4dd7eb.png)

The next step was the Frontend Creation

 To start out with the frontend of the To-do app, I used the create-react-app command to scaffold our app.in the todo directory.
 
 
To run my React app,i installed concurrently which is used to run more than one command simultaneously from the same terminal window and then install nodemon. In case there is any change in the server code, nodemon will restart it automatically and load the new changes.

To Configure Proxy in package.json ,I Changed directory to ‘client’ then Open the package.json file and add  the key value pair in the package.json file "proxy": "http://localhost:5000".to make it possible to access the application directly from the browser by simply calling the server url like http://localhost:5000 rather than always including the entire path like http://localhost:5000/api/todos.To run the app  i ran command npm run dev.

To Create React Components ,I created a folder called components under the src folder which is under Todo/client. In the components folder i created three files Input.js, ListTodo.js and Todo.js. where i inputed and saved my codes.I installed Axios which is a Promise based HTTP client for the browser and node.js

In the src directory i opened the App.css and index.css to input and save code.

I ran npm run dev.
![final real project](https://user-images.githubusercontent.com/94229949/162097635-0cb19fa3-37b0-4474-818f-ad982a0e8f89.png)
