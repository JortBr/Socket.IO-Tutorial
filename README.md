# Socket.IO-Tutorial

Socket.IO tutorial for my personal project fps game to get a look at how this works and how I can implement this into my own game.

🚀 How to Run This Project
- Press the green Code button on this GitHub repository.
- Click the copy icon next to the HTTPS URL.
- Open CMD or Terminal and navigate to the directory where you want to clone the project:
  - cd path/to/your/folder
- Clone the repository using the copied URL:
  - git clone https://github.com/your-username/your-repo-name.git
- Open the project folder in your development environment (e.g., Visual Studio Code).
- Make sure you have Node.js installed. You can check with:
  - node -v
  - npm -v
- Open up the terminal
- Install the required dependencies:
  - npm install
  - npm install express
  - npm install socket.io
  - npm install sqlite3
  - npm install sqlite
- Start the development server using node:
  - node server.js

- serverOffset is used to remember the last received ID (for restoring the connection status):
<img width="454" src="https://github.com/user-attachments/assets/eedc12ef-10b1-453c-84ad-2df86223de5e">

- socket.emit() – sends the event chat message containing the message to the server.
<img width="454" src="https://github.com/user-attachments/assets/2288d9c1-8c7e-4ab6-8cc5-acd1d04a538e">

- As soon as the event chat message is fired, it returns the message from the server and shows it in the list
- serverOffset is updated for state recovery:
<img width="454" src="https://github.com/user-attachments/assets/0d06df1b-953f-4393-bcb0-78eb8fad9805">

- Creates or opens the database file:
<img width="454" src="https://github.com/user-attachments/assets/93e5d0e6-2b38-4c71-ae5d-39e158e4903d">

- Creates the table for storing messages:
<img width="454" src="https://github.com/user-attachments/assets/fa68db05-377a-49df-bc4f-76241f7a6ae1">

- Stores messages in the database.
- Sends the message to all connected clients:
<img width="454" src="https://github.com/user-attachments/assets/14555074-8ed9-4882-bd77-5dac5daba690">

- If the connection is lost, missed messages are still retrieved from the database:
<img width="454" src="https://github.com/user-attachments/assets/ce9831d0-0b59-4ee1-b6b5-87139ce20094">

Results:
 
<img width="600" src="https://github.com/user-attachments/assets/40f5c78d-3b76-413e-a7a4-dd358ed82afa">


<img width="600" src="https://github.com/user-attachments/assets/f96bcd57-ab05-4b1e-b09d-5c9ff54d8c9a">

https://socket.io/docs/v4/tutorial/step-7
