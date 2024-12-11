# Phonebook Actor

A simple Motoko-based actor for managing a phonebook and sending messages on the Internet Computer.

## Features

- **Phonebook Management**:
  - Add contacts with name, description, and phone number.
  - Retrieve contact details by name.

- **Messaging**:
  - Send messages to specific phone numbers.
  - View the history of messages sent from a phone number.

## Methods

- `insert(name: Name, entry: Entry): async ()`
  - Adds a new contact to the phonebook.

- `getPhone(name: Name): async ?Entry`
  - Retrieves contact details by name.

- `sendMessage(senderPhone: Phone, message: Message): async ()`
  - Sends a message and stores it in the history.

- `sentMessages(senderPhone: Phone): async ?Message`
  - Fetches messages sent from a given phone number.

## Usage

Include this actor in your Internet Computer project to manage contacts and messages.
