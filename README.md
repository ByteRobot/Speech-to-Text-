
---

# ✅ Add FFmpeg to Windows PATH (Step-by-Step Guide)

### **1️⃣ Download FFmpeg**

Download the latest FFmpeg build for Windows from the official website:

🔗 **FFmpeg Official Download:**
[https://www.gyan.dev/ffmpeg/builds/](https://www.gyan.dev/ffmpeg/builds/)

Download the **Release full build (ffmpeg-*-full_build.zip)** and extract it.

---

### **2️⃣ Open Environment Variables**

Open Windows Search and type:

**Edit the system environment variables**

Then click the result to open the System Properties window.

---

### **3️⃣ Open the Environment Variables Panel**

At the bottom, click:

**Environment Variables…**

---

### **4️⃣ Edit the System PATH**

Under the **System variables** section:

* Select **Path**
* Click **Edit**

---

### **5️⃣ Add the FFmpeg Bin Folder**

Click **New** and paste the path to your FFmpeg `bin` directory:

```
C:\Users\user_name\ffmpeg\ffmpeg-2025-11-27-git-61b034a47c-full_build\bin
```

(Adjust the path if your folder name is different.)

---

### **6️⃣ Save Changes**

Click:

**OK → OK → OK**

to close all dialogs.

---

# ✨ Verify Installation

Open **PowerShell** or **Command Prompt** and run:

```
ffmpeg -version
```

If FFmpeg version information appears, the setup is complete.

---
# 📦 2. Required Python Libraries

Install the following dependencies to run the audio transcription script.

---

## **1. pydub**

Handles audio loading, conversion, and chunking.

```
pip install pydub
```

> Requires FFmpeg to be installed and added to PATH (steps above).

---

## **2. SpeechRecognition**

Used for converting speech to text via Google's speech API.

```
pip install SpeechRecognition
```

---

## **3. (Optional) PyAudio**

Only required if you plan to record audio from the microphone.
Not needed for file-based audio transcription.

```
pip install pyaudio
```

If it fails on Windows:

```
pip install pipwin
pipwin install pyaudio
```

---

## **4. Built-In Python Libraries**

These come with Python automatically:

* `os`

---

# 🚀 Quick Install Command

If you only need transcription from audio files:

```
pip install pydub SpeechRecognition
```

With microphone support:

```
pip install pydub SpeechRecognition pyaudio
```

---

