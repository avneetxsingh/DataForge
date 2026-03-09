# DataForge: AI Training Data Collection Platform

> A robust web application for collecting, managing, and visualizing training data for AI models

![Language](https://img.shields.io/badge/Python-63.7%25-blue)
![HTML](https://img.shields.io/badge/HTML-24.7%25-orange)
![CSS](https://img.shields.io/badge/CSS-9.0%25-purple)
![JavaScript](https://img.shields.io/badge/JavaScript-2.6%25-yellow)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

---

## 📋 Overview

**DataForge** is a Django-powered web application designed to streamline the collection and management of training data for AI/ML models. It provides an intuitive interface for data annotation, user management, and comprehensive data visualization capabilities.

Whether you're building a machine learning pipeline, conducting research, or training custom AI models, DataForge simplifies the data collection workflow while maintaining security and data integrity.

### Key Features

- 🔐 **Secure User Authentication** - Role-based access control and session management
- 📊 **Data Visualization** - Interactive dashboards and analytics for collected data
- 🗂️ **Data Management** - Efficient organization, filtering, and export capabilities
- 🎯 **Intuitive Interface** - User-friendly design for seamless data annotation
- 📈 **Progress Tracking** - Monitor data collection metrics and project statistics

---

## 🏗️ Tech Stack

| Component | Technology |
|-----------|-----------|
| **Backend** | Python 3.x, Django |
| **Frontend** | HTML5, CSS3, JavaScript |
| **Database** | SQLite (default) / PostgreSQL (recommended for production) |
| **Authentication** | Django built-in auth system |

---

## 📦 Installation & Setup

### Prerequisites

- Python 3.8+
- pip (Python package manager)
- Virtual environment (recommended)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/avneetxsingh/AI-Data-Collection-Platform.git
   cd AI-Data-Collection-Platform
   ```

2. **Create and activate virtual environment**
   ```bash
   python -m venv venv
   
   # On Windows
   venv\Scripts\activate
   
   # On macOS/Linux
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure database**
   ```bash
   python manage.py migrate
   ```

5. **Create superuser (admin account)**
   ```bash
   python manage.py createsuperuser
   ```

6. **Run development server**
   ```bash
   python manage.py runserver
   ```

   Access the application at: `http://localhost:8000`

---

## 🚀 Usage

### Admin Dashboard
- Navigate to `/admin` to access the Django admin panel
- Manage users, permissions, and data collections
- Monitor system health and statistics

### Data Collection
- Users can create annotation tasks
- Submit collected and annotated data through the web interface
- Track completion status and project progress

### Data Visualization
- View analytics and trends in collected data
- Export datasets for further analysis
- Generate reports for stakeholder reviews

---

## 📁 Project Structure

```
AI-Data-Collection-Platform/
├── ques_answ/                 # Main Django application
│   ├── migrations/            # Database migrations
│   ├── templates/             # HTML templates
│   ├── static/               # CSS, JavaScript, images
│   ├── models.py             # Data models
│   ├── views.py              # View logic
│   ├── urls.py               # URL routing
│   └── admin.py              # Admin configurations
├── manage.py                  # Django management script
├── requirements.txt           # Python dependencies
└── README.md                  # This file
```

---

## 🔧 Configuration

### Environment Variables (Optional)

Create a `.env` file in the root directory:

```env
DEBUG=True
SECRET_KEY=your-secret-key-here
ALLOWED_HOSTS=localhost,127.0.0.1
DATABASE_URL=sqlite:///db.sqlite3
```

### Production Deployment

For production use:
1. Set `DEBUG=False`
2. Use PostgreSQL instead of SQLite
3. Configure proper `SECRET_KEY`
4. Set up HTTPS/SSL
5. Use a production WSGI server (Gunicorn, uWSGI)

---

## 📊 Database Models

The application includes models for:
- **User Profiles** - Extended user information and preferences
- **Data Collections** - Project and task management
- **Annotations** - User-submitted data and labels
- **Analytics** - Tracking and reporting data

---

## 🔐 Security Considerations

- Passwords are hashed using Django's default PBKDF2
- CSRF protection enabled on all forms
- SQL injection prevention through ORM
- Session-based authentication
- Recommend using HTTPS in production

---

## 🤝 Contributing

This is a sample/prototype project maintained for demonstration purposes. If you'd like to contribute improvements or report issues:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -m 'Add improvement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

---

## 📝 License

This project is provided as-is for educational and research purposes.

---

## ⚠️ Disclaimer

**This is a sample prototype** of a larger production system. The complete and up-to-date version is maintained in a confidential repository due to proprietary features and ongoing development.

**Limitations of this version:**
- May not reflect the latest features
- Some advanced functionality is not included
- Not recommended for direct production use
- Designed for demonstration and educational purposes

For production use cases or to access the full feature set, please contact the project maintainer.

---

## 👨‍💻 Author

**Avneet Singh**  
Created: July 11, 2023

---

## 📞 Support & Questions

For questions or issues related to this sample version, please open an issue on GitHub or contact the maintainer directly.

---

## 🎯 Roadmap & Future Enhancements

Planned features in the full version include:
- Advanced ML model integration
- Real-time collaboration features
- Enhanced analytics dashboard
- API endpoints for external integrations
- Mobile application
- Blockchain-based data verification

---

**Last Updated:** March 2026  
**Status:** Active Development (Private Repository)
