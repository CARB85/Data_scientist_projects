# Web Application Development Project

## Project Description
This project is designed to help to practice typical software engineering tasks

The tasks include:
- Creating and managing Python virtual environments.
- Developing a web application.
- Deploying the application to a cloud service for public access.

A car sales dataset is provided, but the focus of the project is not on the dataset or analysis.

### Demo of the Web Application
_Include a screenshot or link to your demo application here "https://github.com/CARB85/web_aplication.git"

---

## Instructions for Completing the Project

### Step 1: Setup
1. **GitHub Setup:**
   - Create an account at [github.com](https://github.com) if you don't have one.

2. **Render.com Setup:**
   - Create an account at [render.com](https://render.com). Use the "GitHub" option to link your Render account with GitHub.

3. **Install Required Packages:**
   - Create a Python virtual environment with a meaningful name (e.g., `vehicles_env`).
   - Install the following packages in your environment:
     - `pandas`
     - `plotly_express`
     - `streamlit`
   - Create a `requirements.txt` file in your project directory and include these libraries:
     ```
     pandas
     plotly_express
     streamlit
     ```

4. **Set Up Your Development Environment:**
   - Install [VS Code](https://code.visualstudio.com/) if you haven’t already.
   - Clone your project repository from GitHub and open it in VS Code.
   - Set the Python interpreter to use your virtual environment.

---

### Step 2: Dataset Preparation
1. Download the car sales dataset (`vehicles_us.csv`) or use your own dataset in CSV format.
2. Place the dataset in your project directory.

---

### Step 3: Exploratory Data Analysis (EDA)
1. Create a directory called `notebooks` in your project directory.
2. In VS Code, create a Jupyter notebook named `EDA.ipynb` and save it in the `notebooks` directory.
3. Use `plotly-express` to create basic visualizations for EDA. Examples include:
   - Histograms.
   - Scatter plots.

---

### Step 4: Develop the Web Application Dashboard
1. Create a file named `app.py` in the root directory of your project.
2. Import the required libraries (`streamlit`, `pandas`, `plotly_express`).
3. Read the dataset into a DataFrame and create the following:
   - **Header:** Use `st.header()` to create a header for your application.
   - **Buttons for Visualizations:**
     - A button to generate a histogram.
     - A button to generate a scatter plot.
   - **Optional:** Use checkboxes (`st.checkbox()`) to provide more interactive options for users.

