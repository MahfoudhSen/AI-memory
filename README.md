# 🧠 ChatLog Vault

A minimalist web application for saving and organizing ChatGPT conversations with a design that resembles the ChatGPT interface.

## ✨ Features

### 🔐 Authentication
- **Local Authentication**: Simple sign up and login system
- **Secure Password Storage**: Passwords are hashed using SHA-256 before storage
- **Session Persistence**: Users stay logged in across browser sessions
- **Private Accounts**: Each user has their own isolated conversation storage

### 💬 Chat Management
- **Paste & Save**: Paste ChatGPT conversations and save them with custom titles
- **Auto-Title Generation**: Automatically generates titles from the first message if none provided
- **Smart Parsing**: Intelligently parses conversations with various formats:
  - `User:` or `You:` for user messages
  - `Assistant:`, `ChatGPT:`, or `AI:` for AI responses
- **ChatGPT-like Styling**: Messages are displayed with different styling for user and AI responses

### 📱 Dashboard & Organization
- **Conversation Dashboard**: Overview of all saved conversations
- **Sidebar Navigation**: Quick access to conversations with timestamps
- **Search & Filter**: Easy navigation through saved chats
- **Delete & Edit**: Manage conversations with delete and edit capabilities

### 🎨 User Interface
- **ChatGPT-like Design**: Familiar interface that mimics ChatGPT's layout
- **Dark Mode Support**: Toggle between light and dark themes
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Modern UI**: Clean, minimalist design with smooth animations

### 📋 Additional Features
- **Copy Functionality**: Copy entire chats or individual messages
- **Toast Notifications**: User-friendly feedback for all actions
- **Local Storage**: All data stored locally in the browser
- **No External Dependencies**: Pure HTML, CSS, and JavaScript

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No server setup required - runs entirely in the browser

### Installation
1. Download or clone the repository
2. Open `index.html` in your web browser
3. Create an account and start saving your ChatGPT conversations!

### Usage

#### Creating an Account
1. Open the application in your browser
2. Click "Don't have an account? Sign up"
3. Enter your email and password
4. Click "Create Account"

#### Saving a Chat
1. Log in to your account
2. Click "+ New Chat" in the sidebar
3. Optionally enter a title for your conversation
4. Paste your ChatGPT conversation in the text area
5. Click "Save Chat"

#### Viewing Saved Chats
1. Click on any conversation in the sidebar or dashboard
2. View the full conversation with ChatGPT-like styling
3. Use the copy button to copy the entire chat or individual messages

#### Managing Chats
- **Edit**: Click the "Edit" button to modify a saved conversation
- **Delete**: Click the "Delete" button to remove a conversation
- **Copy**: Use the "Copy Chat" button to copy the entire conversation

## 🏗️ Technical Details

### Tech Stack
- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Styling**: TailwindCSS (CDN)
- **Storage**: Browser localStorage
- **Security**: SHA-256 password hashing

### Data Structure
The application stores data in localStorage using the following structure:

```json
{
  "users": {
    "user@example.com": {
      "passwordHash": "hashed_password_here",
      "conversations": [
        {
          "id": "unique_chat_id",
          "title": "Chat Title",
          "date": "2025-01-02",
          "messages": [
            {
              "role": "user",
              "text": "User message content"
            },
            {
              "role": "ai",
              "text": "AI response content"
            }
          ]
        }
      ]
    }
  },
  "currentUser": "user@example.com",
  "darkMode": true
}
```

### Supported Chat Formats
The application can parse various chat formats:

```
User: How do I make pasta?
ChatGPT: Here's a simple recipe...

You: What's the weather like?
Assistant: I don't have access to real-time weather data...

User: Can you help me with coding?
AI: Of course! I'd be happy to help you with coding questions.
```

### Browser Compatibility
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## 🔒 Security & Privacy

### Local Storage
- All data is stored locally in your browser
- No data is sent to external servers
- Your conversations remain private and on your device

### Password Security
- Passwords are hashed using SHA-256 before storage
- No plain text passwords are ever stored
- Each user's data is isolated

### Data Privacy
- No analytics or tracking
- No external API calls
- Complete privacy and control over your data

## 🎯 Future Enhancements

Potential features for future versions:
- **Export/Import**: Backup and restore conversations
- **Search**: Search through saved conversations
- **Tags/Categories**: Organize conversations with tags
- **Cloud Sync**: Optional cloud storage integration
- **Rich Text**: Support for formatted text and code blocks
- **Conversation Templates**: Pre-defined conversation starters

## 🤝 Contributing

This is an MVP (Minimum Viable Product) designed to be simple and functional. Feel free to fork and modify for your own needs!

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Inspired by ChatGPT's clean and intuitive interface
- Built with modern web technologies for optimal performance
- Designed for simplicity and ease of use

---

**ChatLog Vault** - Keep your ChatGPT conversations organized and accessible! 🧠✨ 