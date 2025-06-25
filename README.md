## Web Survey Tool for Healthcare Industry
📌 Project Overview
This project is a Flask-based web application developed as part of a final assignment. The goal is to collect participant data and analyze their income spending patterns in preparation for a new healthcare product launch.

Deployed app at: https://mynexfordsurvey.onrender.com/

🛠️ Features
✅ Web Development with Flask
- A simple and interactive web interface to collect user input.
- Collects basic details: Age, Gender, Total Income, and Expenses.
- 
✅ Data Storage with MongoDB
- Stores user-submitted data in MongoDB Atlas.
- Expense categories are captured using checkboxes with text fields:
  * Utilities
  * Entertainment
  * School Fees
  * Shopping
  * Healthcare
    
✅ Data Processing with Python
- Implements a User class to encapsulate user data.
- Collected records are written to a CSV file for analysis.
- CSV is loaded and processed in a Jupyter Notebook for visualization.

✅ Data Visualization
- A bar chart showing ages with the highest income.
- A grouped chart showing gender distribution across spending categories.
- Visualizations are exported as image files for use in PowerPoint presentations.
  
🚀 Getting Started
1. Clone the Repository
   git clone https://github.com/url
   
3. Set Up the Virtual Environment
   python -m venv env
   env\Scripts\activate

4. Install Dependencies
   pip install -r requirements.txt

5. Configure MongoDB
   * Create a MongoDB Atlas account.
   * Set up a free-tier cluster.
   * Create a database and collection (e.g., survey_db and responses).
   * Whitelist your IP address and get the MongoDB connection URI.
   * Replace the URI in your Flask app (app.py) with the one from your MongoDB dashboard.

6. Run the App Locally
   python app.py
   The app will be available at http://127.0.0.1:5000/

🌍 Deployment
This project is deployable on Render: https://mynexfordsurvey.onrender.com/

1. Create a requirements.txt file:
   pip freeze > requirements.txt

2. Create a Procfile with the following line:
   web: gunicorn app:app

3. Push your project to GitHub.

4. On Render:
   * Create a new Web Service.
   * Connect it to your GitHub repo.
   * Use main as the branch.
   * Build and deploy.
📊 Jupyter Notebook Visualizations

After data is collected:
* Open analysis.ipynb or any notebook created.
* Load the CSV file.
* Perform analysis and generate plots.
* Export visualizations as .png or .jpeg for use in presentations.

  
📁 Project Structure

🔹 app.py                # Main Flask app

🔹 templates/            # HTML templates

🔹 static/               # Static assets (CSS, JS)

🔹 get_data.csv          # User data (generated)

🔹 data_analysis.ipynb   # Jupyter notebook for analysis

🔹 requirements.txt      # Python dependencies

🔹 Procfile              # For deployment (Render)

🔹 README.md             # Project documentation


📄 License
This project is for educational purposes and not intended for commercial use without permission.
