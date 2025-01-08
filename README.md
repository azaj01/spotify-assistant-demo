# Spotify Assistant Demo

This demo showcases a Spotify Assistant that helps users create Spotify playlists through pipecat.
The assistant uses services like Spotify API, Google LLM, Deepgram STT, and Cartesia TTS to provide a seamless experience.

## Features

- Authenticate with Spotify
- Create playlists based on mood, genre, artist or whatever comes to mind
- Start playback of generated playlists

## Requirements

- Python 3.8+
- Spotify Developer Account
- Google API Key
- Deepgram API Key
- Cartesia API Key

## Creating a Spotify App

To use the Spotify Assistant, you need to create a Spotify app to obtain a client ID and client secret. Follow these steps:

1. Go to the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/applications).
2. Log in with your Spotify account.
3. Click on "Create an App".
4. Fill in the required details such as the app name and description.
5. Click on "Create".
6. Once the app is created, you will find the client ID and client secret on the app's dashboard.

Make sure to add these credentials to your `.env` file as shown in the setup section.

## Setup

1. Clone the repository:

   ```sh
   git clone https://github.com/yourusername/spotify-assistant-demo.git
   cd spotify-assistant-demo
   ```

2. Create a virtual environment and activate it:

   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the dependencies:

   ```sh
   pip install -r requirements.txt
   ```

4. Copy the example environment file and rename it to `.env`:

   ```sh
   cp env.example .env
   ```

5. Open the `.env` file and enter your API keys and other environment variables:

   ```env
   SPOTIFY_CLIENT_ID=your_spotify_client_id
   SPOTIFY_CLIENT_SECRET=your_spotify_client_secret
   GOOGLE_API_KEY=your_google_api_key
   DEEPGRAM_API_KEY=your_deepgram_api_key
   CARTESIA_API_KEY=your_cartesia_api_key
   DAILY_API_KEY=your_daily_api_key
   DAILY_SAMPLE_ROOM=your_daily_room_url
   ```

## Running the Demo

1. Run the main script:

   ```sh
   python spotify-assistant.py
   ```

2. Follow the instructions in the terminal to authenticate with Spotify.

3. Interact with the assistant to create and manage your playlists.

## License

This project is licensed under the BSD 2-Clause License.
