# Morocco Tours Website 🇲🇦

A beautiful website for booking and exploring tours across Morocco. Built with HTML/CSS/JavaScript frontend and Python Flask backend with MongoDB Atlas.

## Features

- 🗺️ Tour listings with detailed information
- 🏨 Tour packages and pricing
- 📱 Responsive design
- 🔍 Search and filter tours
- 💬 Contact form
- 🗄️ MongoDB database for tour data

## Project Structure

```
morocco-tours-website/
├── backend/
│   ├── app.py              # Flask application
│   ├── requirements.txt    # Python dependencies
│   ├── config.py           # Configuration settings
│   └── routes/
│       └── tours.py        # Tour API routes
├── frontend/
│   ├── index.html          # Home page
│   ├── tours.html          # Tours listing page
│   ├── tour-detail.html    # Individual tour page
│   ├── booking.html        # Booking page
│   ├── contact.html        # Contact page
│   ├── css/
│   │   └── style.css       # Main stylesheet
│   └── js/
│       └── script.js       # Main JavaScript
└── .gitignore
```

## Tech Stack

- **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
- **Backend:** Python Flask
- **Database:** MongoDB Atlas
- **API:** RESTful API

## Setup Instructions

### Backend Setup

1. **Install Python dependencies:**
   ```bash
   cd backend
   pip install -r requirements.txt
   ```

2. **Configure MongoDB:**
   - Create a MongoDB Atlas account at https://www.mongodb.com/cloud/atlas
   - Create a cluster and get your connection string
   - Update `config.py` with your MongoDB URI

3. **Run the Flask server:**
   ```bash
   python app.py
   ```
   Server will run on `http://localhost:5000`

### Frontend Setup

1. Open `frontend/index.html` in your browser
   - Or use a local server: `python -m http.server 8000`
   - Visit `http://localhost:8000`

## API Endpoints

- `GET /api/tours` - Get all tours
- `GET /api/tours/<id>` - Get tour details
- `POST /api/tours` - Create new tour (admin)
- `PUT /api/tours/<id>` - Update tour
- `DELETE /api/tours/<id>` - Delete tour

## Environment Variables

Create a `.env` file in the backend directory:

```
MONGODB_URI=your_mongodb_connection_string
FLASK_ENV=development
SECRET_KEY=your_secret_key
```

## Contributing

Feel free to fork, modify, and improve this project!

## License

MIT License

## Support

For issues or questions, please open a GitHub issue.

---

**Discover the beauty of Morocco! 🏜️🏔️🌊**
