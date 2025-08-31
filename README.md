# CLI YouTube Video Manager

A simple command-line interface (CLI) application for managing YouTube videos with local SQLite database storage.

## 🎯 Overview

This project is a Python-based CLI tool that allows users to manage their YouTube video collection locally. It provides basic CRUD (Create, Read, Update, Delete) operations for video entries, storing video names and timestamps in a SQLite database.

## ✨ Features

- **List Videos**: View all stored video entries
- **Add Video**: Add new videos with name and time information
- **Update Video**: Modify existing video details
- **Delete Video**: Remove videos from the database
- **Persistent Storage**: Data is stored in SQLite database (`youtube_videos.db`)

## 🚀 Getting Started

### Prerequisites

- Python 3.x
- No external dependencies required (uses built-in `sqlite3` module)

### Installation

1. Clone or download this repository
2. Navigate to the project directory
3. Run the application

```bash
python cli_note.py
```

## 📖 Usage

The application provides an interactive menu with the following options:

### 1. List Videos
Displays all videos currently stored in the database with their ID, name, and time.

### 2. Add a YouTube Video
Add a new video entry by providing:
- Video name
- Video time/timestamp

### 3. Update a YouTube Video Details
Modify an existing video by providing:
- Video ID (to identify which video to update)
- New video name
- New video time

### 4. Delete a YouTube Video
Remove a video from the database by providing its ID.

### 5. Exit the App
Close the application and save all changes.

## 🗄️ Database Schema

The application uses a SQLite database with the following table structure:

```sql
CREATE TABLE videos (
    id INTEGER PRIMARY KEY,
    name TEXT NOT NULL,
    time TEXT NOT NULL
);
```

- **id**: Unique identifier for each video (auto-incrementing)
- **name**: Name or title of the YouTube video
- **time**: Timestamp or duration of the video

## 📁 Project Structure

```
cli_note/
├── cli_note.py          # Main application file
├── youtube_videos.db    # SQLite database file
├── README.md            # This file
└── .git/                # Git repository
```

## 🔧 Technical Details

- **Language**: Python 3.x
- **Database**: SQLite3 (built-in)
- **Architecture**: Simple CLI with interactive menu
- **Data Persistence**: Local SQLite database file



## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

Created as a CLI project for managing YouTube video information locally.

---
