<a id="readme-top"></a>

<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#license">License</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

## About The Project

Not sure what should be your next read? Checkout this Book Discovery App! 



<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

- [![TypeScript][TypeScript.js]][TypeScript-url]
- [![React][React.js]][React-url]
- [![Spring Boot][SpringBoot]][SpringBoot-url]
- [![MySQL][MySQL]][MySQL-url]


<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->

## Getting Started

### Prerequisites

Before you begin, ensure you have the following software and tools installed on your local machine:

1. **Node.js and npm**  
   Node.js is required to run the JavaScript runtime environment, while npm (Node Package Manager) manages packages for your React and TypeScript application.

   - **Install npm and Node.js**:  
     Download the latest version of Node.js, which includes npm, from the [official Node.js website](https://nodejs.org/).

   - **Verify installation**:
     ```sh
     node -v
     npm -v
     ```

2. **TypeScript**  
   TypeScript is a superset of JavaScript that adds static types. It's required for developing TypeScript applications.

   - **Install TypeScript**:
     ```sh
     npm install -g typescript
     ```

   - **Verify installation**:
     ```sh
     tsc -v
     ```

3. **Java Development Kit (JDK) 17 or higher**  
   JDK is necessary to run Spring Boot applications.

   - **Install JDK**:  
     Download and install JDK 17 or higher from [Adoptium](https://adoptium.net/) or [Oracle](https://www.oracle.com/java/technologies/javase-jdk17-downloads.html).

   - **Verify installation**:
     ```sh
     java -version
     ```

4. **MySQL**  
   MySQL is required to store and manage your application data.

   - **Install MySQL**:  
     Download and install MySQL Community Server from the [official MySQL website](https://dev.mysql.com/downloads/mysql/).

   - **Verify installation**:
     ```sh
     mysql --version
     ```

5. **Maven or Gradle (depending on your build tool)**  
   Maven or Gradle is needed to build your Spring Boot project.

   - **Install Maven**:  
     Follow the installation guide at the [official Apache Maven website](https://maven.apache.org/install.html).

   - **Install Gradle**:  
     Follow the installation guide at the [official Gradle website](https://gradle.org/install/).

6. **Visual Studio Code (VS Code)**  
   VS Code is a recommended code editor for working with JavaScript, TypeScript, and React. It offers various extensions to enhance the development experience.

   - **Download and Install VS Code**:  
     Visit the [official Visual Studio Code website](https://code.visualstudio.com/).

   - **Recommended Extensions**:
     - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint): Helps maintain consistent code quality.
     - [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode): Automatically formats your code.
     - [JavaScript (ES6) code snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets): Adds code snippets for JavaScript and TypeScript.
     - [Spring Boot Extension Pack](https://marketplace.visualstudio.com/items?itemName=Pivotal.vscode-boot-dev-pack): Enhances the development of Spring Boot applications.
7. **IntelliJ IDEA**  
   IntelliJ IDEA is a robust IDE for Java and Spring Boot development, offering advanced features for code completion, refactoring, debugging, and version control integration.

   - **Download and Install IntelliJ IDEA**:  
     Visit the [official JetBrains website](https://www.jetbrains.com/idea/) to download and install IntelliJ IDEA. The Community edition is free and suitable for most Java and Spring Boot projects.

   - **Recommended Plugins**:
     - **Spring Boot**: Supports Spring Boot projects with easy configuration and management.
     - **Lombok**: Simplifies Java code with annotations, reducing boilerplate.
     - **Database Tools**: Provides powerful database management capabilities directly within IntelliJ IDEA.

8. **MySQL Workbench**  
   MySQL Workbench is a visual tool for database architects, developers, and DBAs. It provides data modeling, SQL development, and comprehensive administration tools for server configuration and user management.

   - **Download and Install MySQL Workbench**:  
     Visit the [official MySQL website](https://dev.mysql.com/downloads/workbench/) to download and install MySQL Workbench.

   - **Key Features for Development**:
     - **SQL Editor**: Execute SQL queries and scripts to interact with your MySQL database.
     - **Database Design**: Visually design, model, generate, and manage databases.
     - **Data Export and Import**: Easily export and import data to and from your MySQL database.


### Installation
To get a local copy up and running locally on your computer follow these steps:


1. Clone the repo
   ```sh
   git clone https://github.com/ItsKader/Book-Discovery-App.git

   ```
2. Directly in the front-end directory, create a `.env` file with the variable name **`REACT_APP_API_URL`**. This variable will store the base URL of your backend API, allowing your React application to make HTTP requests to the correct server. For local development, you can set it to `http://localhost:8080`, where your backend server will run by default:
     ```sh
   REACT_APP_API_URL=http://localhost:8080

   ```

   
3. Log into MySql Workbench and run the files in the scripts folder to create the database and tables for the application.
 

4. In the main back-end directory, create a `.env` file in which you set up configuration settings and credentials to connect with the database and front-end. This file should include the following environment variables:

- **`DATASOURCE_URL`**: Specifies the JDBC URL used to connect to your MySQL database. 

- **`DATASOURCE_USER`**: The username for your database connection. This user should have the necessary permissions to read from and write to the database.

- **`DATASOURCE_PASSWORD`**: The password associated with the `DATASOURCE_USER` for authenticating the database connection. Ensure this password is strong and secure.

- **`FRONTEND_URL`**: The URL where your React frontend application is running, typically set to `http://localhost:3000` during development.
  ```sh
   DATASOURCE_URL=jdbc:mysql://localhost:3306/mydatabase
   DATASOURCE_USER=myuser
   DATASOURCE_PASSWORD=mysecretpassword
   FRONTEND_URL=http://localhost:3000
   ```

5. Now The application can be started. First, run the back-end in IntelliJ. After that, start the front-end with the following command:
 ```sh
  npm install && npm run dev
   ```





<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- LICENSE -->

## License

Distributed under the MIT License.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->


[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[TypeScript.js]: https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white
[TypeScript-url]: https://www.typescriptlang.org/
[SpringBoot]: https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white
[SpringBoot-url]: https://spring.io/projects/spring-boot
[MySQL]: https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white
[MySQL-url]: https://www.mysql.com/
