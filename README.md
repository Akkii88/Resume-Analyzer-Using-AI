🚀 AI Resume Analyzer – Installation Guide
Follow these steps to set up and run the AI Resume Analyzer locally on your machine.

✅ Prerequisites
Make sure you have Python and Git installed.

Update pip to the latest version.

🧰 Step-by-Step Setup
1️⃣ Clone the Repository
bash
Copy
Edit
git clone https://github.com/Altoks-AI/AI-Resume-Analyzer.git
cd AI-Resume-Analyzer  # Replace with actual folder name if different
2️⃣ Set Up a Virtual Environment
bash
Copy
Edit
python -m venv myenv
# Activate the virtual environment
# On Windows:
.\myenv\Scripts\activate
# On macOS/Linux:
source myenv/bin/activate
3️⃣ Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
4️⃣ Configure Environment Variables
Create a .env file in the root directory and add your Groq API key:

ini
Copy
Edit
GROQ_API_KEY=your_groq_api_key_here
5️⃣ Run the Streamlit App
bash
Copy
Edit
streamlit run main.py
6️⃣ Access the Application
Once started, the app will automatically open in your default web browser:

arduino
Copy
Edit
http://localhost:8501
🎉 You're All Set!
You can now upload a resume, paste a job description, and let the AI analyze the resume for job-fit and suggestions.

🛠️ Optional Customizations
✏️ Customize Prompts:
Modify prompts in main.py to tailor the results to your needs.

🔍 Change Embedding Model:
Default is "sentence-transformers/all-mpnet-base-v2" – switch to alternatives like BERT, SBERT, etc.

🧠 Switch LLM Provider:
Currently uses Groq API with "llama-3.3-70b-versatile" model. You may switch to OpenAI GPT-4o, or another provider if needed.

🎨 UI Customizations:
Change the app title, labels, and display formatting as desired in main.py.
