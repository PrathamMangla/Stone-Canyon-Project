# Stone-Canyon-Project

This is a home improvement chatbot application built with React for the frontend and Node.js/Express for the backend. The chatbot interacts with users to guide them through a decision-making process based on the services available in a CSV file. The application collects user details and generates a summary at the end.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)

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

2. Navigate to the frontend directory and install dependencies:
   cd home-improvement-chatbot/frontend
   npm install

3. Navigate to the backend directory and install dependencies:
   cd ../backend
   npm install
   
4. Make sure to replace the OpenAI API key in server.js with your actual API key.

5. Start the backend server:
   node server.js
   
6. Start the frontend application:
   cd ../frontend
   npm start
   
## Usage

1. **Select Category ID**: The chatbot will first ask you to select a Category ID based on the CSV data.
2. **Select Category Name**: Once you choose the Category ID, select the Category Name.
3. **Answer Questions**: The chatbot will then ask questions based on your selected Category, and it will show options for you to choose from.
4. **User Details**: After answering all the questions, you will be prompted to enter your details (Name, Email, Phone, etc.).
5. **Get Service ID**: Once the details are entered, the chatbot will provide a unique Service ID based on your responses.
6. **Summary**: The chatbot will display a summary of your answers and user details.

## Dependencies

### Frontend

- **React**
- **Papaparse** (for CSV parsing)

Install these by running the following command in the `frontend/` directory: npm install

### Backend

- **Express**
- **OpenAI**
- **Papaparse**
- **Cors**
- **Body-parser**

Install these by running the following command in the `backend/` directory: npm install

# Chatbot for Home Improvement Services

This project is a chatbot application designed to assist users in selecting home improvement services. It guides users through a series of questions based on a CSV file containing service categories and questions, and then provides a unique Service ID based on the user's responses. The chatbot also collects user details and displays a summary of the interaction before final submission.

## Approach

### Frontend
- **React**: The frontend was built using React to provide an interactive user experience. React components were used to create the decision-tree-like interface for service selection and input forms.
- **Papaparse**: Used to parse the CSV file that contains service categories and corresponding questions. The data is then used to dynamically generate questions and options for the user.

### Backend
- **Express**: The backend API is built using Express.js, providing routes to handle user responses, fetch CSV data, and generate the Service ID.
- **OpenAI**: Integrated for any dynamic conversational aspects (if required).
- **Papaparse**: Also used in the backend to parse the CSV file for processing responses.
- **Cors**: Enables Cross-Origin Resource Sharing to allow the frontend and backend to communicate effectively.
- **Body-parser**: Parses incoming JSON data from frontend requests.

### User Flow
1. **Select Category ID**: The chatbot prompts the user to select a Category ID from the CSV data.
2. **Select Category Name**: Based on the Category ID, the user selects the Category Name.
3. **Answer Questions**: The chatbot displays questions associated with the selected category and provides multiple-choice options.
4. **User Details**: After answering the questions, the user is prompted to enter personal details such as name, email, and phone number.
5. **Get Service ID**: A unique Service ID is generated based on the user's responses.
6. **Summary**: A summary of the user's responses and details is displayed for confirmation before submission.

## Challenges Faced

1. **CSV Parsing**: Ensuring that the CSV data is properly parsed on both the frontend and backend required careful handling of file formats and structure. We had to normalize the data to make it easier to use in a conversational flow.

2. **Dynamic Question Flow**: Implementing a flexible decision-tree-like approach based on user selections and dynamically rendering questions from the CSV file was a challenge.

3. **Frontend and Backend Communication**: Ensuring smooth communication between the React frontend and the Express backend required proper configuration of CORS and consistent API design.

## Testing

The solution was tested locally using the following methods:

1. **Manual Testing**: The chatbot was run in a local development environment, and various service categories were selected to ensure the correct flow of questions and answers.

2. **CSV Validation**: The CSV data was verified to ensure correct parsing and display in the frontend.

3. **Backend Testing**: API routes were tested using Postman to verify the correct processing of responses and generation of Service IDs.




