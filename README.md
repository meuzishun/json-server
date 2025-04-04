# Mock Server with JSON Server

This project is a simple and reusable mock API powered by [`json-server`](https://www.npmjs.com/package/json-server). It's designed to quickly spin up a RESTful API for frontend development, testing, or prototyping.

## 🚀 Features

- Zero-setup mock API
- Supports GET, POST, PUT, PATCH, DELETE
- Reusable for any project

## 📦 Setup

1. **Install dependencies**:

```bash
npm install
```

2. **Start the mock server**:

```bash
npm run server
```

By default, the server runs at `http://localhost:3000/`.

## 🗂 Project Structure

```
json-server/
├── package.json
└── README.md
```

## ⚙️ Create Your Own `db.json`

Create a `db.json` file at the root of the project:

```json
{
  "users": [
    { "id": 1, "name": "Alice Johnson", "email": "alice@example.com" },
    { "id": 2, "name": "Bob Smith", "email": "bob@example.com" },
    { "id": 3, "name": "Charlie Rose", "email": "charlie@example.com" }
  ],
  "posts": [
    {
      "id": 1,
      "title": "Getting Started with JavaScript",
      "body": "JavaScript is a versatile language used on the web...",
      "userId": 1,
      "tags": [1, 2]
    },
    {
      "id": 2,
      "title": "Understanding React Hooks",
      "body": "Hooks let you use state and lifecycle methods in functional components...",
      "userId": 2,
      "tags": [2, 3]
    },
    {
      "id": 3,
      "title": "Tips for Writing Clean Code",
      "body": "Readable code is maintainable code...",
      "userId": 1,
      "tags": [4]
    }
  ],
  "comments": [
    { "id": 1, "postId": 1, "userId": 2, "body": "Great intro, thanks!" },
    { "id": 2, "postId": 1, "userId": 3, "body": "This was helpful." },
    {
      "id": 3,
      "postId": 2,
      "userId": 1,
      "body": "Hooks took me a while to get used to!"
    }
  ],
  "tags": [
    { "id": 1, "name": "JavaScript" },
    { "id": 2, "name": "Frontend" },
    { "id": 3, "name": "React" },
    { "id": 4, "name": "Best Practices" }
  ]
}
```

## 🧼 Git Ignore Note

This project adds `db.json` to `.gitignore` so you can use custom mock data for each project without polluting version control.

## 📄 License

MIT
