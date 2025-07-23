
# 🛡️ AI-Powered Python Code Reviewer

This project uses OpenAI's GPT model to **automatically review and annotate Python source code** with meaningful and security-conscious comments. It's ideal for educational use, peer review, or security audits.

---

## 📌 Features

- ✅ Loads a Python source file (`source_code.py`)
- 🤖 Sends it to OpenAI's GPT-3.5 model for review
- 🛡️ Annotates functions and lines with:
  - Purpose explanations
  - Security insights
  - Inline comments using `#` (not triple quotes)
- 💾 Outputs the commented version to `source_code_commented.py`

---

## 📁 File Structure

```
.
├── review_script.py              # Main script that reviews and annotates code
├── source_code.py               # Your input Python file (to be reviewed)
├── source_code_commented.py     # Output file with comments added
└── README.md                    # This documentation
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/code-reviewer.git
cd code-reviewer
```

### 2. Set OpenAI API Key

Make sure you have your OpenAI API key set as an environment variable:

**Linux/macOS**
```bash
export OPENAI_API_KEY=your_api_key_here
```

**Windows (PowerShell)**
```powershell
$env:OPENAI_API_KEY="your_api_key_here"
```

---

### 3. Place Your Python File

Replace or create a file named `source_code.py` in the project directory. This is the file that will be reviewed.

---

### 4. Run the Script

```bash
python review_script.py
```

---

### ✅ Output

After execution, a new file `source_code_commented.py` will be generated with detailed inline comments added by the AI.

---

## 📦 Dependencies

- Python 3.7+
- [`openai`](https://pypi.org/project/openai/)

Install using pip:

```bash
pip install openai
```

---

## 💡 Use Cases

- Security-focused code review
- Teaching Python to students with AI-generated comments
- Documenting legacy code automatically
- Catching potential vulnerabilities in logic flow

---

## 🔐 Notes

- Ensure your API key has access to GPT-3.5 or higher.
- GPT model responses may vary slightly each time due to temperature settings.

---

## 🧠 Future Enhancements

- ✅ Multi-file support
- 🖼️ Web UI with file upload (Streamlit or Flask)
- 🧪 Highlighting only security flaws
- 🔄 GitHub action integration for PR review bots
