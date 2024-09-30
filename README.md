# Stone-Canyon-Project

This is a home improvement chatbot application built with React for the frontend and Node.js/Express for the backend. The chatbot interacts with users to guide them through a decision-making process based on the services available in a CSV file. The application collects user details and generates a summary at the end.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Backend API Endpoints](#backend-api-endpoints)
- [CSV File Structure](#csv-file-structure)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Category Selection**: Users can select a category ID and name to filter available questions.
- **Question Funnel**: Users are guided through a series of questions based on their selections.
- **User Details Collection**: Collects user information such as name, email, phone number, zip code, and address.
- **Service ID Generation**: Provides a matching service ID based on user responses.
- **Talking Prompts**: Uses OpenAI's GPT-4 to generate conversational prompts for the chatbot.
- **Summary Display**: Displays a summary of user responses and the service ID at the end.

## Technologies Used

- **Frontend**: React, CSS
- **Backend**: Node.js, Express
- **Data Parsing**: PapaParse
- **OpenAI**: ChatGPT (GPT-4)
- **CSV Data**: Used for questions and answers

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/home-improvement-chatbot.git
