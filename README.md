# TheraConnect Chatbot

A professional, mobile-friendly mental health therapy chatbot with comprehensive crisis detection and natural language processing.

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Mobile](https://img.shields.io/badge/mobile-optimized-brightgreen)

## 🎯 Overview

TheraConnect is an intelligent chatbot designed for mental health therapy practices. It provides instant responses to common questions, detects crisis situations, and helps users navigate therapy services while maintaining a compassionate, professional tone.

## ✨ Key Features

### 🚨 Crisis Detection & Safety
- **Comprehensive keyword detection** for suicide ideation (60+ variations)
- **Depression symptom recognition** with supportive responses
- **Violence/weapon detection** for immediate emergency routing
- **Smart cooldown system** (10-minute intervals) to prevent crisis message spam
- **Immediate resource provision** - 988 Suicide & Crisis Lifeline, 911 emergency

### 🧠 Natural Language Processing
- **150+ keyword mappings** for natural conversation
- **Synonym recognition** understands multiple ways to ask the same question
- **Fuzzy matching algorithm** finds relevant responses even with typos or variations
- **Context-aware responses** tailored to specific mental health concerns

### 💬 Comprehensive FAQ System
**Services covered:**
- Therapy types (CBT, DBT, EMDR, etc.)
- Individual, couples, family, and child therapy
- Pricing and insurance information
- Appointment scheduling
- Office location and hours
- Telehealth options

**Mental health conditions addressed:**
- Anxiety and panic attacks
- Depression
- PTSD and trauma
- OCD
- ADHD
- Bipolar disorder
- Grief and loss
- Eating disorders
- Addiction

### 📱 Mobile-First Design
- **Fully responsive** - optimized for iPhone 12 and all mobile devices
- **Full-screen chat on mobile** for immersive experience
- **Touch-optimized** with proper tap targets and gestures
- **iOS-friendly** - 16px input font prevents auto-zoom
- **Body scroll prevention** when chat is open
- **Landscape mode support**

### ♿ Accessibility
- **ARIA labels** and semantic HTML
- **Keyboard navigation** support
- **Screen reader friendly**
- **Focus management** for better UX
- **High contrast** for readability

### 💾 User Experience
- **Message history** saved in localStorage
- **Typing indicators** for natural conversation flow
- **Timestamps** on all messages
- **Quick reply chips** for easy navigation
- **Smooth animations** and transitions
- **Clear history option** for privacy

## 🛠️ Technical Stack

- **Pure JavaScript** (ES6+) - No frameworks required
- **CSS3** with CSS variables for theming
- **HTML5** semantic markup
- **LocalStorage API** for chat history
- **Object-oriented architecture** for maintainability

## 📋 Installation

1. **Download the file:**
   ```bash
   # Clone or download theraconnect-chatbot.html
   ```

2. **Open in browser:**
   ```bash
   # Simply open the HTML file in any modern browser
   # No build process or dependencies required!
   ```

3. **Or integrate into existing site:**
   ```html
   <!-- Copy the entire file contents into your page -->
   <!-- Or include as iframe -->
   <iframe src="theraconnect-chatbot.html"></iframe>
   ```

## 🎨 Customization

### Change Brand Colors
```css
:root {
  --brand: #7c4bd2;        /* Primary purple */
  --brand-hover: #6a3bc0;  /* Darker purple for hover */
  --brand-light: #e9e3fb;  /* Light purple background */
}
```

### Add New Responses
```javascript
const RESPONSES = {
  "your keyword": "Your custom response here",
  // Add more...
}
```

### Modify Crisis Keywords
```javascript
const KEYWORDS = {
  suicide: [
    "your custom keyword",
    // Add more variations...
  ]
}
```

### Update Contact Information
Search and replace:
- Email: `hello@theraconnect.net`
- Phone: `(123) 456-7890`
- Address: `400 NW Gilman Blvd. #787 Issaquah, WA 98027`

## 📊 Chatbot Flow

```
User Opens Chat
    ↓
Empty Chat Window (No Auto-Messages)
    ↓
User Types Message
    ↓
    ├─→ Violence Keywords? → 911 Emergency Message
    ├─→ Suicide Keywords? → 988 Crisis Line Resources
    ├─→ Depression Keywords? → Supportive + Crisis Info
    ├─→ Synonym Match? → Relevant Response
    ├─→ Keyword Match? → Relevant Response
    └─→ No Match? → Fallback + Suggestions
    ↓
Quick Reply Chips Appear (After First Message)
```

## 🔒 Privacy & Security

- **No server communication** - All data stays on user's device
- **LocalStorage only** - No cookies or tracking
- **HIPAA-compliant messaging** recommended in responses
- **Clear history option** for user privacy
- **No personal data collection**

## 📱 Mobile Specifications

### Tested & Optimized For:
- iPhone 12/13/14/15 (390px)
- iPhone SE (375px)
- Android devices (360px - 480px)
- Tablets (portrait & landscape)

### Responsive Breakpoints:
- `max-width: 480px` - Full mobile optimization
- `max-width: 390px` - iPhone 12 specific tweaks
- `max-height: 480px` - Landscape orientation

## 🚀 Performance

- **Lightweight** - Single HTML file (~80KB)
- **Fast load** - No external dependencies
- **Instant responses** - No API calls
- **Smooth animations** - CSS transitions
- **Efficient storage** - Compressed JSON in localStorage

## 🧪 Browser Compatibility

| Browser | Version | Support |
|---------|---------|---------|
| Chrome | 90+ | ✅ Full |
| Firefox | 88+ | ✅ Full |
| Safari | 14+ | ✅ Full |
| Edge | 90+ | ✅ Full |
| Mobile Safari | iOS 14+ | ✅ Full |
| Chrome Mobile | Latest | ✅ Full |

## 📖 Usage Examples

### Common User Queries:

**Getting Started:**
- "Hi" / "Hello" / "I need help"
- "What services do you offer?"
- "How much does therapy cost?"

**Crisis Situations:**
- "I want to die" → 988 Crisis Resources
- "I have a gun" → 911 Emergency
- "I'm so depressed" → Supportive + Resources

**Booking & Logistics:**
- "How do I book an appointment?"
- "Do you take insurance?"
- "Where are you located?"

**Specific Concerns:**
- "I have anxiety"
- "PTSD treatment"
- "Couples therapy"

## 🔧 Configuration Options

### Timing Settings
```javascript
const CONFIG = {
  TYPING_DELAY_MS: 600,    // Bot typing indicator delay
  STORAGE_KEY: 'theraChat_v1'
}

const CRISIS_COOLDOWN_MS = 10 * 60 * 1000; // 10 minutes
```

### Quick Reply Chips
```javascript
const CHIPS = [
  { label: 'Start', key: 'greeting' },
  { label: 'Services', key: 'services' },
  // Customize labels and keys...
];
```

## 🎯 Use Cases

Perfect for:
- ✅ Mental health therapy practices
- ✅ Counseling centers
- ✅ Crisis hotline websites
- ✅ Telehealth platforms
- ✅ University counseling services
- ✅ Employee assistance programs (EAP)
- ✅ Mental health non-profits

## ⚠️ Limitations & Disclaimers

- **Not a replacement for professional help** - This is an informational chatbot
- **Limited AI** - Uses keyword matching, not true AI/ML
- **Requires manual updates** - Responses must be coded manually
- **No backend** - Cannot actually book appointments or process payments
- **Crisis detection not perfect** - Should not be sole crisis intervention tool

## 🚧 Future Enhancements

Potential additions:
- [ ] API integration for real appointment booking
- [ ] Multi-language support
- [ ] Voice input/output
- [ ] Analytics dashboard
- [ ] Machine learning for better responses
- [ ] Integration with CRM systems
- [ ] SMS/text message support
- [ ] Admin panel for response management

## 📄 License

MIT License - feel free to use and modify for your projects.

## 👥 Contributing

This is a standalone project, but suggestions and improvements are welcome!

## 📞 Support Resources Referenced

- **988 Suicide & Crisis Lifeline** - Available 24/7
- **911** - Emergency services
- **Crisis Text Line** - Text HELLO to 741741

## 🙏 Acknowledgments

Built with consideration for:
- Mental health best practices
- Crisis intervention protocols
- Accessibility guidelines (WCAG)
- Mobile-first design principles

---

## 📸 Screenshots

### Desktop View
- Clean, centered chat window
- Purple branding with modern UI
- Smooth animations and transitions

### Mobile View
- Full-screen immersive experience
- Touch-optimized buttons
- Prevents background scrolling

### Crisis Detection
- Red-highlighted crisis messages
- Clear emergency resources
- Supportive, non-judgmental tone

---

**Built with ❤️ for mental health support**

*Last Updated: 2025*
