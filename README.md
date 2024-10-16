## AI-Medical Diagnosis System
#### This project is an AI-powered healthcare web application designed to assist users in predicting potential diseases based on their symptoms. Leveraging machine learning models, the system provides an accurate diagnosis, along with additional information about the expected disease, such as precautions, medications, recommended diets, and workout plans. The project is built using Streamlit for the user interface and Scikit-learn for model deployment.

### Key Features:
* Symptom Input: Users can input multiple symptoms in natural language.
* Disease Prediction: The AI model predicts the most likely disease based on the provided symptoms.
* Disease Description: Detailed description of the predicted disease.
* Precautions: Suggested preventive measures to avoid worsening the condition.
* Medications: List of common medications used for treating the predicted disease.
* Diet Recommendations: Suggested dietary plans that complement the treatment.
* Workout Plans: Exercises that can help improve recovery based on the disease.

### Technology Stack:
* Python: Core language used for backend processing.
* Streamlit: Web framework used to build an interactive user interface.
* Scikit-Learn: Machine learning library used for training and predicting diseases.
* Pandas: Data manipulation and analysis library.
* Pickle: Used for loading the pre-trained machine learning model.
* CSV Datasets: Symptom descriptions, precautions, medications, diets, and workout plans are stored in CSV format.

### Setup:
1. Clone the Repository:
```
git clone https://github.com/AbdAziz1/AI-Medical-System.git
cd AI-Medical-System
```
2. Create a Virtual Environment (optional but recommended):
```
python -m venv .venv
source .venv/bin/activate  # For Windows: .venv\Scripts\activate
```
3. Install Dependencies: Install all required Python libraries by running:
```
pip install -r requirements.txt
```
4. Run the Application: Use the following command to start the Streamlit web application:
```
streamlit run app.py
```
5. Access the Web Application: After running the command, the application will be available at http://localhost:8501/. Open this URL in your browser to interact with the app.

### Folder Structure:
```
├── app.py                 # Main Streamlit app file
├── model.pkl              # Pre-trained machine learning model
├── medicaldata/           # Folder containing CSV files for symptoms, medications, diets, etc.
│   ├── symptoms_df.csv
│   ├── precautions_df.csv
│   ├── workout_df.csv
│   ├── description.csv
│   ├── medications.csv
│   └── diets.csv
├── requirements.txt       # Python dependencies file
├── README.md              # Project description and setup instructions
```
### How It Works:
* Input Symptoms: The user enters a comma-separated list of symptoms.
* Predict Disease: The machine learning model processes the symptoms and predicts the most probable disease.
* Display Results: The system displays the disease description, along with appropriate precautions, medications, diets, and workouts.

### Future Improvements:
* Expanding the database with more diseases and symptoms.
* Integrating additional machine learning models to improve prediction accuracy.
* Providing real-time updates from medical databases for symptoms, medications, and treatments.
