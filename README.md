# 🤖 AI YouTube Shorts Automation

An automated pipeline that generates and uploads YouTube Shorts using **AI, n8n workflows, Docker, and FFmpeg**.

The system generates scripts, converts them to voice, creates subtitles, merges video and audio, generates metadata, and uploads the final video automatically.

---
Youtube:https://www.youtube.com/@FactActVibe
---
# 🚀 Features

• AI generated short video scripts
• Text-to-speech voice generation
• Automatic subtitle generation
• Random background video selection
• FFmpeg video processing
• Automated YouTube metadata generation
• Direct upload to YouTube
• Scheduled automation using n8n

---

# ⚙️ Tech Stack

* n8n
* Docker
* Google Gemini AI
* HuggingFace APIs
* FFmpeg
* YouTube Data API

---

# 🔄 Workflow Pipeline

1. Generate video script using AI
2. Convert script to speech (TTS)
3. Download generated audio
4. Select random background video
5. Merge audio and video using FFmpeg
6. Generate subtitles
7. Burn subtitles into video
8. Generate YouTube title, description, and tags
9. Upload automatically to YouTube

---

# 🐳 Running n8n with Docker

```bash
docker run -d \
 --name n8n \
 -p 5678:5678 \
 -v D:\n8n\Yt_Automation\audio:/home/node/audio \
 -v D:\n8n\Yt_Automation\videos:/home/node/videos \
 -v D:\n8n\Yt_Automation\images:/home/node/images \
 -v D:\n8n\Yt_Automation\subtitles:/home/node/subtitles \
 -v D:\n8n\Yt_Automation\temp:/home/node/temp \
 n8nio/n8n
```

Open:

```
http://localhost:5678
```

---

# 📥 Import Workflow

1. Open n8n
2. Click **Import Workflow**
3. Upload `workflow.json`
4. Configure API credentials

---

# 📂 Required Folder Mounts

```
/home/node/audio
/home/node/videos
/home/node/subtitles
/home/node/temp
```

---

# ⚠️ Setup Required

After importing the workflow configure:

• Google Gemini API
• YouTube OAuth credentials

---

# 👨‍💻 Author

Koushal
Computer Science Student | Automation Builder | AI Enthusiast
