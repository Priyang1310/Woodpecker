# Chat Interface with Database 

## Table of Contents
1. [Introduction](#introduction)
2. [Project Overview](#project-overview)
3. [Technologies Used](#technologies-used)
4. [System Architecture](#system-architecture)
5. [Features](#features)
6. [Installation](#installation)
7. [Usage](#usage)
8. [Endpoints](#endpoints)
9. [Model Training with Gemini-pro](#model-training-with-gemini-pro)
10. [Performance Evaluation](#performance-evaluation)
11. [Future Enhancements](#future-enhancements)

---

## Introduction
Welcome to the "Chat with Database" project. This repository contains the source code for a chat interface that allows users to interact with SQL and NoSQL databases through a user-friendly interface.

## Project Overview
The aim of this project is to develop a chat application where users can:
- Authenticate using Auth0.
- Chat with a bot to interact with databases.
- Manage their user profiles.
- Connect to either MySQL or MongoDB databases.
- Execute queries and get responses.
- Train a custom machine learning model using Gemini-pro based on user-selected tables.

## Technologies Used
- **Frontend**: React, Material-UI, Axios, React Router
- **Backend**: Flask, REST APIs
- **Authentication**: Auth0
- **Database**: MySQL, MongoDB
- **Machine Learning**: Gemini-pro

## System Architecture
The system architecture comprises:
- **Frontend**: Built using React and Material-UI.
- **Backend**: A Flask server for handling API requests and responses.
- **Databases**: MySQL for SQL support and MongoDB for NoSQL support.
- **Authentication**: Managed by Auth0.
- **Machine Learning**: Gemini-pro for training models and generating responses.

## Features
- **Landing Page**: Displays a welcoming message and an option to sign in.
- **Authentication**: Uses Auth0 for user login.
- **Chat Interface**: Allows users to chat and interact with the application.
- **User Profile Management**: Users can view and edit their profile information.
- **Database Connectivity**: Supports connections to MySQL and MongoDB databases.
- **Model Training**: Trains a custom machine learning model using Gemini-pro.

## Installation
1. **Clone the repository:**
    ```sh
    git clone https://github.com/Priyang1310/Woodpecker.git
    ```

2. **Install dependencies:**
    ```sh
    # For the frontend
    cd client
    npm install

    # For the backend
    cd ../server
    pip install -r requirements.txt
    ```

3. **Set up environment variables:**
    - Create a `.env` file in the `backend` directory and add your environment variables for Auth0, database connections, etc.

4. **Run the application:**
    ```sh
    # Start the frontend
    cd client
    npm run dev

    # Start the backend
    cd ../server
    python app.py
    ```

## Usage
1. **Landing Page**: Navigate to the landing page and click on "Sign In".
2. **Authentication**: Log in using Auth0.
3. **Chat Interface**: Interact with the chat interface to send queries to the database.
4. **Profile Management**: Click on the profile button to view and edit profile information.
5. **Database Connection**: Choose between MySQL and MongoDB for database operations.
6. **Query Execution**: Execute queries and receive responses.
7. **Model Training**: Train the machine learning model with Gemini-pro.

## Endpoints

### Profile Management

### Mongodb Connection
- **/connect**: Establish the connection with mongodb database and the response will return the collections of that database.

### MySQL Connection
- **/mysql/connect**: Establish the connection with mySQL database and the response will return the tables of that database.

### Training Agent
- **/collections**: For training the agent on a specific collection for the mongodb database.
- **/mysql/tables**: For training the agent on a specific collection for the MySQL database.

### NoSQL Queries
- **/ask**: Executes NoSQL queries against the MongoDB database.

### SQL Queries
- **/aski**: Executes SQL queries against the MySQL database.

## Model Training with Gemini-pro
- **Data Preparation**: Extracts data from user-selected tables.
- **Model Training**: Trains the Gemini-pro model with the prepared data.
- **Model Integration**: Integrates the trained model into the Flask server for processing queries.

## Performance Evaluation
- **Response Time**: Measures the time taken to process and respond to user queries.
- **Accuracy**: Assesses the precision of responses generated by the trained model.
- **Scalability**: Evaluates the system's ability to handle multiple users and large datasets simultaneously.

## Future Enhancements
- **Additional Database Support**: Integrate support for other databases like PostgreSQL or Cassandra.
- **Advanced Analytics**: Add features for advanced data analytics and reporting.
- **Improved UI/UX**: Enhance the user interface with more customization options and interactive elements.
- **Real-time Collaboration**: Enable real-time collaboration features for multiple users.

## Screenshots

### Landing Page
![Landing Page](https://github.com/Priyang1310/Woodpecker/blob/main/client/public/Screen_shots/Landing-page.png)

### Authentication
![Authentication](https://github.com/Priyang1310/Woodpecker/blob/main/client/public/Screen_shots/Auth0.png)

### Chat Interface
![Chat Interface](https://github.com/Priyang1310/Woodpecker/blob/main/client/public/Screen_shots/Chat_Interface.png)

### Profile Management
![Profile Management](https://github.com/Priyang1310/Woodpecker/blob/main/client/public/Screen_shots/User_Profile.png)

### Query Execution 
![SQL Query Execution](https://github.com/Priyang1310/Woodpecker/blob/main/client/public/Screen_shots/Query.png)

### Query Execution in Light Theme
![SQL Query Execution](https://github.com/Priyang1310/Woodpecker/blob/main/client/public/Screen_shots/White_Theme.png)

