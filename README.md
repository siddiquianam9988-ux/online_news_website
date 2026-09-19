# online_news_website 
# NewsHub 📰

**NewsHub** is an Online News Website built with **Python, Flask, and SQLite**. It lets readers browse the latest news by category, search for articles, and read full stories. An admin can publish and manage news through a simple admin panel.

---

## ✨ Features

- **Latest News** — homepage shows the newest articles first.
- **Category Pages** — Sports, Politics, Tech, Entertainment, etc.
- **Article Page** — full news detail with image, date and author.
- **Search** — find news by keyword.
- **Admin Panel** — add, edit and delete news articles.
- **Admin Login** — only authorized admin can manage content.
- **Responsive Design** — works on mobile and desktop.

---

## 🛠 Tech Stack

| Component | Technology |
|-----------|------------|
| Backend | Python, Flask |
| Database | SQLite |
| Frontend | HTML, CSS (Jinja2 templates) |
| Image Storage | Local `static/uploads/` folder |

---

## 📁 Project Structure

```
news-website/
├── app.py                 # Main Flask application
├── database.db            # SQLite database (auto-generated)
├── requirements.txt       # Python dependencies
├── templates/
│   ├── base.html          # Common layout (navbar, footer)
│   ├── index.html         # Homepage
│   ├── category.html      # Category-wise news
│   ├── article.html       # Single article page
│   ├── login.html         # Admin login
│   └── admin.html         # Admin dashboard
└── static/
    ├── css/               # Stylesheets
    └── uploads/           # News images
```

---

## 🚀 Setup & Installation

**Requirement:** Python 3.9 or above.

**1. Clone the repository**
```
git clone https://github.com/siddiquianam9988-ux/news-website.git
cd news-website
```

**2. Create a virtual environment (recommended)**
```
python -m venv venv
venv\Scripts\activate        # Windows
source venv/bin/activate     # macOS/Linux
```

**3. Install dependencies**
```
pip install -r requirements.txt
```

**4. Run the app**
```
python app.py
```

**5. Open in browser**
```
http://127.0.0.1:5000
```

---

## 📖 How to Use

1. Open the homepage to read the latest news.
2. Click a category (Sports, Tech, etc.) to see news of that topic.
3. Click any headline to open the full article.
4. Use the search bar to find news by keyword.
5. For admin: go to `/login`, sign in, then add, edit or delete news from the dashboard.

---

## ⚙️ How It Works

1. **Admin adds news** through the admin panel (title, category, content, image).
2. **Flask** receives the form data and saves it in the **SQLite** database.
3. When a visitor opens the site, Flask fetches articles from the database.
4. **Jinja2 templates** render those articles into HTML pages.
5. **Search** runs a query on the database and shows matching articles.

---

## 🔮 Future Improvements

- Add user registration and login for readers.
- Add comments and likes on articles.
- Add bookmark / save-for-later option.
- Add pagination for long article lists.
- Fetch live news using a News API.
- Deploy on a cloud platform (Render, PythonAnywhere, etc.).
- Add dark mode.

---

## ⚠️ Notes

- `database.db` and uploaded images are generated at runtime and may be excluded from git via `.gitignore`.
- Change the default admin username and password before using the project publicly.
- This project is for learning purposes and is not production-ready.

---

## 👩‍🎓 Author

**Anam**
MCA (AI & ML) Student
Project — Online News Website (NewsHub)
GitHub: [siddiquianam9988-ux](https://github.com/siddiquianam9988-ux)
