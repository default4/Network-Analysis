# Kafka-ML Diabetes Classification Project

This project demonstrates a real-time data processing and machine learning application using Apache Kafka, FastAPI, and a diabetes classification model. It is designed to consume streaming data, apply a machine learning model for diabetes prediction, and expose results through a FastAPI interface.

## Prerequisites

- Python 3.x
- Apache Kafka
- Docker (optional, for Docker Compose)
- Libraries: FastAPI, Kafka-Python, Pandas, Scikit-learn 

## Installation and Setup

1. **Kafka Setup:**
   - Install and configure Apache Kafka.
   - Create necessary Kafka topics (replace `<topic_name>` with your topic):
     ```bash
     kafka-topics --create --topic <topic_name> --bootstrap-server localhost:9092
     ```

2. **Python Environment:**
   - Set up a Python virtual environment and install the required packages:
     ```bash
     python -m venv venv
     source venv/bin/activate
     pip install -r requirements.txt
     ```

3. **Docker Compose (Optional):**
   - Use `docker-compose.yaml` to set up the environment (if applicable).

## Configuration

- Configure environment variables in `database.env`.
- Adjust Kafka and FastAPI settings in respective scripts as necessary.

## Running the Application

1. **Start Kafka Producers:**
   ```bash
   python producer-diabets.py
   python producer-example.py
   ```

2. **Start Kafka Consumers:**
  ```bash
  python consumer-diabets.py
  python consumer-example.py
  ```

3. **Run FastAPI Application:**
  ```bash
  uvicorn fastapi_app:app --reload
  ```

4. **Use the Machine Learning Model:**
  1. The Jupyter notebook diabet-classification.ipynb contains the model training process.
  2. The trained model is saved as model.pkl, used by the consumers for real-time predictions.

## Usage Examples

1. Send requests to FastAPI to get diabetes predictions.
2. Kafka producers send data, and consumers process and use the ML model to predict diabetes based on the data.

## Project Structure

* producer-diabets.py: Kafka producer script for diabetes data.
* consumer-diabets.py: Kafka consumer script that uses ML model for predictions.
* fastapi_app.py: FastAPI application to expose prediction results.
* data_request_model.py: Defines data models for FastAPI.
* diabet-classification.ipynb: Jupyter notebook for ML model training.
* model.pkl: Serialized ML model for diabetes prediction.
* docker-compose.yaml: Docker compose file for environment setup.
* database.env: Environment variables for database configuration.