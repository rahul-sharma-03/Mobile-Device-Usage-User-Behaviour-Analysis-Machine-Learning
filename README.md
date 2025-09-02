 # 📱 Mobile Device Usage and User Behaviour Analysis
 _Classifying user behavior patterns from mobile device data using machine learning to uncover actionable insights._
 ---
 📌 Table of Contents
 
- <a href="#overview">Overview</a>

- <a href="#business-problem">Business Problem</a>

- <a href="#dataset">Dataset</a>

- <a href="#tools--technologies">Tools & Technologies</a>

- <a href="#project-structure">Project Structure</a>

- <a href="#methodology">Methodology</a>

- <a href="#results-and-visualizations">Results and Visualizations</a>

- <a href="#gui-dashboard">GUI Dashboard</a>

- <a href="#how-to-run-this-project">How to Run This Project</a>

- <a href="#key-takeaways--next-steps">Key Takeaways & Next Steps</a>

- <a href="#author--contact">Author & Contact</a>

---
<h2><a class="anchor" id="overview"></a>📝 Overview</h2>
This project focuses on analyzing mobile device usage data to understand and classify user behavior. By leveraging various machine learning algorithms,
the goal is to build a robust classification model that can predict a user's behavior class based on features like app usage, screen time, and battery drain.
The project demonstrates a complete data science workflow, from data exploration and preprocessing to model training, evaluation, and the development of an interactive user interface for real-time predictions.

---
<h2><a class="anchor" id="business-problem"></a>🎯 Business Problem</h2>
Understanding how users interact with their mobile devices is crucial for app developers, marketers, and device manufacturers. This project aims to solve this by:

- **Segmenting Users**: Automatically classifying users into distinct behavioral groups (e.g., light, moderate, heavy users).

- **Personalizing Experiences**: Providing insights that can help tailor user experiences, such as optimizing battery life or personalizing app recommendations.

- **Enabling Targeted Strategies**: Allowing businesses to develop targeted marketing and engagement strategies based on how different user segments behave.

---
<h2><a class="anchor" id="dataset"></a>💾 Dataset</h2>
  The project utilizes the user_behavior_dataset.csv, a dataset containing various metrics of mobile device usage.

- **Key Features**: App Usage Time, Screen On Time, Battery Drain, Number of Apps Installed, Data Usage, Age, and Gender.

- **Target Variable**: User Behavior Class, a categorical variable representing different levels of user engagement.

---
<h2><a class="anchor" id="tools--technologies"></a>🛠️ Tools & Technologies</h2>

- **Python**: The core programming language for the project.

**Libraries**:

- **Pandas & NumPy**: For efficient data loading, manipulation, and numerical operations.

- **pandas-profiling**: For generating an in-depth, automated exploratory data analysis report.

- **Scikit-learn**: For implementing the entire machine learning pipeline, including data preprocessing (StandardScaler), model training (Logistic Regression, SVM, Random Forest, etc.), and evaluation (accuracy_score, classification_report).

- **Matplotlib & Seaborn**: For comprehensive data visualization and exploratory data analysis.

- **Tkinter**: For building an intuitive graphical user interface (GUI) to make predictions.

- **Pickle**: For saving the trained machine learning model so it can be deployed in the GUI.

---
<h2><a class="anchor" id="project-structure"></a>🏗️ Project Structure</h2>

```
user-behavior-classification/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── notebooks/
│   └── Mobile-Device-Usage-User-Behaviour-Analysis.ipynb
│
├── data/
│   └── user_behavior_dataset.csv
│
├── models/
│   └── user_behavior_model.pkl
```

---
<h2><a class="anchor" id="methodology"></a>🔬 Methodology</h2>

- **Automated Exploratory Data Analysis (EDA)**: An initial, comprehensive analysis was performed using pandas-profiling to generate a detailed report. This step automatically provided key insights into data types, missing values, correlations, and feature distributions, significantly speeding up the EDA process.

- **Manual EDA**: Following the automated report, a manual exploration was conducted with Matplotlib and Seaborn to create custom visualizations and further investigate specific relationships between features.

- **Data Preprocessing**: Categorical features like Gender are converted into numerical format using LabelEncoder. The data is then split into training and testing sets, and features are scaled using StandardScaler to ensure optimal model performance.

- **Model Training**: A variety of classification algorithms are trained on the preprocessed data, including Logistic Regression, Support Vector Machines (SVM), Decision Trees, and Random Forest.

- **Model Evaluation**: Each model's performance is evaluated using metrics like accuracy and the classification report to identify the best-performing model for the task.

- **Model Saving**: The final, most accurate model (Random Forest) is saved as a .pkl file using the Pickle library, making it ready for deployment.

---
<h2><a class="anchor" id="results-and-visualizations"></a>📊 Results and Visualizations</h2>

- **Feature Importance**: The initial pandas-profiling report and subsequent manual analysis both highlighted that App Usage Time, Screen On Time, and Battery Drain are the most significant predictors of user behavior.

- **Model Performance**: The Random Forest Classifier achieved the highest accuracy (over 98%) on the test set, proving to be the most effective model for this classification problem.

- **Visualizations**: The project includes various insightful plots, such as correlation heatmaps and distribution plots, which help in understanding the relationships between different usage metrics.

---
<h2><a class="anchor" id="gui-dashboard"></a>🖥️ GUI Dashboard</h2>

- An interactive GUI was developed using Tkinter, allowing users to input mobile usage data and receive an instant prediction of the user's behavior class.

- The interface provides a simple form for entering feature values and displays the predicted class clearly. This makes the model accessible and easy to use for non-technical users.

---
<h2><a class="anchor" id="how-to-run-this-project"></a>🚀 How to Run This Project</h2>

1. **Clone the repository**:
```bash
git clone https://github.com/yourusername/user-behavior-classification.git
```
2. **Install the required libraries**:
```bash
pip install -r requirements.txt
```
3. **Run the Jupyter Notebook for a detailed walkthrough**:
```bash
notebooks/Mobile-Device-Usage-User-Behaviour-Analysis.ipynb
```
4. **To use the GUI for predictions, run the relevant Python script.**

---
<h2><a class="anchor" id="key-takeaways--next-steps"></a>🔑 Key Takeaways & Next Steps</h2>

- **Key Takeaways**: This project successfully proves that machine learning models, especially Random Forest, can classify user behavior from mobile data with high accuracy. The key predictors of user behavior are App Usage Time, Screen On Time, and Battery Drain. The Tkinter GUI provides a simple yet effective way to deploy the model for practical use.

- **Next Steps**:

- **Live Data Integration**: Move from static CSV analysis to a real-time system that can analyze live user data streams.

- **Discover New Segments**: Apply unsupervised clustering algorithms to identify new and potentially more nuanced user groups.

- **Boost Performance**: Experiment with advanced models like XGBoost or LightGBM to push for even higher predictive accuracy.

---
<h2><a class="anchor" id="author--contact"></a>✍️ Author & Contact</h2>

**B Rahul Sharma**  
Data Analyst  
📧 Email: brahulsharma02@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/bukkapatnam-rahulsharma/)



 
