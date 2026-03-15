# 🔌 CloudEagle AI Integration Code Generator

An AI-powered tool that generates production-ready API integration code in minutes using Claude 3.5 Sonnet.

![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Anthropic](https://img.shields.io/badge/Claude-191919?style=for-the-badge&logo=anthropic&logoColor=white)

## 🌟 Features

- 🤖 **AI-Powered Code Generation** - Leverages Claude 3.5 Sonnet to analyze API documentation and generate complete integration code
- 🛡️ **Built-in Safety Checks** - Automated security scans, style validation, and credential safety checks
- 📦 **Complete Integration Package** - Generates API client, authentication, data sync, error handling, and configuration modules
- 🧪 **Sandbox Testing** - Test integrations safely before production deployment
- 💅 **Beautiful UI** - Modern, professional interface with custom theming
- ⚡ **Fast & Efficient** - Generate integration code in minutes instead of days

## 🚀 Quick Start

### Prerequisites

- Python 3.9 or higher
- Anthropic API key ([Get one here](https://console.anthropic.com))

### Local Development

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd cloudeagle-integration-builder
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables**
   
   Create a `.env` file in the project root:
   ```bash
   ANTHROPIC_API_KEY=your_api_key_here
   ```

4. **Run the app**
   ```bash
   streamlit run app.py
   ```

5. **Open your browser**
   
   Navigate to `http://localhost:8501`

## 🌐 Deploy to Streamlit Cloud

### Step 1: Push to GitHub

```bash
git init
git add .
git commit -m "Initial commit: CloudEagle Integration Builder"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

### Step 2: Deploy on Streamlit Cloud

1. Go to [share.streamlit.io](https://share.streamlit.io)
2. Sign in with GitHub
3. Click "New app"
4. Select your repository
5. Set main file path: `app.py`
6. Click "Deploy"

### Step 3: Add Secrets

In Streamlit Cloud dashboard:

1. Go to your app settings
2. Click "Secrets"
3. Add your Anthropic API key:
   ```toml
   ANTHROPIC_API_KEY = "your_api_key_here"
   ```
4. Save

Your app will be live at: `https://YOUR_APP_NAME.streamlit.app`

## 📚 How It Works

### 1. **Input API Documentation**
   - Provide a URL to the API documentation
   - Or select from popular integrations (Calendly, Slack, Salesforce, etc.)

### 2. **AI Code Generation**
   - Claude 3.5 Sonnet analyzes the documentation
   - Generates production-ready Python code
   - Creates 5 core modules:
     - `api_client.py` - Main API client
     - `auth.py` - OAuth 2.0 authentication
     - `data_sync.py` - Data retrieval functions
     - `error_handler.py` - Error handling & retries
     - `config.py` - Configuration management

### 3. **Safety Validation**
   - Automatic security scans
   - Code style validation (PEP 8)
   - Credential safety checks
   - Rate limiting verification

### 4. **Sandbox Testing**
   - Test integration in isolated environment
   - Verify authentication flow
   - Validate data retrieval
   - Check error handling

### 5. **Download & Deploy**
   - Download complete package as ZIP
   - Includes README with setup instructions
   - Ready for CloudEagle platform integration

## 🎯 Generated Code Includes

✅ **Complete API Client** - Fully structured class with all endpoints
✅ **OAuth 2.0 Authentication** - Secure authentication flow
✅ **Data Retrieval Functions** - User data and usage statistics
✅ **Error Handling** - Retry logic with exponential backoff
✅ **Pagination Support** - Handle large datasets efficiently
✅ **Rate Limiting** - Respect API constraints automatically
✅ **Comprehensive Logging** - Debug and monitor integration
✅ **Type Hints** - Full type annotations for better IDE support
✅ **Documentation** - Detailed docstrings and comments

## 🛡️ Security Features

- ✅ No hardcoded credentials
- ✅ Environment variable configuration
- ✅ Input validation
- ✅ Secure authentication flows
- ✅ Rate limiting protection
- ✅ Comprehensive error handling

## 📖 Usage Example

1. **Visit the app** (local or deployed)
2. **Select "Calendly"** from popular integrations
3. **Click "Generate Integration Code"**
4. **Review generated files** in the Review tab
5. **Download ZIP** with all code
6. **Test in sandbox** before production
7. **Deploy** to CloudEagle platform

## 🏗️ Project Structure

```
cloudeagle-integration-builder/
├── app.py                      # Main Streamlit application
├── requirements.txt            # Python dependencies
├── .streamlit/
│   └── config.toml            # Streamlit theme configuration
├── .gitignore                 # Git ignore file
└── README.md                  # This file
```

## 🎨 UI Features

- **Modern Design** - Clean, professional interface
- **Custom Theme** - Branded colors and styling
- **Responsive Layout** - Works on all screen sizes
- **Syntax Highlighting** - Beautiful code display
- **Progress Indicators** - Clear feedback during generation
- **Tabbed Interface** - Organized workflow

## 🤝 Contributing

This project was built for the CloudEagle PM assignment. If you'd like to extend it:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📝 License

MIT License - Feel free to use this code for your projects!

## 🙏 Acknowledgments

- **Anthropic** - For Claude 3.5 Sonnet API
- **Streamlit** - For the amazing app framework
- **CloudEagle** - For the assignment opportunity

## 📧 Contact

Built by [Your Name] for CloudEagle PM Assignment

---

**Powered by Claude 3.5 Sonnet** 🤖
