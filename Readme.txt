
Sentiment Analysis Flask App

This project is a Flask-based web application that deploys a Sentiment Analysis model using Naïve Bayes (NB) and Support Vector Machine (SVM). The application is containerized using Docker.

Prerequisites

Ensure you have the following installed:

Docker

Git

Installation & Setup

Clone the Repository

git clone https://github.com/yourusername/yourrepo.git
cd yourrepo

Build the Docker Image

Use the following command to build the Docker image:

docker build --no-cache -t sentiment-analysis .

Run the Docker Container

Start the Flask app by running the container:

docker run -p 5000:5000 sentiment-analysis

Access the Web Application

Once the container is running, open your browser and go to:

http://localhost:5000

Project Structure

📦 yourrepo
 ┣ 📂 templates
 ┃ ┣ 📜 index.html  # Frontend template
 ┣ 📜 app2.py  # Flask application
 ┣ 📜 Dockerfile  # Docker build instructions
 ┣ 📜 naive_bayes_model.pkl  # Naïve Bayes pre-trained model
 ┣ 📜 svm_model.pkl  # Support Vector Machine model
 ┣ 📜 vectorizer.pkl  # Text vectorizer model
 ┣ 📜 requirements.txt  # Python dependencies
 ┣ 📜 Readme.txt  # Additional documentation
 ┣ 📜 README.md  # Project documentation

Docker Hub (Optional)

If you want to push your image to Docker Hub:

docker tag sentiment-analysis your-dockerhub-username/sentiment-analysis:latest

docker push your-dockerhub-username/sentiment-analysis:latest

Users can then pull the image using:

docker pull your-dockerhub-username/sentiment-analysis:latest

License

This project is licensed under the MIT License.

Author

Created by  Rodrigo Velazquez