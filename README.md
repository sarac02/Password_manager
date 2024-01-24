# Password_manager

## Introduction <br>
This Python script serves as a simple password manager utilizing SQLite for data storage. Users can store and retrieve passwords for different services using a master password. The script employs SHA-256 hashing to enhance security.

## Prerequisites <br>
Python 3.x
SQLite3 module

## Setup <br>
Download the script (password_manager.py) to your local machine.
Ensure you have Python installed on your system.
Install the SQLite3 module by running:

pip install sqlite3

## Usage <br>
Run the script using the following command:
python password_manager.py

Enter the master password when prompted. If you want to quit the program, type 'q' and press Enter.
Once authenticated, the script will either create a new password manager database or use an existing one.

## Security <br>
The master password is hashed using SHA-256 for enhanced security.
Passwords for services are generated using a combination of the master password, service name, and a unique key. The result is a SHA-256 hash truncated to 15 characters.

## Database <br>
The script utilizes an SQLite database (pass_manager.db) with a single table (KEYS) to store the hashed keys for each service.
