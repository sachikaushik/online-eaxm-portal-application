
<div align="center">
  <h1>Online Exam Portal</h1>
  <p>
    A Online Exam portal website with backend in Nodejs and frontend in React js 
  </p>

</div>

<br />

<!-- Table of Contents -->
# :notebook_with_decorative_cover: Table of Contents

- [About the Project](#star2-about-the-project)
  * [Tech Stack](#space_invader-tech-stack)
  * [Features](#dart-features)
  * [Environment Variables](#key-environment-variables)
- [Getting Started](#toolbox-getting-started)
  * [Prerequisites](#bangbang-prerequisites)
  * [Run Locally](#running-run-locally)
  * [Run with Docker](#run-with-docker)
- [To-do](#notes-to-do)
- [Contributing](#wave-contributing)
- [License](#warning-license)
- [Contact](#handshake-contact)
- [Acknowledgements](#gem-acknowledgements)

  

<!-- About the Project -->
## :star2: About the Project
  Web Application for online MCQ test usecase


<!-- TechStack -->
### :space_invader: Tech Stack

<details>
  <summary>Frontend</summary>
  <ul>
    <li><a href="https://reactjs.org/">React.js</a></li>
    <li><a href="https://react-redux.js.org/">React-Redux</a></li>
    <li><a href="https://www.mui.com">Material UI library</a></li>
    <li><a href="https://html.com/html5/">HTML 5</a></li>
    <li><a href="https://www.css3.com/">CSS 3</a></li>
  </ul>
</details>

<details>
  <summary>Backend</summary>
  <ul>
    <li><a href="https://www.nodejs.org">Node.js</a></li>
    <li><a href="https://www.expressjs.com/">Express.js</a></li>
    <li><a href="https://www.passportjs.org/">Passport.js</a></li>
  </ul>
</details>

<details>
<summary>Database</summary>
  <ul>
    <li><a href="https://www.mongodb.com/">MongoDB</a></li>
  </ul>
</details>


<!-- Features -->
### :dart: Features

- Student User
  - View Tests Details
  - Register for test
  - Give Test
  - Check Result and correct answer and explanation for questions
- Teacher User
  - Create, Update Questions and Question Banks
  - Create, View Test
- Admin User
  - Create and Manage Teacher users
  - Create and Manage subjects


<!-- Env Variables -->
### :key: Environment Variables

To run this project, you will need to add the following variables to your backend/config.json file

`mongodb.connectionString`
`jwt.secret`

<!-- Getting Started -->
## 	:toolbox: Getting Started

<!-- Prerequisites -->
### :bangbang: Prerequisites

This project uses MongoDB as database. please install mongodb server in local environment.

<!-- Run Locally -->
### :running: Run Locally

Clone the project

```bash
  git clone https://github.com/chintan-golakiya/online-exam-portal.git
```

Go to the project directory

```bash
  cd project-directory
```

Install dependencies

```bash
  cd backend
  npm install
  cd ../frontend
  npm install
  cd ../user-portal-frontend
  npm install
```

Start the backend server

```bash
  cd backend
  npm start
```

Start the frontend client for admin

```bash
  cd frontend
  npm start
```

Start the frontend client for teacher/student

```bash
  cd user-portal-frontend
  npm start
```

<b>Note</b> : admin user is created when backend runs first time. default admin (username, password) details are <b>("sysadmin","systemadmin"). addAdminIfNotFound() function of backend/services/admin.js file </b> is for this logic. You can check/modify default admin details from this function.

<!-- Run with Docker -->
### Run With Docker

build docker images

```bash
  docker-compose build
```

Run container and services

```bash
  docker-compose up
```

Use following paths 

```bash
  Backend server : localhost:5000/
  Admin Frontend : localhost:3100/
  User  Frontend : localhost:3200/
```







<!-- Acknowledgments -->
## :gem: Acknowledgements
Following libraries have been used in this projects.

 - [Material UI](https://www.mui.com)
 - [Passport JS](https://www.passportjs.org/)
 - [Awesome Readme Template](https://github.com/Louis3797/awesome-readme-template)
