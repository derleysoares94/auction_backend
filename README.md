```markdown
# 🏷️ Auction API - Django Backend

This is a RESTful API built with Django and Django REST Framework for an auction platform. It is designed to serve as the backend for a frontend application (e.g., built with React). The API handles user and company registrations, auction creation, bidding, and viewing of auctions.

## 🚀 Features

- 🔐 User and Company registration & authentication
- 🧑 Users:
  - View all active auctions
  - Place bids on auctions
- 🏢 Companies:
  - View all active auctions
  - Create auctions
  - Place bids

> Note: This project exposes only API endpoints. There is no frontend interface included.

---

## 🛠️ Technologies Used

- Python
- Django
- Django REST Framework
- PostgreSQL (or SQLite for development)

---

## 📦 Installation

1. **Clone the repository**

```bash
git clone https://github.com/derleysoares94/auction_backend.git
cd auction_backend
```

2. **Install dependencies**

```bash
pip install -r requirements.txt
```

3. **Configure the environment variables**

Create a `.env` file in the root directory with necessary environment variables like:

```env
SECRET_KEY=your_secret_key
DEBUG=True
ALLOWED_HOSTS=*
DATABASE_URL=sqlite:///db.sqlite3
```

4. **Run migrations**

```bash
python manage.py migrate
```

> JWT or token-based authentication required for protected endpoints.

---

## 🧑‍💻 Roles

### Users

- Can register and log in
- Can view all auctions
- Can place bids on any auction

### Companies

- Can register and log in
- Can view all auctions
- Can place bids on any auction
- Can create new auctions
