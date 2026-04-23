# Boipoka - MERN Server Side

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=json-web-tokens&logoColor=white)

**Backend API** for **Boipoka** — A modern book management platform for book enthusiasts.

## ✨ Features

- User authentication & authorization (JWT)
- Book CRUD operations
- User profile management
- Book review and rating system
- Search and filter books
- Wishlist / Reading list support
- Secure API with proper validation and error handling
- MongoDB with Mongoose ODM

## 🛠️ Tech Stack

- **Runtime:** Node.js + Express.js
- **Database:** MongoDB (Mongoose)
- **Authentication:** JWT (JSON Web Tokens)
- **Validation:** Joi / express-validator (recommended)
- **Others:** dotenv, cors, helmet, morgan, bcryptjs

## 📁 Project Structure

```bash
boipoka-mern-server-side/
├── config/
├── controllers/
├── middleware/
├── models/
├── routes/
├── utils/
├── .env.example
├── server.js
├── package.json
└── README.md
```

## 🚀 Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/blu3be3tle/boipoka-mern-server-side.git
cd boipoka-mern-server-side
```

### 2. Install dependencies
```bash
npm install
```

### 3. Environment Variables
Copy the example environment file and configure it:

```bash
cp .env.example .env
```

Add your credentials in `.env`:

```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/boipoka
JWT_SECRET=your_super_secret_jwt_key_here
JWT_EXPIRE=30d
NODE_ENV=development
```

### 4. Run the server

**Development mode:**
```bash
npm run dev
```

**Production mode:**
```bash
npm start
```

Server will run at `http://localhost:5000`

## 📡 API Endpoints

| Method | Endpoint              | Description                  |
|--------|-----------------------|------------------------------|
| POST   | `/api/auth/register`  | Register new user            |
| POST   | `/api/auth/login`     | User login                   |
| GET    | `/api/books`          | Get all books                |
| GET    | `/api/books/:id`      | Get single book              |
| POST   | `/api/books`          | Create new book (Admin)      |
| PUT    | `/api/books/:id`      | Update book                  |
| DELETE | `/api/books/:id`      | Delete book                  |
| POST   | `/api/reviews`        | Add review to a book         |

> Full API documentation will be available soon (Swagger recommended).

## 🧪 Scripts

```json
"scripts": {
  "start": "node server.js",
  "dev": "nodemon server.js"
}
```

## 🤝 Contributing

Contributions are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

**Made with ❤️ for book lovers**
