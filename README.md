# 📞 AI-Powered Outbound Calling Platform

A sophisticated Streamlit application that automates outbound sales calls using AI assistants from Vapi. This platform enables businesses to efficiently manage leads, create custom AI agents, and conduct batch calling campaigns with real-time interaction handling.

## 🚀 Key Features

- **📋 Lead Management** - CSV-based lead import with status tracking (pending/done)
- **🤖 AI Assistant Creation** - Build custom sales assistants with voice selection and behavior customization
- **🚀 Batch Calling** - Automated sequential calling to multiple leads with intelligent pacing
- **⏱️ Real-time Interaction** - Smart call handling with pause/resume during customer speech
- **💬 Multi-channel Support** - Voice calls and WhatsApp messaging capabilities
- **📊 Deals Pipeline** - Track successful conversions and sales outcomes

## 🛠️ Technical Stack

- **Frontend**: Streamlit for intuitive web interface
- **AI Integration**: Vapi.ai for voice AI capabilities
- **Data Management**: Pandas for CSV processing, JSON for configuration storage
- **APIs**: RESTful integration with Vapi's voice AI platform

## 📦 Installation

### Prerequisites
- Python 3.8+
- Vapi API account
- Twilio account (for phone numbers)

### Step 1: Clone the Repository
```bash
git clone https://github.com/Hasan8123/outbound-calling-app.git
cd outbound-calling-app
```

### Step 2: Install Dependencies
```bash
pip install streamlit pandas python-dotenv requests
```

### Step 3: Environment Configuration
Create a `.env` file in the root directory:
```env
VAPI_API_KEY=your_vapi_api_key_here
TWILIO_ACCOUNT_SID=your_twilio_account_sid
```

### Step 4: Prepare Leads CSV
Create `numbers.csv` with the following columns:
```csv
phone,name,status
+1234567890,John Doe,pending
+1987654320,Jane Smith,pending
```

### Step 5: Run the Application
```bash
streamlit run app.py
```

## 💡 Usage Guide

### 1. **Leads Management Tab**
- Upload your CSV file with customer numbers
- View pending and completed calls
- Monitor lead status in real-time

### 2. **Assistants Management Tab**
- Create custom AI assistants with specific voices and personalities
- Set initial messages and behavior instructions
- Manage multiple assistants for different campaigns

### 3. **Start Calls Tab**
- Select your AI assistant
- Initiate batch calls to all pending leads
- Monitor call progress in real-time

### 4. **Deals Tab**
- Track successful conversions
- Analyze call outcomes and performance metrics

## 🎯 Use Cases

- **Sales Teams**: Automate cold outreach campaigns
- **Customer Service**: Follow-up calls and satisfaction surveys
- **Healthcare**: Appointment reminders and follow-ups
- **Market Research**: Conduct automated surveys via voice AI

## 🔧 Configuration

### AI Assistant Settings
Customize your assistant with:
- Voice selection (11Labs integration)
- GPT model choice (3.5-turbo, GPT-4, etc.)
- Custom instructions and behavior patterns
- Call duration limits and interruption settings

### Call Management
- Adjust call pacing between leads
- Configure real-time speech detection
- Set up custom call workflows

## 📁 Project Structure
```
outbound-calling-app/
├── app.py                 # Main application file
├── numbers.csv           # Leads database
├── assistants.json       # AI assistants storage
├── deals.json           # Closed deals tracking
├── .env                 # Environment variables
└── README.md           # This file
```

## 🔒 Environment Variables
| Variable | Description | Required |
|----------|-------------|----------|
| `VAPI_API_KEY` | Your Vapi.ai API key | ✅ |
| `TWILIO_ACCOUNT_SID` | Twilio account SID for calling | ✅ |

## 🚀 Deployment

### Local Deployment
```bash
streamlit run app.py
```

### Cloud Deployment (Streamlit Cloud)
1. Push code to GitHub repository
2. Connect to Streamlit Cloud
3. Set environment variables in cloud dashboard
4. Deploy automatically

## 🤝 Contributing

We welcome contributions! Please feel free to submit pull requests for:
- New features and enhancements
- Bug fixes and optimizations
- Documentation improvements

## ⚠️ Important Notes

- Ensure compliance with telecommunications regulations in your region
- Respect Do Not Call lists and privacy laws
- Test call volumes to avoid carrier limitations
- Monitor AI behavior for quality assurance

## 🆘 Support

For issues and questions:
1. Check existing GitHub issues
2. Create a new issue with detailed description
3. Contact support with your use case

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

**Ready to transform your outbound sales** 🚀 Start calling with AI today!
