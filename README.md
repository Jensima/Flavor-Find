1. Install Python Dependencies
To begin, you'll need to set up a Python environment and install the required libraries. If you're using virtualenv (recommended), follow these steps:

Step 1: Set up a Virtual Environment (Optional)

If you don't have virtualenv installed, you can install it with:
pip install virtualenv
Create a virtual environment:
virtualenv venv
Activate the virtual environment:
Windows:
venv\Scripts\activate
macOS/Linux:
source venv/bin/activate
Step 2: Install Dependencies

Install the required libraries from the requirements.txt file.

Create a requirements.txt file with the following content:
streamlit
pymongo
spacy
requests
pandas
scikit-learn
Install all the dependencies:
pip install -r requirements.txt
Step 3: Install the SpaCy Model

Run the following command to install the en_core_web_md SpaCy model:

python -m spacy download en_core_web_md
2. MongoDB Setup
Option 1: Install MongoDB Locally
Download and install MongoDB from the official MongoDB website: MongoDB Download Center.
After installation, start the MongoDB server by running:
mongod
Option 2: Use MongoDB Atlas (Cloud Database)
If you prefer using a cloud database, sign up for MongoDB Atlas and create a cluster.
Obtain the connection string (you'll need it for pymongo).
3. Edamam API Setup
Sign Up for the Edamam API:
Go to the Edamam API site and create an account.
Get your API Key and API ID for the Recipe Search API.
Add Your API Credentials to the Code: Replace the placeholders in your code with your actual API credentials:
EDAMAM_APP_ID
EDAMAM_APP_KEY
4. Running the Streamlit App
After all dependencies are installed and configurations are complete, run the Streamlit app by using the following command:
streamlit run app.py
The app will open in your default browser. If it doesn't, you can manually navigate to http://localhost:8501 to view the app.
