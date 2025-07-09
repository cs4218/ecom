# CS4218 Project - Virtual Vault

## 1. Project Introduction

Virtual Vault is a full-stack MERN (MongoDB, Express.js, React.js, Node.js) e-commerce website, offering seamless connectivity and user-friendly features. The platform provides a robust framework for online shopping. The website is designed to adapt to evolving business needs and can be efficiently extended.

## 2. Website Features

- **User Authentication**: Secure user authentication system implemented to manage user accounts and sessions.  
- **Payment Gateway Integration**: Seamless integration with popular payment gateways for secure and reliable online transactions.  
- **Search and Filters**: Advanced search functionality and filters to help users easily find products based on their preferences.  
- **Product Set**: Organized product sets for efficient navigation and browsing through various categories and collections.  

## 3. Your Task

- **Unit and Integration Testing**: Utilize Jest for writing and running tests to ensure individual components and functions work as expected, finding and fixing bugs in the process.  
- **UI Testing**: Utilize Playwright for UI testing to validate the behavior and appearance of the website's user interface.  
- **Code Analysis and Coverage**: Utilize SonarQube for static code analysis and coverage reports to maintain code quality and identify potential issues.  
- **Load Testing**: Leverage JMeter for load testing to assess the performance and scalability of the ecommerce platform under various traffic conditions.  

## 4. Setting Up the Existing Project

### a. Installing Node.js

1. **Download and Install Node.js**:  
   - Visit [nodejs.org](https://nodejs.org) to download and install Node.js.  

2. **Verify Installation**:  
   - Open your terminal and check the installed versions of Node.js and npm:  
     ```bash
     node -v  
     npm -v  
     ```

### b. MongoDB Setup

Follow these steps to set up MongoDB for your project:

1. **Download MongoDB Compass**:  
   - Download MongoDB Compass for your operating system from the official MongoDB website.  
   - Sign up or log in to MongoDB Atlas.  

2. **Create a New Shared Cluster**:  
   - After logging in, create a new shared cluster and name it accordingly.  

3. **Configure Database Access**:  
   - Navigate to "Database Access" under "Security" and create a new user with appropriate permissions.  

4. **Whitelist IP Address**:  
   - Go to "Network Access" and whitelist your IP address (e.g., 0.0.0.0) to allow access from your machine.  

5. **Connect to the Database**:  
   - Click on "Connect" and choose "Connect with MongoDB Compass".  
   - Copy the connection string and copy and save it to be added later to project environment  

6. **Establish Connection with MongoDB Compass**:  
   - Open MongoDB Compass, paste the connection string, and establish a connection to your cluster.  

### c. Downloading and Using a MERN App from GitHub

To download and use the MERN (MongoDB, Express.js, React.js, Node.js) app from GitHub, follow these general steps:

1. **Clone the Repository**  
   - Go to the GitHub repository of the MERN app. (GitHub - cs4218/ecom)  
   - Click on the "Code" button and copy the URL of the repository.  
   - Open your terminal or command prompt.  
   - Use the `git clone` command followed by the repository URL to clone the repository to your local machine:  
     ```bash
     git clone <repository_url>
     ```  
   - Navigate into the cloned directory.  

2. **Add database connection string to .env**  
   - Add the connection string copied from MongoDB Atlas to the `.env` file inside the project directory:  
     ```env
     MONGO_URL = <connection string>
     ```

3. **Install Dependencies**  
   - Navigate into the root directory (where `package.json` file for the backend is located).  
   - Run `npm install` to install backend dependencies.  
   - Navigate into the `client` directory (where `package.json` file for the frontend is located).  
   - Run `npm install` to install frontend dependencies.  

4. **Set Up Environment Variables**  
   - Check if there are any environment variables required for the app (e.g., database connection URI).  
   - Create a `.env` file in the backend directory and set the required environment variables.  

5. **Adding Sample data to database**  
   - Download “Sample DB Schema” from Canvas  
   - In MongoDB Compass, inside the cluster create `test` database.  
   - Load the Sample data inside test database.  

6. **Running the Application**  
   - Open your web browser.  
   - Use `npm run dev` to run the app from root directory, which starts the development server.  
   - Navigate to `http://localhost:3000` to access the application.  

## 5. Unit Testing with Jest

Unit testing is a crucial aspect of software development aimed at verifying the functionality of individual units or components of a software application. It involves isolating these units and subjecting them to various test scenarios to ensure their correctness.  
Jest is a popular JavaScript testing framework widely used for unit testing. It offers a simple and efficient way to write and execute tests in JavaScript projects.

### Getting Started with Jest

To begin unit testing with Jest in your project, follow these steps:

1. **Install Jest**:  
   Use your preferred package manager to install Jest. For instance, with npm:  
   ```bash
   npm install --save-dev jest

2. **Write Tests**  
   Create test files for your components or units where you define test cases to evaluate their behaviour.

3. **Run Tests**  
   Execute your tests using Jest to ensure that your components meet the expected behaviour.  
   You can run the tests by using the following command in the root of the directory:

   - **Frontend tests**  
     ```bash
     npm run test:frontend
     ```

   - **Backend tests**  
     ```bash
     npm run test:backend
     ```

   - **All the tests**  
     ```bash
     npm run test
     ```
