# EduLearn - Mini E-Learning Platform

A beautiful, responsive mini e-learning platform built with HTML, CSS, and JavaScript. This single-page application allows users to browse courses, view detailed information, and track their learning progress.

PUBLISHED URL: https://claude.ai/public/artifacts/412cf5d8-0865-4680-9109-36c4cf18baf6


![Platform Preview](https://img.shields.io/badge/Status-Ready-brightgreen) ![License](https://img.shields.io/badge/License-MIT-blue)

## 🌟 Features

### Core Functionality
- **Course Catalog**: Display of 3 professionally designed courses
- **Course Details**: Click any course to view comprehensive information including:
  - Course overview
  - Learning topics
  - Duration and difficulty level
  - Requirements
- **Progress Tracking**: Visual progress bar showing completion percentage
- **Completion System**: Mark courses as complete with persistent state
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices

### User Interface
- Modern gradient design with smooth animations
- Interactive hover effects on course cards
- Modal popup for detailed course information
- Visual badges for completed courses
- Clean, intuitive navigation

## 📋 Course Offerings

1. **Introduction to Web Development** (8 weeks, Beginner)
   - HTML, CSS, and JavaScript fundamentals
   - Responsive web design
   - Web accessibility

2. **Python Programming Masterclass** (10 weeks, Intermediate)
   - Python syntax and fundamentals
   - Data structures and algorithms
   - Object-oriented programming

3. **Digital Marketing Essentials** (6 weeks, Beginner)
   - SEO and social media marketing
   - Content marketing strategies
   - Analytics and tracking

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, or Edge)
- No additional dependencies or installations required

### Installation

1. **Download the HTML file**
   - Save the complete HTML code as `index.html`

2. **Open in Browser**
   - Double-click the `index.html` file, or
   - Right-click and select "Open with" your preferred browser

3. **Alternative: Use a Local Server** (Optional)
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (with http-server)
   npx http-server
   ```
   Then navigate to `http://localhost:8000`

## 💻 Usage

### Browsing Courses
1. Upon loading, you'll see the main dashboard with 3 course cards
2. Each card displays:
   - Course icon
   - Title and description
   - Duration and difficulty level

### Viewing Course Details
1. Click on any course card to open the detailed view
2. Read through the course overview, topics, and requirements
3. Click the **×** button or click outside the modal to close

### Marking Courses as Complete
1. Open a course detail modal
2. Click the **"Mark as Complete"** button at the bottom
3. The course card will display a green "✓ Completed" badge
4. Your progress bar will update automatically
5. Completion status is saved for your current session

### Tracking Progress
- View your overall progress at the top of the dashboard
- The progress bar shows percentage of completed courses
- Text indicator shows "X out of 3 courses" completed

## 🎨 Customization

### Modifying Courses

To add, remove, or edit courses, locate the `courses` array in the JavaScript section:

```javascript
const courses = [
    {
        id: 1,
        title: "Your Course Title",
        description: "Course description here",
        duration: "X weeks",
        level: "Beginner/Intermediate/Advanced",
        icon: "🎯", // Any emoji
        completed: false,
        details: {
            overview: "Detailed overview...",
            topics: [
                "Topic 1",
                "Topic 2"
            ],
            requirements: "Prerequisites..."
        }
    },
    // Add more courses...
];
```

### Changing Colors

Update the CSS gradient colors in the `<style>` section:

```css
/* Main background gradient */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Button gradient */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Modifying Layout

Adjust the grid layout for course cards:

```css
.courses-grid {
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 25px;
}
```

## 🔧 Technical Details

### Technologies Used
- **HTML5**: Semantic structure
- **CSS3**: Modern styling with flexbox and grid
- **JavaScript (ES6+)**: Interactive functionality
- **SessionStorage**: Temporary data persistence

### Browser Compatibility
- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

### Data Persistence
- Course completion status is stored in `sessionStorage`
- Data persists during the browser session
- Clearing browser data will reset progress

## 📱 Responsive Breakpoints

- **Desktop**: 1200px and above
- **Tablet**: 768px - 1199px
- **Mobile**: Below 768px

The layout automatically adjusts for optimal viewing on all devices.

## 🛠️ Future Enhancements

Potential features for expansion:
- User authentication system
- Backend integration for data persistence
- Course categories and filtering
- Search functionality
- User ratings and reviews
- Video content integration
- Quiz and assessment features
- Certificate generation
- Multiple user profiles
- Course recommendations

## 📄 File Structure

```
elearning-platform/
│
├── index.html          # Complete application (HTML + CSS + JS)
└── README.md          # This file
```

## 🐛 Known Limitations

- No backend server (data stored locally in browser)
- Progress resets when browser data is cleared
- No user authentication
- Limited to 3 courses (easily expandable)
- No actual video/lesson content

## 🤝 Contributing

Feel free to fork this project and customize it for your needs. Some ideas:
- Add more courses
- Implement additional features
- Improve styling and animations
- Add accessibility features
- Create a backend API

## 📝 License

This project is open source and available under the MIT License.

## 👨‍💻 Author

Created as a mini e-learning platform prototype demonstrating modern web development practices.

## 📞 Support

For issues or questions:
- Review the code comments in `index.html`
- Check browser console for any error messages
- Ensure JavaScript is enabled in your browser

## 🎯 Quick Start Checklist

- [ ] Download the HTML file
- [ ] Open in web browser
- [ ] Click on a course to view details
- [ ] Mark a course as complete
- [ ] Check progress bar updates
- [ ] Test responsive design on mobile

---

**Enjoy your learning journey with EduLearn! 📚✨**
