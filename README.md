# Student Performance Analyzer (Python)

## Project overview
A beginner-friendly data analytics dashboard that reads student marks from a CSV file, calculates totals and averages, assigns performance bands, displays subject averages and grade distribution, highlights students below a selected average, and lets users download analyzed results.

## Tech stack
- Python
- Streamlit (dashboard interface)
- pandas (CSV and calculations)
- matplotlib (charts)

## Run it on your laptop
1. Install Python 3.10 or newer from https://www.python.org/downloads/ (during installation on Windows, tick **Add Python to PATH**).
2. Extract this ZIP file to a folder.
3. Open Command Prompt / Terminal in that folder.
4. Create a virtual environment (recommended):
   - Windows: `py -m venv .venv` then `.venv\Scripts\activate`
   - macOS/Linux: `python3 -m venv .venv` then `source .venv/bin/activate`
5. Install packages: `python -m pip install -r requirements.txt`
6. Start the app: `python -m streamlit run app.py`
7. A browser tab should open automatically. If not, copy the local URL shown in the terminal (usually http://localhost:8501).

## Data format
Use `student_performance.csv` as the template. Required columns:
`Student_ID, Student_Name, Maths, Science, English, Computer`
Marks should be numeric values from 0 to 100.

## How it works
1. Reads the supplied sample CSV or an uploaded CSV.
2. Validates required columns.
3. Converts subject marks to numeric values and skips rows with missing/non-numeric marks.
4. Calculates each student's total and mean.
5. Assigns performance bands: A (90+), B (80–89.99), C (70–79.99), D (60–69.99), Needs Support (below 60).
6. Shows summary metrics, subject-average chart, grade distribution chart, and a filtered support list.
7. Offers a CSV download of analyzed results.

## Important notes
- The included student names and marks are fictional sample data.
- Explain the project in your own words and customize at least one part (for example, add your name, change the colors/layout, add a subject, or test with a small CSV you create).
- Do not upload real student personal data without permission.
