# FoodLens App

Aplikasi untuk mendeteksi dan menganalisis makanan menggunakan teknologi AI.

## Struktur Project

```
FoodLens-App/
├── src/                    # Frontend source code
│   ├── styles/            # CSS files
│   ├── scripts/           # JavaScript files
│   ├── public/            # Static assets
│   └── index.html         # Main HTML file
├── backend/               # Backend API service
│   ├── index.js          # Main server file
│   ├── db.js             # Database configuration
│   └── package.json      # Backend dependencies
├── ml-api/               # Machine Learning API service
│   └── app/              # ML application code
├── package.json          # Frontend dependencies
├── vite.config.js        # Vite configuration
├── netlify.toml          # Netlify configuration
└── README.md            # Project documentation
```

## Setup dan Deployment

### Frontend (Netlify)
1. Install dependencies:
   ```bash
   npm install
   ```
2. Build project:
   ```bash
   npm run build
   ```
3. Deploy ke Netlify:
   - Connect repository ke Netlify
   - Build command: `npm run build`
   - Publish directory: `dist`

### Backend
1. Masuk ke direktori backend:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Setup environment variables
4. Jalankan server:
   ```bash
   npm start
   ```

### ML API
1. Masuk ke direktori ml-api:
   ```bash
   cd ml-api
   ```
2. Setup Python environment
3. Install dependencies
4. Jalankan API:
   ```bash
   python app/main.py
   ```

## Environment Variables

### Frontend (.env)
```
VITE_API_URL=http://localhost:3000
VITE_ML_API_URL=http://localhost:5000
```

### Backend (.env)
```
DATABASE_URL=postgresql://user:password@localhost:5432/foodlens
JWT_SECRET=your_jwt_secret
```

## Teknologi yang Digunakan
- Frontend: Vite, JavaScript
- Backend: Node.js, Express
- Database: PostgreSQL
- ML API: Python, TensorFlow
- Deployment: Netlify (Frontend) 