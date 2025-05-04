# Sentiment Analysis Web App
This is a full-stack application that uses FastAPI for the backend and Streamlit for the frontend to perform sentiment analysis on user-input text. The backend connects to a Hugging Face Inference API to analyze sentiment in real time.

## How to Run the App
Build and start the services using Docker Compose:

bash
Copier
Modifier
docker-compose up --build
This command will start two services:

frontend – The Streamlit user interface.

backend – A FastAPI service that communicates with the Hugging Face inference API to get sentiment predictions.

Once running, open your browser and go to http://localhost:8501 to use the app.

## How to Use the App
Enter a sentence or paragraph into the text box.

Click the "Analyze Sentiment" button.

The app will send your input to the FastAPI backend, which in turn calls the Hugging Face Inference API.

The predicted sentiment (e.g., positive, negative, or neutral) will be displayed on the screen.

## Notes
The FastAPI backend runs on http://localhost:8000.

It acts as a middleware between the frontend and the Hugging Face model endpoint.

You can modify the model being used by updating the Hugging Face API call in the backend code.
