# Frontend application

This repository contains the React/Vite client. The Django REST API is
maintained separately in `Phinehastephen/artisan_connect`.

Install dependencies and start the frontend development server from this
folder:

```powershell
npm install
npm run dev
```

Set `VITE_API_BASE_URL` in `.env.local` to the API base URL, for local
development:

```env
VITE_API_BASE_URL=http://127.0.0.1:8000/api/v1
```

Start the backend separately from its repository:

```powershell
git clone https://github.com/Phinehastephen/artisan_connect.git
cd artisan_connect
python backend/manage.py runserver
```

The backend must allow the frontend's origin in `CORS_ALLOWED_ORIGINS`. Build
and lint this frontend with `npm run build` and `npm run lint`.
