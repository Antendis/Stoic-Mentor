# Stoic Mentor

An AI chatbot that lets you have conversations with Marcus Aurelius, the Roman Emperor and Stoic philosopher.

## About

This project creates an interactive experience where you can discuss philosophy, life challenges, and Stoic wisdom with an AI representation of Marcus Aurelius. The chatbot uses a hybrid approach combining rule-based responses, semantic understanding, and generative AI to provide thoughtful, historically-informed replies.

## Features

- Conversational AI powered by Llama-3.1-70B-Instruct
- Historically accurate personality based on Marcus Aurelius's writings and life
- Semantic search for contextually relevant responses
- Support for text and file attachments
- Persistent conversation history

## Tech Stack

**Frontend:** React + Vite  
**Backend:** Node.js + Express  
**Database:** MongoDB  
**AI:** Hugging Face Inference API

## Setup

### Prerequisites

- Node.js (v16 or higher)
- MongoDB connection string
- Hugging Face API key

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/Stoic-Mentor.git
cd Stoic-Mentor
```

2. Install dependencies
```bash
# Install client dependencies
cd Client
npm install

# Install server dependencies
cd ../Server
npm install
```

3. Configure environment variables

Create a `.env` file in the `Server` directory:
```
MONGODB_URI=your_mongodb_connection_string
HUGGINGFACE_API_KEY=your_huggingface_api_key
PORT=5000
```

4. Run the application
```bash
# Start the server (from Server directory)
npm run dev

# Start the client (from Client directory)
npm run dev
```

The client will run on `http://localhost:5173` and the server on `http://localhost:5000`.

## Architecture

The application uses a hybrid response system:
1. **Rule-based matching** for common queries
2. **Semantic search** for conceptually similar questions
3. **Generative AI** for open-ended conversations

This ensures fast, accurate responses while maintaining the philosophical depth and personality of Marcus Aurelius.