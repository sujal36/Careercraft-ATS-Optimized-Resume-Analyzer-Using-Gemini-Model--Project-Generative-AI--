CareerCraft: ATS-Optimized Resume Analyzer Using Gemini Model - README
CareerCraft is an ATS-optimized resume analysis tool designed to evaluate the compatibility between a candidate's resume and a job description. Using Google Generative AI, this tool offers insightful feedback to help users tailor their resumes for specific job applications. The application is hosted on a Streamlit platform, allowing seamless interaction through an intuitive web interface.

Features
User-Friendly Interface: Provides clear sections for uploading resumes, entering job descriptions, and viewing results.
PDF Resume Parsing: Efficiently extracts text from PDF resumes.
AI-Powered Analysis: Uses Google Generative AI for precise, job-focused resume analysis.
Custom Styling: Enhances user experience with tailored design elements.
Doughnut Chart Visualization: Displays analysis results visually for easier interpretation.
Technologies Used
Streamlit: Simplifies the development of the web app interface.
Python: Core language used for development.
Google Generative AI: Powers the resume analysis functionality.
dotenv: Manages environment variables for secure configuration.
PyPDF2: Extracts text from PDF resumes.
Pillow (PIL): Manages images within the app.
Matplotlib: Used for visualizing data, such as doughnut charts for result representation.
How It Works
Environment Setup:
Loads the API key securely from a .env file using the dotenv library.
The Google API key is configured for interaction with the Google Generative AI model.
Streamlit Application Flow:
Displays a clean and interactive UI for resume upload, job description input, and results display.
The input_pdf_text function extracts text from uploaded PDFs.
The get_gemini_response function communicates with the AI model, sending both resume text and job description for analysis.
User Interaction:
Users upload PDF-format resumes and enter job descriptions.
Displays a loading spinner during AI processing.
Results are presented with a match percentage, missing keywords, and a brief profile summary.
Resume Analysis Output:
Shows how closely the resume aligns with the job description.
Highlights missing keywords, providing a clear profile summary for improvement.
Setup Instructions
Clone the Repository: git clone <repository_url> cd resume-ats-tracker

Install Dependencies: pip install streamlit python-dotenv google-generativeai pypdf2 pillow matplotlib

Create a .env File:

Add your Google API Key: GOOGLE_API_KEY=your_api_key_here
Run the Application: streamlit run app.py
File Structure
app.py:Main application file for Streamlit code.
.env: Environment file containing API key for secure access.
Usage Instructions
Start the Application:
Run streamlit run app.pyto launch the app.
Upload Resume:
Upload your resume in PDF format.
Enter Job Description:
Fill in the job description field.
Submit for Analysis:
Click "Submit" to initiate the resume analysis.
Review Results:
Analyze the match percentage, keywords, and summary to optimize your resume accordingly.
Deployment Link
Resume Analyzer

Acknowledgments
Streamlit for providing a user-friendly framework.
Google Generative AI for powering resume analysis.
dotenv for environment management.
PyPDF2 for PDF text extraction.
Pillow (PIL) for image handling.
Matplotlib for doughnut chart data visualizatio
