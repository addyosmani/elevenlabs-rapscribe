# Rapscribe 🎵

A React-based audio visualization application powered by ElevenLabs' Scribe model that helps you visualize audio tracks and their transcriptions with high accuracy.

## Features

- Audio visualization using React
- Speech-to-text transcription powered by ElevenLabs' Scribe model
  - Support for 99+ languages with excellent accuracy (< 5% word error rate) for 25+ languages
  - Smart speaker diarization
  - Word-level timestamps for accurate subtitles
  - Auto-tagging of sound events
  - Exceptional handling of high-speed vocals and complex rap lyrics
- Support for multiple audio tracks
- TypeScript support for enhanced type safety
- Modern build system using Vite
- Tailwind CSS for styling

## Demo Highlights

This project showcases ElevenLabs' Scribe model's impressive ability to transcribe extremely rapid speech, as demonstrated with Eminem's "Rap God" - a song notorious for its super-fast sections that exceed 6 words per second. Where many speech recognition systems fail with such challenging content, Scribe maintains high accuracy even with the most technically demanding vocal performances.

## Requirements

- ElevenLabs API key (Required for speech-to-text transcription)
- Supported audio formats for transcription (pre-recorded audio only, real-time transcription coming soon)

## Getting Started

1. Clone the repository:
```bash
git clone https://github.com/addyosmani/rapscribe.git
cd rapscribe
```

2. Install dependencies:
```bash
npm install
```

3. Configure environment variables:
```bash
cp .env.example .env
```
Edit `.env` and add your ElevenLabs API key:
```
ELEVENLABS_API_KEY=your-api-key-here
```

4. Start the development server:
```bash
npm run dev
```

## API Usage

The application uses ElevenLabs' Scribe model for speech-to-text transcription, which costs $0.40 per hour of transcribed audio. For more information about the API and its capabilities, visit the [ElevenLabs API documentation](https://elevenlabs.io/docs/api-reference/speech-to-text/convert).

## Tech Stack

- React
- TypeScript
- Vite
- Tailwind CSS
- ESLint for code quality

## Project Structure

- `/src` - Source code
  - `App.jsx` - Main application component
  - `AudioVisualizer.jsx` - Audio visualization component
  - `songs.ts` - Song configuration
- `/public` - Static assets including audio files

## License

MIT © [Addy Osmani](https://github.com/addyosmani)
