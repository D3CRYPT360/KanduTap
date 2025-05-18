## Prerequisites

Before running the application, ensure you have the following installed:

- **Node.js** (v22.14.0 or higher)
- **Python** (v3.8 or higher)
- **npm** or **yarn** package manager

## Setup Instructions

### 1. Backend Setup (Flask)

1. Navigate to the Flask backend directory:

   ```bash
   cd flask_backend
   ```

2. Create a Python virtual environment (recommended):

   ```bash
   python -m venv venv
   ```

3. Activate the virtual environment:

   - Windows:
     ```bash
     venv\Scripts\activate
     ```
   - macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. Install the required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

5. Start the Flask backend server:
   ```bash
   python app.py
   ```
   The backend will run on http://localhost:5000 with Swagger documentation available at http://localhost:5000/api/docs

### 2. Frontend Setup (Next.js)

1. From the root directory, install the required Node.js packages:

   ```bash
   npm install
   # or
   yarn install
   ```

2. Start the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```
   The frontend will run on http://localhost:3000

## Database

The application uses SQLite for data storage. The database file (`kandutap.db`) is automatically created in the `flask_backend` directory when the backend is started for the first time.

## Notes

- Make sure both the frontend and backend are running simultaneously for the application to work properly.
- The backend includes test data that is automatically loaded when the database is first created.
- The frontend is configured to connect to the backend at http://localhost:5000.
- To test you can use the following test users: 11111, 12345, 67890
- Admin user login is: username: admin, password: root
