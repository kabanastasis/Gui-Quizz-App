# Python Quiz Game

A graphical True/False quiz game built with **Python** and **Tkinter**.

The application retrieves trivia questions dynamically from the **Open Trivia Database API** and uses Object-Oriented Programming to separate the user interface, quiz logic, question model, and API data handling.

## Features

* Interactive GUI built with Tkinter
* Trivia questions retrieved from the Open Trivia Database API
* True/False question format
* Automatic progression through questions
* Real-time score tracking
* Immediate answer checking
* Object-Oriented Programming structure
* API requests and JSON data handling

### `data.py`

Handles communication with the **Open Trivia Database API** using the `requests` package.

It sends the API request, receives the trivia questions, and makes the question data available to the rest of the application.

### `questionmodel.py`

Defines the question model.

Each question object stores:

* The question text
* The correct answer

This provides a simple structure for representing each quiz question.

### `quizbrain.py`

Contains the main quiz logic.

It is responsible for:

* Keeping track of the current question
* Providing the next question
* Checking whether the user's answer is correct
* Updating the score
* Determining when the quiz has finished

### `ui.py`

Contains the graphical user interface built with **Tkinter**.

It displays:

* The current question
* The user's score
* True and False buttons
* Feedback after each answer

The UI communicates with the quiz logic to retrieve questions and validate the user's answers.

### `main.py`

Acts as the entry point of the application.

It connects the different parts of the project together by:

1. Retrieving the question data
2. Creating question objects
3. Creating the quiz logic
4. Creating the Tkinter user interface
5. Starting the application

## How It Works

1. `data.py` retrieves questions from the Open Trivia Database API.
2. The returned JSON data is processed.
3. `question_model.py` is used to create question objects containing the question text and answer.
4. The question objects are passed to `quizbrain.py`.
5. `quizbrain.py` manages the question sequence, score, and answer checking.
6. `ui.py` displays the quiz through a Tkinter graphical interface.
7. `main.py` connects all components and starts the program.

## API

The application uses the **Open Trivia Database (OpenTDB)** to retrieve quiz questions dynamically.

This means the questions do not need to be stored manually inside the project and can change whenever the application is run.

## Concepts Practiced

This project demonstrates:

* Object-Oriented Programming
* Python classes and objects
* Separation of responsibilities across multiple modules
* Building graphical applications with Tkinter
* Event-driven programming
* Working with REST APIs
* Sending HTTP requests
* Processing JSON responses
* Application logic and state management

## Future Improvements

Possible future improvements include:

* Category selection
* Number-of-questions selection
* Restart button
* High-score tracking
* Improved UI design

## Author

**Anastasis Kabiotis**

