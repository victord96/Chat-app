Chat Room
A simple Django app that allows users to create and participate in chat rooms.

Installation
Clone the repository:
Copy code
git clone https://github.com/<your-username>/chat-room.git
Navigate to the project directory:
Copy code
cd chat-room
Install the required packages:
Copy code
pip install -r requirements.txt
Run the migrations to set up the database:
Copy code
python manage.py migrate
Run the development server:
Copy code
python manage.py runserver
Open a browser and go to http://127.0.0.1:8000 to view the app.
Usage
On the home page, enter a room name and a username, and click "Enter Room". If the room does not exist, it will be created.

You will be redirected to the chat room page. Type a message in the input field and click "Send" to send it to the chat room.

All messages for the chat room will be displayed in the chat window.

Files
urls.py defines the URLs for the project and the corresponding view functions in the views.py file.

views.py contains the view functions for the app. These include:

home, which renders the home page.
checkview, which checks if a room with the specified name exists and creates it if it does not.
room, which renders the chat room page.
send, which handles sending messages to a chat room.
getMessages, which retrieves and returns a list of messages for a given chat room.
Requirements
Python 3.x
Django 2.x
License
This project is licensed under the MIT License - see the LICENSE file for details.