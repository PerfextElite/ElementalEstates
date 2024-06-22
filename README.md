### Project Setup Instructions

To run this project, follow these steps:

1. Clone the repository `full-stack-estate-main` to your local device and open it in VS Code.

2. Inside the `full-stack-estate-main` folder, you will find three folders:
   - `api`
   - `client`
   - `socket`

3. Install the dependencies for each folder:

   - **API Folder:**
     ```
     cd api
     npm i
     ```

   - **Client Folder:**
     Open another terminal and navigate to the `client` folder:
     ```
     cd client
     npm i
     ```

   - **Socket Folder:**
     Open another terminal and navigate to the `socket` folder:
     ```
     cd socket
     npm i
     ```

4. Ensure all dependencies are correctly installed on your local device.

5. In the `api` folder, create a new file named `.env` and add the following content:
   ```
   # Environment variables declared in this file are automatically made available to Prisma.
   # See the documentation for more detail: https://pris.ly/d/prisma-schema#accessing-environment-variables-from-the-schema

   # Prisma supports the native connection string format for PostgreSQL, MySQL, SQLite, SQL Server, MongoDB, and CockroachDB.
   # See the documentation for all the connection string options: https://pris.ly/d/connection-strings

   DATABASE_URL="mongodb+srv://admin:OQMQACfF1IFdDVdG@cluster7.yuqrtrc.mongodb.net/estate?retryWrites=true&w=majority&appName=Cluster7" # Add your MongoDB connection string
   JWT_SECRET_KEY="Xt6kT99JZDeih7pxA9QKBD4Oar8CF/vIMRy1X6F3gGo=" # Create your own key
   CLIENT_URL="http://localhost:5173" # This can stay the same
   ```

6. After setting up the `.env` file, open the terminal again and run:
   ```
   npx prisma db push
   ```

### Running the Project

- **To run the backend:**
  Open the terminal, navigate to the `api` folder, and enter:
  ```
  nodemon app.js
  ```

- **To run the frontend:**
  Open the terminal, navigate to the `client` folder, and enter:
  ```
  npm run dev
  ```

Following these steps should make the whole project functional.

