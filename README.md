# 📝 To-Do App

A simple and efficient To-Do Application built using Node.js, Express.js, MongoDB, and Mongoose. Users can create, update, delete, and manage their daily tasks.

## 🚀 Features

- Create new tasks
- View all tasks
- Update task status
- Delete tasks
- Mark tasks as completed
- RESTful API architecture
- MongoDB database integration
- Error handling and validation

## 🛠️ Tech Stack

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose

### Tools
- Postman
- Git & GitHub
- VS Code

## 📂 Project Structure

```
todo-app/
│
├── controllers/
│   └── task.controller.js
│
├── models/
│   └── task.model.js
│
├── routes/
│   └── task.routes.js
│
├── config/
│   └── db.js
│
├── .env
├── server.js
├── package.json
└── README.md
```

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/your-username/todo-app.git
```

### Navigate to Project

```bash
cd todo-app
```

### Install Dependencies

```bash
npm install
```

### Configure Environment Variables

Create a `.env` file in the root directory:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
```

### Start Server

```bash
npm start
```

For development:

```bash
npm run dev
```

## 📌 API Endpoints

### Create Task

```http
POST /api/tasks
```

Request Body:

```json
{
  "title": "Learn Node.js"
}
```

### Get All Tasks

```http
GET /api/tasks
```

### Update Task

```http
PUT /api/tasks/:id
```

Request Body:

```json
{
  "completed": true
}
```

### Delete Task

```http
DELETE /api/tasks/:id
```

## 📊 Sample Task Schema

```javascript
const taskSchema = new mongoose.Schema({
  title: {
    type: String,
    required: true
  },
  completed: {
    type: Boolean,
    default: false
  }
}, {
  timestamps: true
});
```

## 🔒 Environment Variables

| Variable | Description |
|----------|-------------|
| PORT | Server Port |
| MONGODB_URI | MongoDB Connection String |

## 🎯 Future Improvements

- User Authentication (JWT)
- Task Categories
- Task Priority Levels
- Due Dates
- Search & Filter Tasks
- Frontend Integration (React)

## 👨‍💻 Author

Harsh Singh

## ⭐ Support

If you like this project, give it a star on GitHub.
