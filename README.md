
# 🎬 Movie Assistant Bot (AWS Lambda)

A LINE chatbot deployed on **AWS Lambda + API Gateway**, built with **Python + Flask + line-bot-sdk**.  
It fetches movie info (posters, ratings, box office, categories) and local weather so users can quickly plan a cinema trip.

---

## 🧱 Architecture

```
LINE Messaging API  →  API Gateway (HTTP API)  →  AWS Lambda (Python)
                                        ↘︎ CloudWatch Logs
```

- **Flask** handles routing (e.g., `/webhook` for LINE events).
- **serverless-wsgi** adapts Flask to Lambda.
- **API Gateway** exposes a public HTTPS endpoint for the LINE webhook.

---

## ✨ Features

- Movie search by title with posters, release date, and ratings
- Taipei/Global box office rankings
- Movie categories & upcoming releases
- Local weather snapshots
- Rich carousel/bubble messages (LINE Flex messages)
## 🖼 Screenshots

| Movie Info | Weather Info | Box Office | Categories |
|------------|--------------|------------|------------|
|<img width="828" height="1612" alt="1" src="https://github.com/user-attachments/assets/28ba3d30-b997-44e4-b4fc-9feb570371a0" /> | <img width="828" height="1792" alt="2" src="https://github.com/user-attachments/assets/47f6e253-0994-4ed0-a6ec-37999c47ec3b" /> | <img width="223" height="2048" alt="3" src="https://github.com/user-attachments/assets/1c1f417c-9621-4ab2-97c2-c41a38565133" /> | <img width="465" height="2048" alt="4" src="https://github.com/user-attachments/assets/3ced8078-fcde-4c34-98c9-9a72e3057fc1" />|

## 🚀 How It Works

1. **User Input**: Users can type a movie name, genre, or command (e.g., "電影", "天氣 台北市").
2. **API Integration**: The bot fetches real-time data from movie and weather APIs.
3. **LINE Messaging API**: Formats and sends rich messages with images, ratings, and details.

## 🛠 Tech Stack

- **Language**: Python
- **Framework**: Flask (for webhook handling)
- **API**: LINE Messaging API, movie data API, weather API
- **Database**: SQLite / MongoDB (optional for storing user preferences)

## 📦 Installation

```bash
# Clone the repo
git clone https://github.com/yourusername/movie-assistant-bot.git
cd movie-assistant-bot

# Install dependencies
pip install -r requirements.txt

# Run locally
python app.py
```

## 📜 License

MIT License
