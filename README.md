# 🎙️ AI Call Transcript Tool (Groq + Whisper + LLM Cleanup)

A powerful browser-based tool to upload multiple audio files (WAV/MP3/etc.) and generate clean, structured Hindi call transcripts.

---

## 🚀 Features

### ✅ Multi-file Upload
- Upload multiple audio files at once  
- Drag & drop support  
- Supports:
  - WAV
  - MP3
  - M4A
  - FLAC
  - OGG  

---

### 🧠 2-Step AI Processing

#### 1. 🎧 Transcription (Whisper)
Converts audio → raw text  

#### 2. ✨ AI Cleanup (LLM)
Transforms raw text into structured conversation:

```
ग्राहक: हेलो!
कस्टमर सपोर्ट: नमस्ते सर...
```

- Speaker separation (ग्राहक / कस्टमर सपोर्ट)  
- Noise tags → *(पृष्ठभूमि में शोर)*  
- Clean readable formatting  

---

### 📊 Smart Processing (V3)

#### ⚠️ Rate Limit Handling
- Detects Groq rate limits  
- Auto wait + retry  
- Countdown timer  

#### 📦 Large File Compression
- Converts to 16kHz mono WAV  
- Reduces large files (50MB → ~5–8MB)  

#### 🔁 Auto Retry
- Handles network/API failures automatically  

---

### 🎨 UI Features

- Two tabs:
  - ✨ Clean Dialogue  
  - 📝 Raw Transcript  

- Color coding:
  - ग्राहक (Red)
  - कस्टमर सपोर्ट (Blue)

- Progress tracking:
```
Upload → Whisper → AI Cleanup → Done
```

---

### 📥 Export Options

- Download:
  - Individual `.txt`
  - Individual `.doc`
  - All transcripts combined  

- Copy all text to clipboard  

---

## 🛠️ Tech Stack

- HTML5  
- CSS3  
- JavaScript  
- Web Audio API  
- Groq API  
- Whisper (Speech-to-Text)  
- LLM (Dialogue formatting)  

---

## 🔑 API Setup

Replace API key:

```js
const API_KEY = "YOUR_GROQ_API_KEY";
```

⚠️ Do NOT expose your API key in public repos.

---

## 📦 Installation & Usage

### 1. Clone Repo

```bash
git clone https://github.com/your-username/call-transcript-tool.git
cd call-transcript-tool
```

---

### 2. Open

Just open:

```
index.html
```

No server needed.

---

### 3. Steps

1. Upload audio files  
2. Click "Start Transcription"  
3. Wait for processing  
4. Download results  

---

## ⚠️ Limitations

### Groq Free Tier
- ~7200 seconds/hour  
- Tool auto waits if limit reached  

### File Size
- API limit ~25MB  
- Auto compression enabled  

### Browser
- Works best on Chrome / Edge  

---

## 📌 Example Output

```
ग्राहक: हेलो!
कस्टमर सपोर्ट: नमस्ते सर, मैं जेसीबी राजस्थान मोटर्स से बोल रहा हूँ।
ग्राहक: मशीन के फिल्टर अभी तक नहीं बदले गए हैं।
कस्टमर सपोर्ट: कृपया चेसिस नंबर बताएं।
(पृष्ठभूमि में शोर)
ग्राहक: मैं गाँव में हूँ, अभी नंबर नहीं है।
```

---

## 🔮 Future Improvements

- Speaker auto-detection  
- Multi-language support  
- Dashboard & analytics  
- Backend for API security  

---

## 🤝 Contributing

1. Fork repo  
2. Create branch  
3. Commit  
4. Open PR  

---

## ⚖️ License

MIT License  

---

## 👨‍💻 Author

Anshu 🚀
