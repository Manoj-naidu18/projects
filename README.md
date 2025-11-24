# Career Guidance Platform

A comprehensive, AI-powered career guidance platform that helps students make informed decisions about their academic streams, courses, and college choices. This one-stop solution addresses the gap in awareness about graduation importance, career opportunities, and educational pathways.

## 🌟 Features

### 🧠 Intelligent Aptitude Assessment
- **Interactive Quiz**: 8-question assessment evaluating interests, strengths, and personality traits
- **AI-Driven Recommendations**: Smart algorithm suggests suitable academic streams (Science, Commerce, Arts)
- **Detailed Analysis**: Comprehensive scoring system with explanations for each recommendation

### 📚 Course Explorer
- **Stream-wise Navigation**: Explore courses across Science, Commerce, and Arts streams
- **Career Path Mapping**: Visual representation of career opportunities for each course
- **Detailed Information**: Duration, specializations, salary ranges, and higher studies options
- **Interactive Career Visualization**: See pathways from graduation to career success

### 🏛️ Government College Directory
- **Location-based Search**: Find colleges by state and city
- **Course Filtering**: Filter colleges by available courses
- **Detailed Information**: Fees, facilities, cut-offs, and contact details
- **Interactive Modals**: Rich college profiles with comprehensive information

### 📅 Academic Timeline
- **Admission Deadlines**: Important dates for college applications
- **Scholarship Information**: Deadlines and details for financial aid
- **Calendar Integration**: Add reminders to your personal calendar
- **Status Tracking**: Visual indicators for past, current, and upcoming events

### 🎯 Personalization
- **No Login Required**: Instant access without account creation
- **Local Storage**: Preferences saved locally for better experience
- **Responsive Design**: Perfect experience on desktop, tablet, and mobile
- **Progressive Enhancement**: Works even with slow internet connections

## 🚀 Getting Started

### Prerequisites
- Node.js (version 14 or higher)
- npm (comes with Node.js)

### Installation

1. **Navigate to the project directory:**
   ```bash
   cd Student-Assistance-Chatbot-main
   ```

2. **Install backend dependencies:**
   ```bash
   cd backend
   npm install
   ```

3. **Install frontend dependencies (optional for development):**
   ```bash
   cd ../frontend
   npm install
   ```

### Running the Application

#### Option 1: Quick Start (Recommended)

1. **Start the backend server:**
   ```bash
   cd backend
   npm start
   ```
   The backend API will be available at `http://localhost:5000`

2. **Open the frontend:**
   - Navigate to the `frontend` folder
   - Open `index.html` in your web browser
   - Or use a local server like Live Server (VS Code extension)

#### Option 2: Development Mode

1. **Start the backend in development mode:**
   ```bash
   cd backend
   npm run dev
   ```

2. **Start the frontend with live reload:**
   ```bash
   cd frontend
   npm start
   ```
   Frontend will be available at `http://localhost:3000`

## 📁 Project Structure

```
Student-Assistance-Chatbot-main/
├── backend/                    # Express.js API server
│   ├── data/                  # JSON database files
│   │   ├── quiz.json         # Quiz questions and scoring
│   │   ├── courses.json      # Course and career information
│   │   └── colleges.json     # College directory and timelines
│   ├── server.js             # Main server file
│   └── package.json          # Backend dependencies
├── frontend/                  # Static web application
│   ├── js/                   # JavaScript modules
│   │   ├── api.js           # API communication layer
│   │   ├── quiz.js          # Quiz functionality
│   │   ├── courses.js       # Course exploration
│   │   ├── colleges.js      # College directory
│   │   ├── timeline.js      # Academic timeline
│   │   └── main.js          # Main application logic
│   ├── styles/
│   │   └── main.css         # Comprehensive styling
│   ├── index.html           # Main HTML file
│   └── package.json         # Frontend dependencies
└── README.md               # This file
```

## 🎨 Technology Stack

### Backend
- **Node.js**: Runtime environment
- **Express.js**: Web application framework
- **CORS**: Cross-origin resource sharing
- **JSON**: File-based database for simplicity

### Frontend
- **HTML5**: Semantic markup
- **CSS3**: Modern styling with CSS Grid and Flexbox
- **Vanilla JavaScript**: No frameworks for maximum performance
- **Font Awesome**: Icons
- **Google Fonts**: Typography (Inter font family)

### Design Principles
- **Mobile-First**: Responsive design starting from mobile
- **Progressive Enhancement**: Core functionality works everywhere
- **Accessibility**: WCAG guidelines compliance
- **Performance**: Optimized for fast loading

## 🔧 Configuration

### API Configuration
The frontend connects to the backend API at `http://localhost:5000/api`. To change this:

1. Open `frontend/js/api.js`
2. Modify the `API_BASE_URL` constant
3. Ensure CORS is configured properly in the backend

### Adding Data
The application uses JSON files for data storage:

- **Quiz Questions**: Edit `backend/data/quiz.json`
- **Courses**: Edit `backend/data/courses.json`  
- **Colleges**: Edit `backend/data/colleges.json`

## 📱 Features Walkthrough

### 1. Home Page
- Welcome section with clear call-to-action
- Feature overview cards
- Statistics about the platform

### 2. Aptitude Quiz
- 8 carefully designed questions
- Multiple choice with weighted scoring
- Real-time progress tracking
- Comprehensive results with recommendations

### 3. Course Explorer
- Stream-based navigation (Science/Commerce/Arts)
- Detailed course cards with key information
- Career path visualization with interactive charts
- Links to related colleges and timelines

### 4. College Directory
- Advanced filtering by location and courses
- College cards with essential information
- Detailed modal views with comprehensive data
- Facilities overview and contact information

### 5. Academic Timeline
- Monthly view of admission processes
- Scholarship deadline tracking
- Interactive calendar integration
- Status indicators for time-sensitive events

## 🎯 Key Benefits

### For Students
- **Informed Decision Making**: Data-driven career guidance
- **Time Saving**: All information in one place
- **Cost Effective**: Focus on government colleges with quality education
- **Personalized**: Recommendations based on individual aptitude

### For Educational Institutions
- **Increased Enrollment**: Better awareness leads to more applications
- **Quality Students**: Matched students are more likely to succeed
- **Reduced Dropouts**: Students understand their chosen paths

### For Parents
- **Transparency**: Clear information about costs and opportunities
- **Guidance**: Help children make informed decisions
- **Peace of Mind**: Trust in government institution quality

## 🚀 Future Enhancements

### Planned Features
- **AI Integration**: More sophisticated recommendation algorithms
- **User Accounts**: Save progress and preferences
- **Mobile App**: Native iOS and Android applications
- **Chat Support**: Real-time guidance from counselors
- **Scholarship Matching**: Automated scholarship recommendations
- **College Comparison**: Side-by-side college comparison tool

### Technical Improvements
- **Database Migration**: Move from JSON to proper database (MongoDB/PostgreSQL)
- **Authentication**: JWT-based user authentication
- **Real-time Updates**: WebSocket for live data updates
- **PWA Features**: Offline functionality and push notifications
- **Analytics**: Usage tracking and performance monitoring

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📋 Testing

### Manual Testing Checklist
- [ ] Quiz completes successfully and shows results
- [ ] All stream tabs work in course explorer
- [ ] Career path visualization displays correctly
- [ ] College filtering works properly
- [ ] Timeline shows current month status correctly
- [ ] Mobile responsive design works
- [ ] All modals open and close properly
- [ ] API endpoints respond correctly

### Running Tests
```bash
# Backend API health check
curl http://localhost:5000/api/health

# Test quiz endpoint
curl http://localhost:5000/api/quiz

# Test courses endpoint
curl http://localhost:5000/api/courses
```

## 📞 Support

For support, feature requests, or bug reports:
- Create an issue on GitHub
- Email: support@example.com
- Documentation: Check this README and code comments

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- **Font Awesome** for the comprehensive icon library
- **Google Fonts** for the beautiful Inter typeface
- **Express.js** community for excellent documentation
- **Government Education Departments** for inspiration and data insights

---

**Made with ❤️ for students seeking better career guidance and educational opportunities.**