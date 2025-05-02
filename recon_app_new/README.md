# Detail Shop Tracker

This is a Flask-based web application for managing cars through a reconditioning and detail shop. The app provides features for user authentication, job management, inventory tracking, notes, purchase orders, and reporting.

## Features Implemented

- User login and role-based access control (admin, employee)
- Dashboard with summary stats and searchable units list
- Unit detail pages with job assignments, inventory check-in/out, notes, and images
- Job management with assignment and priority
- Purchase order creation and management
- Chat functionality between users
- Reports on units, jobs, and time tracking
- Admin user and service management
- Secure password hashing and verification supporting legacy and bcrypt hashes

## Setup Instructions

1. Clone the repository:
   ```
   git clone <repo-url>
   cd recon_app
   ```

2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Create a `.env` file in the `recon_app` directory with the following content (update with your database credentials):
   ```
   DB_USER=your_db_user
   DB_PASSWORD=your_db_password
   DB_HOST=your_db_host
   DB_PORT=your_db_port
   DB_NAME=your_db_name
   ```

4. Run the Flask app:
   ```
   python3 app.py
   ```

5. Access the app in your browser at `http://localhost:5001` (or the port specified in `app.py`).

## Notes

- The app uses a MySQL database. Ensure the database is accessible and the credentials in `.env` are correct.
- Passwords are stored using a legacy salted hash format or bcrypt.
- The app includes detailed debug logging for login and database operations.
- Templates use Tailwind CSS and Font Awesome for styling.

## Next Steps

- Add more comprehensive tests.
- Improve UI/UX with additional frontend enhancements.
- Implement additional features as per business requirements.

## Contact

For any questions or support, please contact the development team.

---
