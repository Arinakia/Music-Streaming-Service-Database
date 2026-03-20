# Music Streaming Service Database System

A relational database (MySQL) designed to manage a music streaming platform's core functionalities, including user subscriptions, artist registrations, album/song management, and user interactions like likes and playlists.

## Project Overview
This project provides the complete SQL schema and sample data for a music streaming backend. It handles complex many-to-many relationships such as songs having multiple genres and artists collaborating on albums.

## Database Schema
The database consists of 13 interconnected tables:

* **Users & Artists**: `Subscriber`, `Artist`, and `Artist_registration` for authentication and profile management.
* **Music Library**: `Song`, `Album`, `Genre` to store track details.
* **Relationships**: 
    * `Song_artist` & `Album_artist`: Mapping tracks and albums to their creators.
    * `Song_genre` & `Artist_genre`: Categorizing music by style.
* **User Activity**: `Likes` and `Playlist`/`Playlist_song` to track user preferences.


## Getting Started

### Prerequisites
* MySQL Server (v8.0+) or any SQL-compatible client (MySQL Workbench, DBeaver, etc.)

### Installation
1.  **Clone the repository**:
    ```bash
    git clone [https://github.com/YOUR_USERNAME/Music-Streaming-Database.git](https://github.com/YOUR_USERNAME/Music-Streaming-Database.git)
    ```
2.  **Create the Schema**:
    Run the `create_tables.sql` script to generate the tables and constraints.
3.  **Load Sample Data**:
    Run the `add_samples.sql` script to populate the database with artists like Eminem, Drake, Halsey, and Linkin Park, along with their songs and albums.

