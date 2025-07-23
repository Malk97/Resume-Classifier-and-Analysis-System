
# Resume Data Processing Project

---

## 📌 Project Overview

This project processes a dataset of resumes (`Resume.csv`) to extract structured information such as job titles, qualifications, education details, work experience, skills, and more. The goal is to transform unstructured resume text into a structured format for further analysis (e.g., job matching, candidate ranking).

---

## 🛠️ Technologies Used

- Python (Pandas, NumPy, Regex, Scikit-learn)  
- Data Cleaning & Preprocessing  
- Feature Extraction (Regex-based parsing)  
- Statistical Analysis (Chi-square tests)  

---

## 📂 Project Structure

```
resume-processing/
│── data/
│   └── Resume.csv            # Raw resume dataset
│── scripts/
│   └── resume_processing.py  # Main processing script
│── README.md                 # This file
```

---

## 🔧 Installation & Setup

1. Clone the repository:
```bash
git clone https://github.com/yourusername/resume-processing.git
cd resume-processing
```

2. Install dependencies:
```bash
pip install pandas numpy scikit-learn
```

3. Run the script:
```bash
python scripts/resume_processing.py
```

---

## 📊 Features Extracted

| Feature                      | Description                               |
|------------------------------|-----------------------------------------|
| `POSITION_TITLE`             | Extracted job title from resume          |
| `QUALIFICATIONS`             | List of qualifications (Core Skills)     |
| `EDUCATION_TYPE`             | Degree type (Bachelor’s, Master’s, etc.) |
| `EDUCATION_MAJOR`            | Field of study (e.g., Computer Science)  |
| `EXPERIENCE_LENGTH`          | Total years of work experience            |
| `AWORDS`                    | Whether the applicant has awards (Yes/No)|
| `COMMUNITY_SERVICE`          | If the applicant has community service experience |
| `VOLUNTEERING`               | If the applicant has volunteering experience |
| `DRIVERS_LICENSE_AVAILABILITY` | Whether a driver’s license is mentioned  |
| `SKILLS_COUNT`               | Number of skills listed                   |
| `SKILLS`                    | List of skills extracted                  |
| `LANGUAGE`                   | Number of languages mentioned             |

---

## 🔍 Key Processing Steps

- **Text Cleaning:**  
  Remove unwanted characters, numbers, and extra spaces.  
  Normalize uppercase/lowercase text.

- **Regex-Based Extraction:**  
  Extract job titles, education level, and skills using pattern matching.

- **Handling Missing Data:**  
  Fill missing values based on category modes (e.g., `EDUCATION_MAJOR` filled by `EDUCATION_TYPE`).

- **Categorical Encoding:**  
  Convert text-based categories (Yes/No) into numerical values (0/1).

- **Statistical Testing:**  
  Chi-square tests to check feature associations (e.g., `POSITION_TITLE` vs. Category).

---

## 📈 Example Output

After processing, the cleaned dataset will have structured columns like:

| RESUME_NUMBER | POSITION_TITLE | EDUCATION_TYPE | SKILLS             | EXPERIENCE_LENGTH |
|---------------|----------------|----------------|--------------------|-------------------|
| 1             | Data Scientist | Master         | Python, SQL        | 5                 |
| 2             | HR Manager     | Bachelor’s     | Recruitment, Communication | 8           |

---

## 🚀 Future Improvements

- Optimize Regex Patterns: Improve accuracy in extracting job titles and skills.  
- Machine Learning Integration: Use extracted features for job matching models.  
- Interactive Dashboard: Visualize resume data trends (e.g., most common skills).

---

## 📜 License

This project is open-source under the MIT License.

---

## 📬 Contact

For questions or contributions, reach out to:  
📧 your.email@example.com  
🌐 https://github.com/yourusername

---

## 🎯 Summary

This project automates resume parsing and feature extraction, making it useful for HR analytics, recruitment tools, and data-driven hiring processes. 🚀
