
# 🎬 Movie Assistant Bot

A LINE chatbot that provides movie recommendations, showtimes, weather updates, and more!  
The bot integrates movie ratings, upcoming releases, and local theater listings, making it easy for users to plan their next cinema trip.

## 📌 Features

- **🎥 Movie Search**: Search for movies by title and view posters, ratings, and release dates.
- **📅 Upcoming Movies**: See what’s coming to theaters soon.
- **🏆 Box Office Rankings**: View current top movies in Taipei and beyond.
- **🌦 Weather Info**: Check weather forecasts before heading to the cinema.
- **🎯 Movie Categories**: Filter movies by genre such as Action, Adventure, Sci-Fi, Animation, and more.
- **🎬 Detailed Info**: Access detailed ratings, satisfaction scores, and theater showtimes.

## 🖼 Screenshots

| Movie Info | Weather Info | Box Office | Categories |
|------------|--------------|------------|------------|
| ![Movie Info](c6f2e405-9a67-444c-a6ed-90799edad0df.png) | ![Weather Info](6f8d9006-cb6d-492e-9984-e729dcc06738.png) | ![Box Office](2b99d7cc-b5a5-4f0d-ab0b-4e056f64c7e3.png) | ![Categories](2b944014-0829-4615-84e5-b06762640834.png) |

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
