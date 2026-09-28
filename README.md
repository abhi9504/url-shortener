# 🔗 URL Shortener

A simple and efficient **URL Shortener Web Application** built with **Node.js, Express.js, MongoDB, Mongoose, and EJS**.

The application allows users to convert long URLs into short, shareable links. The generated short URL is stored in MongoDB and redirects users to the original URL when accessed.

---

## 📸 Project Preview

![URL Shortener](screenshots/url-shortener.png)
<img width="1910" height="955" alt="image" src="https://github.com/user-attachments/assets/2087ffad-f826-4af0-abab-7577fc763c1c" />


---

## ✨ Features

- 🔗 Shorten long URLs into compact links
- ⚡ Generate unique short URLs
- 🗄️ Store URL mappings using MongoDB
- 🔄 Redirect short URLs to the original URL
- 🎨 Clean and user-friendly interface
- 🖥️ Server-side rendering using EJS
- 📦 Organized MVC-style project structure
- 🔐 Secure MongoDB configuration using environment variables

---

## 🛠️ Tech Stack

**Backend**
- Node.js
- Express.js

**Database**
- MongoDB
- Mongoose

**Frontend**
- HTML
- CSS
- EJS

**Other**
- ShortID
- Nodemon
- dotenv

---

## 📂 Project Structure

```text
url-shortener/
│
├── Controllers/
│   └── url.js
│
├── Models/
│   └── Url.js
│
├── views/
│   └── index.ejs
│
├── screenshots/
│   └── url-shortener.png
│
├── .gitignore
├── package.json
├── package-lock.json
├── server.js
└── README.md
```

---

## ⚙️ Getting Started

Follow these steps to run the project locally.

### 1. Clone the repository

```bash
git clone https://github.com/abhi9504/url-shortener.git
```

### 2. Navigate to the project directory

```bash
cd url-shortener
```

### 3. Install dependencies

```bash
npm install
```

### 4. Configure environment variables

Create a `.env` file in the root directory:

```env
MONGO_URI=your_mongodb_connection_string
```

Replace `your_mongodb_connection_string` with your MongoDB connection string.

> ⚠️ Never commit your `.env` file or expose your database credentials publicly.

### 5. Start the application

Using Node.js:

```bash
npm start
```

Or using Nodemon:

```bash
nodemon server.js
```

### 6. Open the application

Open your browser and visit:

```text
http://localhost:1000
```

---

## 🔄 How It Works

```text
        User enters a long URL
                  ↓
        Express.js receives request
                  ↓
       Generate a unique short ID
                  ↓
        Store URL in MongoDB
                  ↓
        Return the short URL
                  ↓
       User opens the short URL
                  ↓
     Redirect to the original URL
```

---

## 💡 Example

### Original URL

```text
https://www.example.com/some/very/long/url
```

### Short URL

```text
http://localhost:1000/abc123
```

When the short URL is opened, the application redirects the user to the original URL.

---

## 🗄️ Database

MongoDB is used to store the relationship between the original URL and its generated short identifier.

Example:

```text
Original URL  →  Short ID
Long URL      →  abc123
```

---

## 🔐 Environment Variables

The application uses environment variables to keep sensitive configuration secure.

The following file is excluded from Git:

```text
.env
```

The `node_modules` directory is also excluded:

```text
node_modules/
```

---

## 🚀 Future Improvements

Some features that can be added in future versions:

- 👤 User authentication
- 📊 URL click analytics
- 📈 Dashboard for URL statistics
- 🔗 Custom short URLs
- ⏳ URL expiration
- 📱 QR code generation
- 🌐 Production deployment
- 📋 Copy-to-clipboard functionality

---

## 👨‍💻 Author

### Abhishek Kumar

B.Tech Computer Science Engineering

GitHub: [@abhi9504](https://github.com/abhi9504)

---

## ⭐ Show Your Support

If you found this project useful or interesting, consider giving the repository a ⭐ on GitHub.

---

## 📄 License

This project is created for learning and portfolio purposes.
