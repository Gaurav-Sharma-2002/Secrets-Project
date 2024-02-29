# Secrets Project - Implementing Authentication & Security

Using hashing passwords, passport, local & google authentication strategy, google cloud console, sessions & cookies, environment variables . 

## Getting Started

To run this application, follow these steps:

1. **Download and Extract**
   - Download the source code from [this link](https://github.com/Gaurav-Sharma-2002/Secrets-Project/archive/refs/heads/main.zip).
   - Extract the downloaded file.
   - Open the extracted folder in your favorite code editor such as Visual Studio Code.

2. **Install Dependencies**
   - Open a terminal.
   - Navigate to the project folder using `cd`.
   - Run `npm install` to install all the required dependencies.

3. **Setup SQL Database**
   - Set up your SQL database ( I'm using PostgreSQL (version 15) and PgAdmin 4 ) .
```
CREATE TABLE users (
    id SERIAL PRIMARY KEY,
    email VARCHAR(100) UNIQUE NOT NULL,
    password VARCHAR(100),
    secret TEXT
);
```

4. **Replace Database Credentials**
    - Open the index.js file.
    - Replace the following database connection credentials with your own :
```
  user: process.env.PG_USER,
  host: process.env.PG_HOST,
  database: process.env.PG_DATABASE,
  password: process.env.PG_PASSWORD,
  port: process.env.PG_PORT,
```

5. **Run the Application**
   - In the terminal, run node index.js to start the application.


