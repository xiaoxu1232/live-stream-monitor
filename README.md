# live-stream-monitor

> Monitor live streams and get notified when specific keywords are mentioned!

## ⭐ What This Does

- Monitor live streams 24/7
- Get INSTANT alerts when keywords you care about are mentioned
- Real-time speech transcription
- Multi-language support

## 💡 Solution

Monitor live streams and get INSTANT NOTIFICATIONS when keywords you care about are mentioned!

## ✨ Core Features

### 1. Keyword Alerts ⭐ CORE
- Set keywords you want to monitor
- Get notified IMMEDIATELY when keywords appear in transcription
- Multiple keywords support
- Real-time streaming transcription

### 2. Live Detection
- Monitor if streamer is live
- Auto-detect when stream starts/ends

### 3. Speech Transcription
- Real-time speech-to-text
- Multi-language support (English, Chinese, Japanese, etc.)
- Uses whisper.cpp (FREE, no API needed!)

## 🌐 Supported Platforms

- YouTube Live (https://youtube.com)
- Bilibili Live (https://live.bilibili.com)
- Twitch (https://twitch.tv)

## 🛠 Technical Stack

- **streamlink** - Grab live stream
- **ffmpeg** - Audio processing
- **whisper.cpp** - Local speech recognition (free!)

## 📖 Usage

### Set keyword alert
```
Monitor [keyword] on [stream URL]
Example: Monitor "discount" on https://youtube.com/watch?v=xxx
```

### Get transcription
```bash
# YouTube - 60 seconds
node monitor.js --monitor youtube VIDEO_ID "Channel Name" 60

# Bilibili
node monitor.js --monitor bilibili ROOM_ID "Streamer Name" 60
```

### Check live status
```bash
node monitor.js --check youtube VIDEO_ID
```

## 📝 Example

```
User: Monitor keyword "优惠" on this Bilibili stream
Agent: (starts monitoring)
Agent: ⭐ ALERT! Keyword "优惠" detected!
Transcription: "今天直播间有优惠活动..."
```

## ⏱ Latency

- **2-5 seconds** for keyword detection

## 🔧 Requirements

- Node.js
- streamlink
- ffmpeg
- whisper.cpp + model (small recommended for Chinese)

## 📄 License

MIT
