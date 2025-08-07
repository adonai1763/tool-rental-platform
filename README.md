# 🛠️ Tool Rental Platform

A comprehensive web application for tool rental services built with Django. This platform allows users to browse, book, and rent tools from a local rental business.

## 🌟 Features

### 🔐 User Authentication
- Custom user registration and login system
- Email-based authentication
- Secure password handling
- User dashboard with booking history

### 🛠️ Tool Management
- Browse tools by category (Construction, Gardening, Cleaning)
- Detailed tool information with real images
- Price per day display
- Availability status tracking

### 📅 Booking System
- Date-based booking with validation
- Automatic price calculation
- Booking status tracking (Pending, Confirmed, Cancelled)
- User booking management

### 📍 Pickup Location
- Integrated pickup location system
- Contact information and business hours
- Clear pickup instructions
- Location-based tool assignment

### 🎨 Modern UI/UX
- Responsive Bootstrap 5 design
- Professional landing page
- Mobile-friendly interface
- Intuitive navigation

## 🚀 Technologies Used

- **Backend**: Django 5.2.1, Python 3.13
- **Database**: SQLite (Development)
- **Frontend**: HTML5, CSS3, Bootstrap 5, JavaScript
- **Authentication**: Django's built-in authentication system
- **Image Handling**: Django ImageField with Pillow
- **Icons**: Bootstrap Icons

## 📁 Project Structure

```
tool_rental/
├── core/                          # Main Django app
│   ├── models.py                  # Database models
│   ├── views.py                   # View logic
│   ├── forms.py                   # Django forms
│   ├── urls.py                    # URL routing
│   ├── admin.py                   # Admin interface
│   ├── templates/core/            # HTML templates
│   └── management/commands/       # Custom Django commands
├── static/css/                    # Custom CSS styles
├── media/tools/                   # Tool images
├── tool_rental/                   # Django project settings
│   ├── settings.py               # Project configuration
│   └── urls.py                   # Main URL configuration
└── manage.py                     # Django management script
```

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.8+
- pip (Python package manager)

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/tool-rental-platform.git
cd tool-rental-platform
```

### 2. Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install django pillow
```

### 4. Database Setup
```bash
cd tool_rental
python manage.py makemigrations
python manage.py migrate
```

### 5. Create Sample Data
```bash
python manage.py create_sample_tools
python manage.py create_pickup_location
```

### 6. Create Superuser (Optional)
```bash
python manage.py createsuperuser
```

### 7. Run Development Server
```bash
python manage.py runserver
```

Visit `http://127.0.0.1:8000/` to view the application.

## 📱 Usage

### For Users:
1. **Browse Tools**: View available tools on the homepage
2. **Register/Login**: Create an account or log in
3. **Book Tools**: Select dates and book tools
4. **Manage Bookings**: View and cancel bookings in dashboard
5. **Pickup Information**: Check pickup location and hours

### For Administrators:
1. Access admin panel at `/admin/`
2. Manage tools, bookings, and pickup locations
3. View user accounts and booking statistics

## 🎯 Key Features Demonstrated

### Django Skills:
- **Models**: Custom user model, relationships, model validation
- **Views**: Function-based views, authentication decorators
- **Templates**: Template inheritance, context variables, forms
- **Forms**: Custom forms, validation, error handling
- **Admin**: Customized admin interface
- **URLs**: Clean URL patterns and routing

### Frontend Skills:
- **Responsive Design**: Mobile-first Bootstrap implementation
- **User Experience**: Intuitive navigation and clear CTAs
- **Visual Design**: Professional styling with custom CSS
- **Accessibility**: Proper form labels and semantic HTML

### Business Logic:
- **Authentication Flow**: Registration, login, logout
- **Booking System**: Date validation, price calculation
- **Data Relationships**: Users, tools, bookings, locations
- **Error Handling**: Form validation and user feedback

## 🖼️ Screenshots

### Homepage
- Hero section with value proposition
- Service features explanation
- Tool grid with real images
- How it works section

### Tool Detail Page
- Large tool image
- Detailed description
- Booking form with date selection
- Pickup location information

### User Dashboard
- Booking history
- Status tracking
- Quick actions

## 🔧 Management Commands

The project includes custom Django management commands:

```bash
# Create sample tools with images
python manage.py create_sample_tools

# Set up pickup location
python manage.py create_pickup_location

# Update specific tool images
python manage.py update_lawn_mower_image
python manage.py update_remaining_images
python manage.py update_all_tool_images
```

## 🚀 Deployment Considerations

For production deployment:
- Change `DEBUG = False` in settings.py
- Configure proper database (PostgreSQL recommended)
- Set up static file serving
- Configure media file handling
- Add proper security settings
- Set up environment variables for sensitive data

## 🤝 Contributing

This is a portfolio project, but suggestions and feedback are welcome!

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Developer

**Your Name**
- Portfolio: [Your Portfolio URL]
- LinkedIn: [Your LinkedIn]
- Email: [Your Email]

---

*This project was built to demonstrate full-stack web development skills using Django and modern web technologies.*
