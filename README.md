# Automated Hiring Bias Analysis Tool

## Overview
The **Automated Hiring Bias Analysis Tool** helps detect gender and racial biases in hiring processes. It analyzes recruitment data, provides an NLP-based bias report, and visualizes selection rates. Users can upload data, view insights, and download the analysis report, helping organizations ensure fair and unbiased hiring practices.

## Requirements
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `streamlit`

To install the required libraries, run:

```bash
pip install pandas numpy matplotlib seaborn streamlit
```

# How to Run

1. Clone or download the repository.
2. Navigate to the project directory in your terminal.
3. Run the app with the following command:

    ```bash
    streamlit run app.py
    ```

4. The app will open in your default browser.

---

# Data Format

The input data should be in CSV format with the following columns:

- `gender`: Candidate's gender (e.g., 'male', 'female')
- `race`: Candidate's race (e.g., 'white', 'black')
- `received_callback`: Binary outcome (1 = yes, 0 = no)
- Job-related factors: `job_req_education`, `job_req_min_experience`, `job_req_computer`, `college_degree`, `years_experience`, `computer_skills`, `resume_quality`

**Example:**

```csv
gender,race,received_callback,job_req_education,job_req_min_experience,job_req_computer,college_degree,years_experience,computer_skills,resume_quality
male,white,1,high,5,advanced,yes,3,yes,high
female,black,0,medium,3,intermediate,no,1,yes,medium
```

# Features

- **Bias Detection**: Identifies gender and racial biases in the hiring process based on callback rates.
- **NLP Explanation**: Provides a detailed explanation of the bias detected in the hiring process.
- **Visualizations**: Displays graphs for selection rates by gender and race, and a heatmap showing correlations between job factors and callback rate.
- **Data Upload/Manual Entry**: Users can upload CSV files or enter data manually in the app.
- **Downloadable Report**: Users can download the analysis report as a text file.

---

# How It Works

1. **Data Upload**: Upload a CSV file or enter data manually in the app.
2. **Data Processing**: The tool processes the data and calculates selection rates, bias ratios, and job-related factors.
3. **Bias Report**: The app generates an automated NLP-based bias analysis report, highlighting gender and racial bias, along with the impact of job qualifications on hiring decisions.
4. **Visualizations**: The app also displays visualizations to aid in understanding the data and bias.
5. **Downloadable Report**: After analyzing the data, users can download the detailed bias report in a text file format.

---

# Example Workflow

1. Open the app.
2. Choose to either upload a CSV or enter data manually.
3. View the preview of the uploaded data.
4. Analyze the bias using the tool’s automated analysis.
5. Download the generated bias report.
6. Visualize selection rates and correlations.

# Contact

For questions, reach out at: @gurpreet.go2103@gmail.com  &  ishmeetlotey04@gmil.com
