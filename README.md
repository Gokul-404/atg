# Medical Authentication System 🔥

A Django-based authentication system for Patients and Doctors with **BOLD NEUBRUTALISM** design and exciting UI!

## Features

- **User Types**: Patient and Doctor
- **Custom User Model**: Extended Django user model with additional fields
- **Secure Authentication**: Login and Signup with password validation
- **Role-Based Dashboards**: Separate dashboards for Patients and Doctors
- **Profile Pictures**: Upload and display profile pictures
- **⚡ NEUBRUTALISM UI**: Bold, attention-grabbing design with thick borders, harsh shadows, and vibrant colors!
- **Exciting Animations**: Bouncing, wiggling, and popping elements everywhere!
- **Responsive Design**: Works on desktop, tablet, and mobile devices

## User Fields

- First Name
- Last Name
- Profile Picture (optional)
- Username
- Email
- Password (with confirmation check)
- User Type (Patient/Doctor)
- Address (Line 1, City, State, Pincode)

## Installation & Setup

1. **Ensure you have Python installed** (Python 3.8 or higher recommended)

2. **Install dependencies** (already done):
   ```bash
   pip install django pillow
   ```

3. **The database is already migrated**, but if you need to reset:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

4. **Create a superuser** (optional, for admin panel access):
   ```bash
   python manage.py createsuperuser
   ```

5. **Run the development server**:
   ```bash
   python manage.py runserver
   ```

6. **Access the application**:
   - Main page: http://127.0.0.1:8000/
   - Login: http://127.0.0.1:8000/accounts/login/
   - Signup: http://127.0.0.1:8000/accounts/signup/
   - Admin: http://127.0.0.1:8000/admin/

## Usage

### Sign Up
1. Navigate to the signup page
2. Fill in all required fields
3. Choose your user type (Patient or Doctor)
4. Upload a profile picture (optional)
5. Enter your password twice to confirm
6. Click "Create Account"
7. You'll be automatically logged in and redirected to your dashboard

### Login
1. Navigate to the login page
2. Enter your username and password
3. Click "Login"
4. You'll be redirected to your dashboard based on your user type

### Dashboards
- **Patient Dashboard**: Displays patient information with green accent colors
- **Doctor Dashboard**: Displays doctor information with blue accent colors
- Both dashboards show: Username, Email, Address, and Member Since date

## Project Structure

```
atg/
├── accounts/
│   ├── migrations/
│   ├── templates/
│   │   └── accounts/
│   │       ├── base.html
│   │       ├── signup.html
│   │       ├── login.html
│   │       ├── patient_dashboard.html
│   │       └── doctor_dashboard.html
│   ├── admin.py
│   ├── forms.py
│   ├── models.py
│   ├── urls.py
│   └── views.py
├── medicalauth/
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── media/
│   └── profile_pics/
├── db.sqlite3
├── manage.py
└── README.md
```

## UI Features - NEUBRUTALISM DESIGN! 🎨

### What is Neubrutalism?
A bold, unapologetic design style featuring:
- **Thick Black Borders** (5-8px solid black borders everywhere!)
- **Harsh Drop Shadows** (20px+ offset shadows for depth)
- **Vibrant Flat Colors** (Yellow #FFE951, Red #FF6B6B, Cyan #4ECDC4, Purple #A78BFA, etc.)
- **No Rounded Corners** (or minimal rounding)
- **Bold Typography** (Space Grotesk font, 900 weight, UPPERCASE)
- **Geometric Shapes** (squares, circles, triangles floating in background)

### Our Implementation:
- **Bright Yellow Background** (#FFE951) with floating geometric shapes
- **Brutal Cards**: White cards with 8px black borders and 20px harsh shadows
- **Exciting Animations**:
  - Cards that POP in with bounce effects
  - Icons that WIGGLE and ROTATE
  - Buttons that SLAM when clicked
  - Forms that SLIDE from the side
  - Errors that SHAKE to grab attention
- **Bold Interactions**:
  - Inputs that JUMP when focused (with yellow background)
  - Buttons that transform with shadow changes on hover
  - Cards that rotate on hover
- **Decorative Elements**: Lightning bolts ⚡, fire 🔥, hearts 💚, shapes everywhere!
- **Auto-hiding Messages**: Brutal notifications that slide in with rotation
- **Responsive Layout**: Still brutal on all screen sizes!

## Security Features

- Password confirmation validation
- CSRF protection
- Login required for dashboards
- User type verification (prevents patients from accessing doctor dashboard and vice versa)
- Django's built-in password hashing

## Technologies Used

- **Backend**: Django 5.2.7
- **Database**: SQLite (default)
- **Frontend**: HTML5, CSS3, JavaScript
- **Image Processing**: Pillow

## Notes for Internship Project

This project demonstrates:
- ✅ Django custom user model implementation
- ✅ Form validation and handling
- ✅ User authentication and authorization
- ✅ Role-based access control
- ✅ File upload handling (profile pictures)
- ✅ Template inheritance
- ✅ Modern UI/UX with animations
- ✅ RESTful URL patterns
- ✅ Django admin customization

## Future Enhancements (Optional)

- Email verification
- Password reset functionality
- User profile editing
- Additional dashboard features (appointments, medical records, etc.)
- Search and filter users in admin panel
- Two-factor authentication

## License

This project is created for educational purposes as part of a Python Django internship.
