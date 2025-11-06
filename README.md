# MBAA_6815_StudyGuide

A responsive web application for active recall practice and exam preparation.

## Features

✅ **Multiple Study Modes** - Adaptive, Multiple Choice, Open-ended, and Study modes  
✅ **Adaptive Learning** - Automatically adjusts difficulty based on your performance  
✅ **Multiple Choice** - Build confidence with 4-option questions  
✅ **Active Recall Testing** - Type answers for full memorization  
✅ **Study/Browse Mode** - Review all Q&A without pressure  
✅ **Weak Area Tracking** - Automatically flags questions you struggle with  
✅ **Mastery Progress** - Visual progress bar shows your improvement  
✅ **Module Selection** - Practice all modules or focus on specific ones  
✅ **Progress Persistence** - Your progress is saved in your browser  
✅ **Mobile Responsive** - Works on phones, tablets, and desktops  
✅ **Focus Mode** - Practice only your weak areas  

## Quick Start

### Option 1: Local File (Simplest)
1. Open `index.html` directly in your browser (double-click the file)
2. Start practicing!

### Option 2: Local Web Server (Recommended)
If you have Python installed:

```bash
# Navigate to the folder
cd c:\Users\willi\CascadeProjects\MBAA_6815

# Start a simple web server
python -m http.server 8000
```

Then open: `http://localhost:8000`

### Option 3: VS Code Live Server
1. Install "Live Server" extension in VS Code
2. Right-click `index.html` → "Open with Live Server"

## How to Use

### Study Modes Explained

#### 🎯 Adaptive Mode (Recommended)
The smart way to study! Starts with multiple choice for questions you haven't mastered, then switches to open-ended as you improve.
- **Hard questions** (never answered correctly): Multiple choice
- **Medium questions** (answered correctly once): Multiple choice
- **Easy questions** (answered correctly 2+ times): Open-ended recall

Perfect for building confidence while challenging yourself to truly memorize.

#### ✓ Multiple Choice Mode
All questions are multiple choice with 4 options. Great for:
- Initial learning and familiarization
- Building confidence before the exam
- Quick review sessions

#### ✍️ Open-ended Mode
Type your full answer before revealing the correct response. Best for:
- Final exam preparation
- Testing true recall ability
- Simulating actual exam conditions

#### 📚 Study Mode
Browse through all questions and answers without testing. Use this to:
- Get familiar with content initially
- Quick review before bed
- Navigate freely between questions

### Starting a Practice Session
1. **Select Study Mode**: Choose your preferred learning style
2. **Select Module(s)**: Choose "All Modules" or a specific module (1, 2, or 3)
3. **Click "Start Practice"**: Questions will be shuffled randomly
4. **Answer Questions**: Based on your selected mode
5. **Track Progress**: Watch your mastery bar grow!

### Tracking Progress
- **Total Questions**: All questions in the study guide (21)
- **Attempted**: Questions you've practiced at least once
- **Weak Areas**: Questions marked as "Need Review"

### Focus on Weak Areas
After completing a session:
1. Click "Focus on Weak Areas" button
2. Only questions you marked for review will appear
3. Practice until you master them all!

### Reset Progress
Click "Reset Progress" to clear all tracking data and start fresh.

## Data Structure

Questions are stored in `study-data.json`. To add/edit questions:

```json
{
  "modules": [
    {
      "id": 1,
      "name": "Module Name",
      "questions": [
        {
          "id": "unique-id",
          "question": "Question text?",
          "answer": "Answer text."
        }
      ]
    }
  ]
}
```

## Browser Compatibility

Works on all modern browsers:
- Chrome/Edge (recommended)
- Firefox
- Safari
- Mobile browsers

## Privacy

All data is stored locally in your browser using `localStorage`. Nothing is sent to any server.

## Tips for Exam Success

### Recommended Study Progression

**Week 1-2: Building Foundation**
1. Start with **Study Mode** to familiarize yourself with all content
2. Switch to **Multiple Choice Mode** to test basic recognition
3. Practice daily for 15-20 minutes

**Week 3-4: Building Confidence**
1. Use **Adaptive Mode** (default) - let the app guide your learning
2. Focus on weak areas after each session
3. Increase practice to 20-30 minutes daily

**Final Week: Exam Preparation**
1. Switch to **Open-ended Mode** exclusively
2. Practice under timed conditions (simulate exam pressure)
3. Review weak areas until mastery bar is full for all questions

### General Tips
1. **Practice Daily**: Regular short sessions beat cramming
2. **Focus on Weak Areas**: Use the tracking feature to identify gaps
3. **Write Full Answers**: Don't just think the answer, type it out
4. **Review Regularly**: Revisit questions you got right to reinforce memory
5. **Mix Modules**: Practice all modules together to simulate exam conditions
6. **Trust the Adaptive Mode**: It automatically adjusts to your skill level

## Troubleshooting

**Questions not loading?**
- Make sure `study-data.json` is in the same folder as `index.html`
- Check browser console for errors (F12)

**Progress not saving?**
- Ensure browser allows localStorage
- Check if you're in private/incognito mode (progress won't persist)

**Mobile display issues?**
- Try rotating your device
- Zoom out if text appears too large

## File Structure

```
MBAA_6815/
├── index.html          # Main application
├── study-data.json     # Question database
└── README.md          # This file
```

---

**Good luck with your exam! 🎓**
