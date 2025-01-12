# History Agent (RAG)

# User Interface

<img width="410" alt="Screen Shot 2024-10-23 at 11 59 57 PM" src="https://github.com/user-attachments/assets/46b29a95-6917-411e-995e-e9bbbaeb64fa"> <img width="410" alt="Screen Shot 2024-10-24 at 12 00 26 AM" src="https://github.com/user-attachments/assets/873fe316-467f-415b-8228-4bd90164c1c2">
<img width="410" alt="Screen Shot 2024-10-24 at 12 01 02 AM" src="https://github.com/user-attachments/assets/9a61664a-3c9b-47ae-b8b2-8a301a027879"> <img width="410" alt="Screen Shot 2024-10-24 at 12 01 43 AM" src="https://github.com/user-attachments/assets/34693d21-9873-4996-ae51-b50ed1d1f94f">
<img width="1280" alt="Screen Shot 2024-10-24 at 12 05 42 AM" src="https://github.com/user-attachments/assets/78474afa-5009-4b75-b1dd-3ade2e29d6d4">

# Project Overview

The History Agent project is a full-stack web application designed as an expert chat engine for historical inquiries. Leveraging the principles of Retrieval-Augmented Generation (RAG), this application utilizes the advanced Llama 3 language model to deliver evidence-based responses to historical questions.

The tech stack consists of MongoDB, Flask, React, Python, and PineCone. The project harnesses the following technologies:

* MongoDB: NoSQL database that stores data in a flexible, JSON-like format, allowing for scalable data storage and efficient querying of complex data structures.
* Flask: Serves as the backend framework, providing robust integration capabilities and handling API requests efficiently.
* React: Provides robust framework for the frontend user interface, delivering a responsive and engaging experience for users.
* Python: Acts as the runtime environment for the Flask backend, executing server-side logic and managing asynchronous operations.
* Pinecone: Manages the vector database, enabling efficient storage and retrieval of embeddings for enhanced query responses.

# Purpose
This comprehensive architecture ensures that the History Agent delivers accurate and contextually relevant answers, positioning it as a valuable resource for history enthusiasts, researchers, and students alike. By leveraging the capabilities of the Llama 3 language model and Retrieval-Augmented Generation, the application not only provides reliable information but also serves as an effective and efficient learning tool. It enhances users' understanding of historical concepts and events, fostering a more streamlined learning experience.


# Project Functionalities

1. **Historical Question-Answering**: Provides accurate, evidence-based answers to historical inquiries using the Llama 3 language model and Retrieval-Augmented Generation (RAG).
2. **User-Friendly Interface**: Features an intuitive and engaging frontend built with React, ensuring ease of use and real-time interaction.
3. **Optimized Model Performance**: Trained with the most efficient hyperparameters to deliver the most accurate possible answers, enhancing the overall learning experience.
4. **Previous Chat History Management**: Provides accessibility to previous chat messages for analysis and management of data, optimizing learning efficieny.
5. **Efficient Learning Tool**: Supports students and researchers by facilitating efficient study habits and deeper engagement with historical content.
6. **Seamless Integration**: Utilizes CORS for smooth interaction between frontend and backend, built on the scalable FRAP stack (Flask, React, API, Pinecone).
7. **Vector Data Management**: Utilizes Pinecone for efficient storage and retrieval of vector embeddings, enhancing query performance.



# Repository Structure

* Options: Instructions for running option 1 and option 2 (SEE BELOW FOR MORE INFO)
* Test Data: Comprises of 2 documents (Amendments of U.S.) and is used for quick testing without pinecone account creation (READ BELOW FOR MORE INFORMATION)
* Data: Includes initial 2 documents (Amendments of U.S.) and will be used to store openly available history text data
* rag-history: Contains React application with CSS components, and stores Flask framework with Python, integrated with Pinecone, and MongoDB.


# Getting Started

There are 2 simulations offered for this project:

Select one of the options for testing the project, and follow the instructions after for intial setup as they are required for either option.

[Option 1](Options/Option_1_README.md). Run complete RAG application for history

   * (Longer runtime, application performs the full functionalties for History Agent)
   * Uses vector database and requires Pinecone account creation for API key
   * Uses MongoDB on AWS cloud, requires MongoDB account creation for driver connection
   * You will need to download free history text data from available websites

[Option 2](Options/Option_2_README.md). Run test RAG application using only 2 documents (Amendments of U.S.) as data
    
   * (Faster, used for quick testing of application and doesn't require Pinecone or MongoDB account creation)
   * Application can answer questions about U.S. Amendments)
   * No need to download external history text data


**Initial Setup**

To run this full stack project, you will need to run both the frontend and backend portions of the application. Each respective part and their detailed instructions for setup, configurations, and deployment are described below.

For this project you will need **Python version 3.11.10**

You will also need **Ollama** to run the local LLM model

Download https://ollama.com/

It is best to create a virtual environment to manage the required dependencies and framework versions for this project. To initialize and set up a virtual environment, first clone this repository to your local development environment.

    git clone <repository-url>

**Create a Virtual Environmet**

    python3 -m venv venv


**Activate the Virtual Environment**

* MacOS/Linux:

      source venv/bin/activate

* Windows:

      venv\Scripts\activate

**Install Dependencies (backend)**

      pip install -r requirements.txt

**Navigate to rag-history directory**

      cd rag-history

**Install Node Modules, Axios, and Fontawesome (Frontend)**

      npm install @fortawesome/react-fontawesome @fortawesome/free-solid-svg-icons

      
Please follow the above instructions and select an option ([Option 1](Options/Option_1_README.md)) or ([Option 2](Options/Option_2_README.md)) to simulate the application on your local deployment environemnt.

