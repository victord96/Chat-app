# Chat Room

A simple Django app that allows users to create and participate in chat rooms.

## Installation

1. Clone the repository:

git clone https://github.com/<your-username>/chat-room.git

Copy code

2. Navigate to the project directory:

cd chat-room

Copy code

3. Install the required packages:

pip install -r requirements.txt

Copy code

4. Run the migrations to set up the database:

python manage.py migrate

Copy code

5. Run the development server:

python manage.py runserver

Copy code

6. Open a browser and go to http://127.0.0.1:8000 to view the app.

## Usage

1. On the home page, enter a room name and a username, and click "Enter Room". If the room does not exist, it will be created.

2. You will be redirected to the chat room page. Type a message in the input field and click "Send" to send it to the chat room.

3. All messages for the chat room will be displayed in the chat window.

## Files

- `urls.py` defines the URLs for the project and the corresponding view functions in the `views.py` file.

- `views.py` contains the view functions for the app. These include:

  - `home`, which renders the home page.
  - `checkview`, which checks if a room with the specified name exists and creates it if it does not.
  - `room`, which renders the chat room page.
  - `send`, which handles sending messages to a chat room.
  - `getMessages`, which retrieves and returns a list of messages for a given chat room.

## Requirements

- Python 3.x
- Django 2.x

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.