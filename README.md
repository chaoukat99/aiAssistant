# OMAR CHAOUKAT - AI Assistant Avatar

An animated AI assistant with chat and voice capabilities, featuring a dynamic avatar that responds to interactions.

## Features

✨ **Animated Avatar**
- Robot emoji avatar with smooth animations
- Appears in random positions across the screen
- Talking animation when responding
- Visual wave effects during speech
- Click the avatar to move it to a new position

💬 **Chat Interface**
- Modern, sleek chat UI
- Real-time typing indicators
- Smooth message animations
- Auto-scrolling message history
- User and assistant message differentiation

🎤 **Voice Features**
- Text-to-Speech: Avatar speaks responses aloud
- Speech-to-Text: Use microphone button for voice input
- Recording indicator with pulse animation
- Browser-based voice recognition

🎨 **Visual Effects**
- Gradient backgrounds
- Floating particles animation
- Smooth transitions and animations
- Responsive design
- Glass-morphism effects

## How to Use

### Getting Started
1. Open `index.html` in a modern web browser
2. The avatar will greet you with a voice message
3. Click the avatar to make it jump to a new position

### Chat Interaction
- **Type**: Enter your message in the input field and press Enter or click send (➤)
- **Voice**: Click the microphone button (🎤) to use voice input
- The avatar will respond with dummy data and move to a new position
- Each response is spoken aloud using text-to-speech

### Dummy Responses
The assistant currently uses pre-defined responses about Omar Chaoukat including:
- Developer expertise and skills
- AI and technology focus
- Portfolio information
- Project capabilities

## Browser Compatibility

- **Recommended**: Chrome, Edge (best speech recognition support)
- **Text-to-Speech**: All modern browsers
- **Speech-to-Text**: Chrome, Edge, Safari (with webkit prefix)

## Future Backend Integration

The current implementation uses dummy data for responses. To integrate with a backend:

1. Replace the `getDummyResponse()` function with an API call
2. Add async/await for API requests
3. Handle loading states and error cases
4. Connect to your preferred backend (Node.js, Python, etc.)

Example API integration:
```javascript
async function getAIResponse(userMessage) {
    const response = await fetch('YOUR_API_ENDPOINT', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({ message: userMessage })
    });
    const data = await response.json();
    return data.response;
}
```

## Customization

### Change Avatar Emoji
Edit line with `avatar-face` class:
```javascript
avatarDiv.textContent = '🤖'; // Change to any emoji
```

### Modify Responses
Update the `dummyResponses` array with your own messages.

### Adjust Colors
Modify the CSS gradient values:
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Animation Speed
Change duration values in CSS animations and JavaScript timeouts.

## Technologies Used

- HTML5
- CSS3 (Animations, Gradients, Flexbox)
- Vanilla JavaScript
- Web Speech API (Speech Recognition & Synthesis)

---

**Created for Omar Chaoukat**
Ready for backend integration 🚀
