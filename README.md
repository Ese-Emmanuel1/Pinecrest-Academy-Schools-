Pinecrest Academy - Official School Website
https://img.shields.io/badge/Pinecrest-Academy-blue
https://img.shields.io/badge/version-1.0.0-green
https://img.shields.io/badge/license-MIT-blue

A modern, responsive, and professional school website for Pinecrest Academy featuring student result portal, academic information, and school management system.

🌟 Live Demo
🔗 Live Website: https://ese-emmanuel1.github.io/pinecrest-academy/
🎯 Result Portal: https://ese-emmanuel1.github.io/pinecrest-academy/resultchecker.html

🎯 Features
📱 Core Features
🎓 Student Result Portal - Secure student result checking system with Supabase integration

📱 Responsive Design - Mobile-first approach with full mobile navigation

📚 Academic Information - Comprehensive school curriculum and programs

📝 Admissions Portal - Online application and enrollment system

🏫 School Management - Complete administrative functionality

🔧 Technical Features
⚡ Real-time Database - Supabase integration for student records

🔐 Secure Authentication - PIN-based student result access

🖨️ Print-Ready Reports - Academic reports with professional formatting

📊 Performance Analytics - Student performance tracking and analysis

🌐 Cross-platform - Works on all devices and browsers

📋 Table of Contents
Features

Installation

Database Structure

Usage

API Integration

Deployment

Contributing

License

Support

🚀 Quick Start
Clone & Run Locally
bash
# Clone the repository
git clone https://github.com/Ese-Emmanuel1/pinecrest-academy.git

# Navigate to project directory
cd pinecrest-academy

# Open in browser (No build needed - it's pure HTML/CSS/JS)
open index.html
Live Testing Credentials
JSS1 Student Test Account:

Student ID: SE0001MEC

PIN: 9087

Term: First Term

Year: 2026

SSS1 Student Test Account:

Student ID: SE0009MEC

PIN: 4087

Term: First Term

Year: 2026

📁 Project Structure
text
pinecrest-academy/
├── index.html                 # 🏠 Homepage
├── about.html                 # ℹ️ About page
├── academics.html             # 📚 Academics information
├── admission.html             # 📝 Admissions portal
├── resultchecker.html         # 🎓 Student result portal (MAIN FEATURE)
├── sport.html                 # ⚽ Sports activities
├── news.html                  # 📰 News and announcements
├── contact_us.html            # 📞 Contact information
├── gallery.html               # 📸 Photo gallery
├── assets/                    # 🎨 Assets folder
│   ├── css/                   # 🎨 Stylesheets
│   ├── js/                    # ⚡ JavaScript files
│   └── images/                # 🖼️ Images and icons
└── README.md                  # 📖 This documentation
🗄️ Database Structure
Supabase Tables Configuration
jss1 Table (Junior Secondary School 1)
sql
-- Example student record:
-- Student ID: SE0001MEC, PIN: 9087
-- Name: OSAYI JOHN
-- Maths: Test1=12, Test2=15, Exam=45
-- Total Score: 321, Grade: A
sss1 Table (Senior Secondary School 1)
sql
-- Example student record:
-- Student ID: SE0009MEC, PIN: 4087
-- Name: OASRO ISSAC
-- Maths: Test1=12, Test2=15, Exam=45
-- Total Score: 321, Grade: A
🔌 API Integration
Supabase Configuration
javascript
// Supabase Client Setup
const SUPABASE_URL = 'https://efiruwfplizcbrtgaajs.supabase.co'
const SUPABASE_KEY = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...'
const supabase = createClient(SUPABASE_URL, SUPABASE_KEY)
Fetching Student Results
javascript
// Example: Fetch JSS1 student result
const result = await supabase
  .from('jss1')
  .select('*')
  .eq('id', 'SE0001MEC')
  .eq('pin', '9087')
  .eq('term', 1)
  .eq('year', 2026)
  .single()
📱 How to Use
For Students (Result Checking)
Navigate to the Result Portal page

Enter your Student ID (e.g., SE0001MEC)

Enter your assigned PIN

Select the academic term (First, Second, Third)

Select the academic year

Click "Check My Result"

View and print your academic report

For Teachers/Administrators
Access the student database via Supabase

Add/Update student records and scores

Generate class performance reports

Monitor student academic progress

🎨 Design System
Color Scheme
css
/* Primary Colors */
--pinecrest-blue: #1a5fb4;     /* Main brand color */
--accent-blue: #1c71d8;        /* Secondary blue */
--light-blue: #e3f2fd;         /* Background color */
--success-green: #2ecc71;      /* Success/Actions */
Typography
Primary: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif

Headings: 'Playfair Display', serif

Accent: 'Poppins', sans-serif

🔒 Security Features
PIN-based Authentication - Each student has unique access

Secure Database - Supabase Row Level Security

HTTPS Encryption - All data transmitted securely

Input Validation - Client-side form validation

No Sensitive Data Storage - Only academic records

🌐 Browser Compatibility
Browser	Status	Notes
Chrome	✅ Full	Recommended
Firefox	✅ Full	Recommended
Safari	✅ Full	Recommended
Edge	✅ Full	Recommended
Mobile	✅ Full	Fully responsive
🚀 Deployment
GitHub Pages Deployment (Current)
Push code to GitHub repository

Go to Repository Settings → Pages

Select Source: main branch, / (root) folder

Save and your site is live at: https://ese-emmanuel1.github.io/pinecrest-academy/
