# CloudBlood: AI-Powered Smart Blood Bank System
 CloudBlood is a cloud-based intelligent blood bank system that integrates an AI-powered chatbot, a dynamic web application, and a serverless data querying system. This platform enables users to find blood donors, check availability, and analyze donation trends using AWS cloud services.

## Features
- AI Chatbot – Answers user queries and collects donor information.
- Dynamic Web Application – Manages donor/recipient requests with real-time updates.
- Serverless Data Querying.
- Uses AWS Athena, Glue, and S3 to analyze blood donation trends.
- Cloud Deployment – Hosted on AWS (EC2, S3, Lambda, DynamoDB, and QuickSight).

## Tech Stack
**Backend:** Python (Flask/Django), AWS Lambda
**Frontend:** HTML, CSS, JavaScript (React optional)
**Chatbot:** NLTK, spaCy, scikit-learn
**Database:** AWS DynamoDB / PostgreSQL
**Cloud Services:** AWS EC2, S3, Athena, Glue, QuickSight

## Installation & Setup
1️. Clone the Repository
``` bash

git clone https://github.com/yourusername/CloudBlood.git
cd CloudBlood
```
2️. Create a Virtual Environment & Install Dependencies
```bash

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```
3️. Set Up Environment Variables
Create a .env file in the project root and add your AWS credentials:

```ini

AWS_ACCESS_KEY=your_access_key
AWS_SECRET_KEY=your_secret_key
DB_URI=your_database_uri
```
4️. Run the Application
```bash

python app.py
or for Flask:
```

```bash

flask run
The app will be available at http://127.0.0.1:5000/.
```
## Deploying on AWS
1️. Deploying the Web App on EC2
-Launch an EC2 instance and install Python, Flask/Django.
-Clone the repository and run the app.

2️. Deploying the Chatbot on AWS Lambda
-Package the chatbot script and deploy it as a Lambda function.
-Use API Gateway to expose it as an endpoint.

3️. Setting Up Serverless Data Querying
-Upload blood donation records to AWS S3.
-Use AWS Glue to clean and prepare data.
-Run SQL queries on AWS Athena.
-Use AWS QuickSight to visualize trends.
