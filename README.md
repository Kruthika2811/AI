# 🎤 Voice Assistant

A Python-based voice assistant with speech recognition, Wikipedia search, web browsing, and text-to-speech capabilities. Available in multiple interfaces: command-line, web app, and Streamlit app.

## 🌟 Features

- **Time & Date Queries**: Get current time and date
- **Wikipedia Search**: Search and get summaries from Wikipedia
- **Website Opening**: Open popular websites with clickable links
- **Natural Language Processing**: Understands various command formats
- **Multiple Interfaces**: Choose from CLI, web, or Streamlit interface
- **Cross-Platform**: Works on Windows, macOS, and Linux
- **No OpenAI Dependency**: Uses offline speech recognition and TTS

## 🚀 Quick Start

### Web Interface (Recommended)
```bash
python web_app.py
```
Visit `http://localhost:5000` in your browser.

### Streamlit Interface
```bash
streamlit run streamlit_app.py
```
Visit `http://localhost:8501` in your browser.

### Command Line (Requires microphone)
```bash
python main.py
```

### Demo Mode (Text-based testing)
```bash
python demo_mode.py
```

## 📦 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/voice-assistant.git
   cd voice-assistant
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
   Or using the provided dependencies:
   ```bash
   pip install flask streamlit pyaudio pyttsx3 speechrecognition wikipedia wikipedia-api
   ```

3. **Run the application:**
   ```bash
   # For web interface
   python web_app.py
   
   # For Streamlit interface
   streamlit run streamlit_app.py
   ```

## 🎯 Usage Examples

### Supported Commands

- **Time**: "What time is it?", "Tell me the time"
- **Date**: "What date is it?", "What day is it?"
- **Wikipedia**: "Search Wikipedia for artificial intelligence", "Tell me about Python programming"
- **Websites**: "Open Google", "Visit YouTube", "Go to GitHub"
- **Greetings**: "Hello", "Hi", "Good morning"
- **Help**: "Help", "What can you do?"

### Web Interface
The web interface provides:
- Chat-style interaction
- Quick command buttons
- Clickable website links
- Conversation history
- Mobile-responsive design

### Streamlit Interface
The Streamlit interface offers:
- Modern UI with quick action buttons
- Real-time chat functionality
- Popular search shortcuts
- Sidebar with examples and controls

## 🏗️ Project Structure

```
voice-assistant/
├── voice_assistant/
│   ├── __init__.py
│   ├── speech_handler.py      # Speech recognition
│   ├── tts_handler.py         # Text-to-speech
│   └── command_processor.py   # Command processing logic
├── templates/
│   └── index.html            # Web interface template
├── main.py                   # Full voice assistant (CLI)
├── web_app.py               # Flask web interface
├── streamlit_app.py         # Streamlit interface
├── demo_mode.py             # Text-based demo
├── auto_demo.py             # Automatic demonstration
├── config.py                # Configuration settings
└── README.md               # This file
```

## 🔧 Configuration

Edit `config.py` to customize:
- Wake words and exit commands
- Website shortcuts
- Speech recognition settings
- Text-to-speech parameters

## 🌐 Deployment

### Local Development
```bash
# Flask
python web_app.py

# Streamlit
streamlit run streamlit_app.py
```

### Streamlit Cloud
1. Push to GitHub
2. Connect to [Streamlit Cloud](https://streamlit.io/cloud)
3. Deploy with `streamlit_app.py` as main file

### Replit
The project is ready to run on Replit with pre-configured workflows.

## 🛠️ Technologies Used

- **Python 3.11+**
- **Flask** - Web framework for HTTP interface
- **Streamlit** - Modern web app framework
- **SpeechRecognition** - Speech-to-text conversion
- **pyttsx3** - Text-to-speech synthesis
- **PyAudio** - Audio input/output handling
- **Wikipedia** - Knowledge base integration

## 🎮 Interface Comparison

| Feature | CLI | Web App | Streamlit |
|---------|-----|---------|-----------|
| Microphone Required | ✅ | ❌ | ❌ |
| Browser Interface | ❌ | ✅ | ✅ |
| Mobile Friendly | ❌ | ✅ | ✅ |
| Quick Commands | ❌ | ✅ | ✅ |
| Modern UI | ❌ | ⚡ | ✅ |
| Real-time Chat | ❌ | ✅ | ✅ |

## 🔊 Audio Requirements

- **Full Voice Mode** (`main.py`): Requires microphone and speakers
- **Web/Streamlit Modes**: No audio hardware needed
- **Demo Mode**: Text-only, no audio required

## 🐛 Troubleshooting

### Common Issues

1. **Audio Device Errors**: Use web or Streamlit interface instead of CLI mode
2. **Port Already in Use**: Change port in the code or kill existing processes
3. **Import Errors**: Install all dependencies with `pip install -r requirements.txt`
4. **Wikipedia Timeouts**: Check internet connection

### Cloud Deployment Notes
- CLI mode requires local audio hardware
- Web and Streamlit modes work perfectly in cloud environments
- Use web interfaces for Replit, Heroku, or similar platforms

## 📄 License

This project is open source and available under the MIT License.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📞 Support

For issues or questions:
- Open an issue on GitHub
- Check the troubleshooting section
- Review the configuration options

---

**Built with ❤️ using Python and modern web frameworks**
