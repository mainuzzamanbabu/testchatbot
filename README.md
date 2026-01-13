# Widget Test Page

This folder contains test files for the Central AI chatbot widget.

## Setup

1. **Start the Django server:**
   ```bash
   python manage.py runserver
   ```

2. **Get your Widget API Key:**
   - Log in to the Central AI dashboard
   - Go to **Widget** page in the sidebar
   - Copy your API key

3. **Update the test file:**
   - Open `index.html`
   - Replace `YOUR_API_KEY_HERE` with your actual API key
   ```javascript
   window.CentralAI = {
     apiKey: 'paste-your-api-key-here',
     ...
   };
   ```

4. **Open the test page:**
   - Simply open `index.html` in your browser
   - Or serve via Python: `python -m http.server 3000`
   - Then visit: http://localhost:3000

## Testing

1. The chat bubble should appear in the bottom-right corner
2. Click the bubble to open the chat panel
3. Enter your email to start chatting
4. Send messages and verify AI responses
5. Refresh the page - your chat history should persist

## Troubleshooting

- **"Widget API key is required"**: API key not configured
- **CORS errors**: Ensure Django server is running on localhost:8000
- **No response**: Check Django console for errors
