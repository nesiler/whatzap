# WhatZap - WhatsApp Media Downloader & Sender

WhatZap is an automation system that downloads media files (such as torrents, YouTube videos, or direct media links) and sends them as document files via WhatsApp Business Cloud API. The project enables users to efficiently transfer large video files (up to 2GB) over WhatsApp, making use of unlimited WhatsApp data plans.

## Features
- **WhatsApp Integration**: Uses WhatsApp Business Cloud API for sending media.
- **Torrent Support**: Downloads media files from torrent links.
- **YouTube Downloader**: Fetches and processes YouTube videos.
- **General Media Links**: Supports downloading files from direct links (wget/curl style).
- **File Splitting**: Uses ffmpeg to split large files (>2GB) for WhatsApp compatibility.
- **Live Logging**: Telegram bot integration for real-time logs.
- **Containerized**: Uses Docker for easy deployment.

## Getting Started

### Prerequisites
- A **VPS server** or local machine with Docker installed.
- A registered **WhatsApp Business API** account.
- Telegram bot credentials for logging (optional but recommended).

### Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/whatzap.git
   cd whatzap
   ```
2. Create an `.env` file for API credentials:
   ```sh
   cp .env.example .env
   ```
   - Add your WhatsApp Business API credentials.
   - Configure Telegram bot details for logging.

3. Build and run the project with Docker:
   ```sh
   docker-compose up --build -d
   ```

### Usage
- **Sending a torrent file:** Send `/torrent` along with a torrent file in WhatsApp.
- **Downloading a YouTube video:** Send `/yt <YouTube URL>`.
- **Downloading from a direct link:** Send `/link <file URL>`.

The bot will process the media and send it back as a WhatsApp document.

## Contributing
Contributions are welcome! Feel free to submit issues and pull requests.

## License
This project is licensed under the MIT License.

## Contact
For any inquiries, reach out via GitHub Issues or Telegram.

