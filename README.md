# Learning-Log 📚

**Your personal knowledge companion for capturing and organizing learnings from books**

A beautiful, modern web application that helps you take notes from books using voice recording (English & Hindi) or manual typing. All your data is stored locally in your browser, with the ability to export to PDF.

![Learning-Log](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## ✨ Features

### 📖 Book Management
- ✅ Add and manage multiple books
- ✅ Edit book names
- ✅ Delete books with confirmation
- ✅ View note count per book
- ✅ Beautiful, intuitive interface

### 🎤 Voice Recording (Speech-to-Text)
- ✅ **English** voice recognition (`en-IN`)
- ✅ **Hindi (हिंदी)** voice recognition (`hi-IN`) with Devanagari script
- ✅ Real-time transcription
- ✅ Pause/Resume during recording
- ✅ Recording timer
- ✅ Review and edit before saving
- ✅ Re-record option

### ⌨️ Manual Typing
- ✅ Type notes in English or Hindi
- ✅ Character count display
- ✅ Auto-save drafts every 2 seconds
- ✅ Full editing capabilities
- ✅ Proper font support for Devanagari script

### 📝 Note Management
- ✅ Auto-numbered notes per book
- ✅ Timestamps (formatted as "Jan 12, 2026 at 2:30 PM")
- ✅ Language badges (English/हिंदी)
- ✅ Click to expand/collapse notes
- ✅ Edit existing notes
- ✅ Delete notes with confirmation
- ✅ Search notes within books
- ✅ Sort by newest/oldest

### 💾 Data & Export
- ✅ All data stored in browser localStorage
- ✅ **Export to PDF** with beautiful formatting
- ✅ Offline-capable (no internet needed)
- ✅ Data persists across sessions

### 🎨 Design
- ✅ Modern, attractive UI with purple gradients
- ✅ Responsive design (works on mobile, tablet, desktop)
- ✅ Smooth animations and transitions
- ✅ Clean, minimalist interface
- ✅ Dark purple theme with white accents

### ⌨️ Keyboard Shortcuts
- `Ctrl/Cmd + N` - Create new note (when book is selected)
- `Ctrl/Cmd + S` - Save note (when editing)
- `Esc` - Close modals
- `Enter` - Confirm in modals

## 🚀 Demo

**[Live Demo](https://yourusername.github.io/learning-log/)** ← Try it now!

## 📸 Screenshots

### Main Interface
Beautiful sidebar with books list and main content area with notes.

### Voice Recording
Record notes in English or Hindi with real-time transcription and recording timer.

### PDF Export
Export all your notes as a beautifully formatted PDF document.

## 🛠️ Installation & Setup

### Option 1: Use Directly (Recommended)
1. Visit the [Live Demo](https://yourusername.github.io/learning-log/)
2. Start adding books and notes!
3. Everything is saved in your browser

### Option 2: Run Locally
1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/learning-log.git
   cd learning-log
   ```

2. **Open in browser**
   - Simply open `index.html` in your web browser
   - Or use a local server:
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Python 2
   python -m SimpleHTTPServer 8000
   
   # Node.js (if you have http-server installed)
   npx http-server
   ```

3. **Visit** `http://localhost:8000`

### Option 3: Deploy to GitHub Pages

1. Fork this repository
2. Go to **Settings** → **Pages**
3. Select **main** branch and **root** folder
4. Click **Save**
5. Your app will be live at `https://yourusername.github.io/learning-log/`

## 📖 How to Use

### Adding a Book
1. Click **"+ Add Book"** in the left sidebar
2. Enter the book name
3. Click **"Add Book"**

### Creating a Note

#### Voice Recording:
1. Select a book from the sidebar
2. Click **"New Note"**
3. Choose **"Record"**
4. Make sure the correct language is selected (English/हिंदी)
5. Click **"Start Recording"**
6. Speak clearly into your microphone
7. Use **Pause/Resume** as needed
8. Click **"Stop Recording"** when done
9. Review and edit the transcription
10. Click **"Save Note"**

#### Manual Typing:
1. Select a book from the sidebar
2. Click **"New Note"**
3. Choose **"Type"**
4. Type your note (use Hindi keyboard for Hindi)
5. Click **"Save Note"**

### Managing Notes
- **Expand**: Click on any note to see full text
- **Edit**: Click the "Edit" button in expanded note
- **Delete**: Click the "Delete" button in expanded note
- **Search**: Use the search box to filter notes
- **Sort**: Use the dropdown to sort by newest/oldest

### Exporting to PDF
1. Click **"Export PDF"** in the header
2. A new window opens with formatted preview
3. The print dialog opens automatically
4. Select **"Save as PDF"**
5. Choose location and save

## 🌐 Browser Compatibility

| Feature | Chrome | Edge | Safari | Firefox |
|---------|--------|------|--------|---------|
| English Voice | ✅ | ✅ | ✅ | ⚠️ Limited |
| Hindi Voice | ✅ | ✅ | ❌ | ❌ |
| Manual Typing | ✅ | ✅ | ✅ | ✅ |
| PDF Export | ✅ | ✅ | ✅ | ✅ |

**Recommended**: Google Chrome for full Hindi speech recognition support.

**Note**: Hindi speech recognition works best on **Google Chrome** due to Web Speech API support.

## 💡 Tips & Best Practices

1. **For Hindi Voice Recording**: Use Google Chrome browser for best results
2. **Backup Regularly**: Export to PDF periodically to backup your notes
3. **Clear Microphone**: Speak clearly and in a quiet environment for better transcription
4. **Use Search**: When you have many notes, use the search feature to find specific content
5. **Edit After Recording**: Always review voice transcriptions and edit if needed
6. **Browser Data**: Don't clear browser data if you want to keep your notes (or export first)

## 🔧 Technical Details

### Built With
- **HTML5** - Structure
- **CSS3** - Styling with modern gradients and animations
- **Vanilla JavaScript** - No frameworks, pure JS
- **Web Speech API** - Voice recognition
- **localStorage API** - Data persistence
- **Google Fonts** - Inter & Noto Sans Devanagari

### Data Structure
```javascript
{
  books: [
    {
      id: "unique-id",
      name: "Book Title",
      notes: [
        {
          id: "note-id",
          serialNumber: 1,
          text: "Note content...",
          language: "en-IN" or "hi-IN",
          dateCreated: "ISO timestamp"
        }
      ],
      dateAdded: "ISO timestamp"
    }
  ]
}
```

### File Structure
```
learning-log/
├── index.html          # Main application (all-in-one file)
├── README.md           # This file
├── LICENSE             # MIT License
└── .gitignore          # Git ignore file
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** your changes (`git commit -m 'Add some AmazingFeature'`)
4. **Push** to the branch (`git push origin feature/AmazingFeature`)
5. **Open** a Pull Request

### Ideas for Contributions
- Add more languages (Spanish, French, etc.)
- Implement cloud sync (Google Drive, Dropbox)
- Add export to other formats (Word, Markdown)
- Implement tags/categories for notes
- Add dark mode
- Create mobile apps (React Native)

## 🐛 Bug Reports

Found a bug? Please [open an issue](https://github.com/yourusername/learning-log/issues) with:
- Browser and version
- Steps to reproduce
- Expected vs actual behavior
- Screenshots (if applicable)

## 📝 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- Website: [yourwebsite.com](https://yourwebsite.com)

## 🙏 Acknowledgments

- **Google Fonts** for Inter and Noto Sans Devanagari fonts
- **Web Speech API** for voice recognition capabilities
- **MDN Web Docs** for excellent documentation
- All contributors and users of this project

## 📞 Support

If you like this project, please consider:
- ⭐ Starring the repository
- 🐛 Reporting bugs
- 💡 Suggesting new features
- 🤝 Contributing code

---

**Made with ❤️ for lifelong learners**

*Last Updated: January 2026*
