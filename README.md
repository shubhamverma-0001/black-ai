# 🖤 Black-AI 🚀

*A voice-activated Python assistant that listens for the trigger word **"Black"** and executes commands like opening websites & playing music.*

Black-AI is a personal voice assistant project built in **Python** using speech recognition and text-to-speech. Once **"Black"** is heard, it springs to life — ready to open browsers, launch websites, or play your favourite songs from a custom music library.  
Perfect for beginner-friendly AI and voice automation experimentation.

---

## 🤖 Features

✅ Listens for voice trigger **"Black"**  
✅ Opens popular websites (Google, YouTube, Facebook, LinkedIn)  
✅ Plays songs directly via YouTube links  
✅ Dual TTS engine — `pyttsx3` (offline) & `gTTS` + `pygame` (online, smoother voice)  
✅ Modular music library for easy song additions  
✅ News API integration ready for future expansion  

---

## 📦 Tech Stack

| Technology | Purpose |
|---|---|
| Python | Main language |
| `speech_recognition` | Voice input via microphone |
| `pyttsx3` | Offline text-to-speech (fallback) |
| `gTTS` | Google Text-to-Speech (online) |
| `pygame` | MP3 audio playback |
| `webbrowser` | Open links in browser |
| `musicLibrary.py` | Custom song → YouTube link dictionary |

---

## 📥 Installation

1. **Clone the repo**

```bash
git clone https://github.com/<your-username>/Black-AI.git
cd Black-AI
```

2. **Install dependencies**

```bash
pip install speechrecognition pyttsx3 gtts pygame
```

3. **Run the assistant**

```bash
python main.py
```

> 🎧 Make sure your **microphone is set up and working** before running.

---

## 🗣️ How It Works

1. **Black-AI** starts up and announces: *"Initializing black…."*
2. It continuously listens for audio input from your microphone.
3. When you say the keyword **"Black"**, it responds: *"Yes Bosss"* and becomes active.
4. Then say a command like:
   - *"Open YouTube"*
   - *"Open Google"*
   - *"Play goat"*
5. Black-AI executes the action — opens the website or plays the song.

---

## 📂 Project Structure

```
Black-AI/
├── main.py            # Core logic & voice command handler
├── musicLibrary.py    # Music title → YouTube link dictionary
├── README.md          # Project documentation (this file)
└── .gitignore
```

---

## 🎵 Sample Commands

| Command | Action |
|---|---|
| *"Open Google"* | Opens google.com |
| *"Open YouTube"* | Opens youtube.com |
| *"Open Facebook"* | Opens facebook.com |
| *"Open LinkedIn"* | Opens linkedin.com |
| *"Play barren"* | Plays Barren on YouTube |
| *"Play east side flow"* | Plays East Side Flow on YouTube |
| *"Play goat"* | Plays Goat on YouTube |

> ➕ Add more songs anytime in `musicLibrary.py`!

---

## 🎶 Adding Songs to the Music Library

Open `musicLibrary.py` and add entries to the dictionary:

```python
music = {
    "song name": "https://www.youtube.com/watch?v=...",
    # Add more songs here
}
```

Then just say *"Play song name"* and Black-AI will open it instantly.

---

## 📌 Contributing

Want to improve Black-AI?  
Feel free to:

- ✨ Add more voice commands
- 🎶 Expand the music library
- 🛠 Improve speech-recognition accuracy
- 📰 Integrate the News API for live headlines
- 🐛 Fix bugs or optimize performance

Just **fork the repo** and make a pull request!

---

## 🧠 Tips & Notes

- You can expand the `processCommand()` function in `main.py` to add any command you want.
- The `speak()` function uses **gTTS + pygame** for a smoother voice experience. The `old_speak()` fallback uses `pyttsx3` for offline use.
- Future ideas: weather updates, system controls, WhatsApp messaging, AI chat integration.

---

## 📜 License

This project is open-source and free to use.  
Feel free to modify and share!

---

⭐ **If you find this helpful, give it a star on GitHub!**