
# YouTube Video Assistant

This project creates a YouTube video assistant that allows users to interact with video content. The assistant uses Whisper for speech-to-text transcription, OpenAI models for question answering, and LangChain for connecting all components into a cohesive workflow.

## Purpose

The YouTube Video Assistant allows users to:

- Download audio from YouTube videos.
- Transcribe the video content using Whisper.
- Summarize the transcribed content.
- Chat with the bot to ask questions based on the video's content.

The assistant is designed to respond only based on the transcription or summary of the video, rejecting any questions that are not related to the video content.

## Key Features

- **Audio Download**: Extracts audio from YouTube videos using yt_dlp.
- **Speech-to-Text Transcription**: Uses Whisper to transcribe audio into text.
- **Text Summarization**: Summarizes the transcribed text to provide a concise summary.
- **Interactive Chatbot**: Allows users to ask questions related to the video, with answers based only on the transcript or summary of the video.

## Technologies Used

- **Whisper**: For transcribing audio to text.
- **yt_dlp**: For downloading YouTube video audio.
- **OpenAI**: For question answering based on the video content.
- **LangChain**: For creating and managing the logic of the chatbot.
- **Gradio**: For creating the interactive user interface.

## Definitions

- **Transcription**: The process of converting speech (from the YouTube video) into written text.
- **Summary**: A concise version of the transcribed text, highlighting the main points of the video.
- **VectorStore**: A storage system used to store the transcribed content and summaries. This enables efficient search and retrieval of relevant data for answering user questions.
- **Retriever**: A mechanism that fetches relevant content from the VectorStore based on user queries.
- **Chatbot**: A conversational agent that answers user questions based on the video content (transcript or summary).

## How It Works

1. **Audio Download**: Users provide a YouTube URL, and the audio from the video is downloaded and stored locally.
2. **Transcription**: The downloaded audio is passed to Whisper for transcription, converting speech to text.
3. **Summarization**: The transcribed text is processed to generate a summary of the video.
4. **Question Answering**: The chatbot is initialized to answer questions based on the transcribed or summarized text.

## Example Use

1. **User Inputs**: Provide a YouTube video URL in the Gradio interface.
2. **Processing**: The system will download the audio, transcribe it, and provide a summary.
3. **Interaction**: Users can ask questions related to the video's content, and the chatbot will provide answers based on the video’s transcript or summary.

## YouTube Video App

This is a project application file using the YouTube clips below.
https://drive.google.com/drive/folders/187v8u2yBEuL45k86RPbw5iZ-WeDlf8xU?usp=drive_link
1. **19 minute video clip**: https://www.youtube.com/watch?v=IvtZBUSplr4
2. **5 minute video clip** : https://www.youtube.com/watch?v=pjEpPj0f_PA
