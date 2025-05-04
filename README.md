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
    {
      "id": "u1",
      "name": "Alice Johnson",
      "email": "alice@example.com"
    },
    {
      "id": "u2",
      "name": "Bob Smith",
      "email": "bob@example.com"
    },
    {
      "id": "u3",
      "name": "Charlie Rose",
      "email": "charlie@example.com"
    }
  ],
  "posts": [
    {
      "id": "p1",
      "title": "Getting Started with JavaScript",
      "body": "JavaScript is a versatile language used on the web for both client-side and server-side development. It's known for its flexibility, dynamic typing, and integration with HTML and CSS. Beginners can start learning basic syntax, data types, and how to manipulate the DOM.",
      "userId": "u1",
      "tags": ["t1", "t2"]
    },
    {
      "id": "p2",
      "title": "Understanding React Hooks",
      "body": "Hooks let you use state and lifecycle methods in functional components, making React code cleaner and easier to maintain. The most commonly used hooks are useState and useEffect. They allow you to manage side effects and component state without writing class components.",
      "userId": "u2",
      "tags": ["t2", "t3"]
    },
    {
      "id": "p3",
      "title": "Tips for Writing Clean Code",
      "body": "Readable code is maintainable code, and it's a crucial part of professional development. Use meaningful names, keep functions short, and avoid deeply nested logic. Consistent formatting and comments where necessary can make your code easier for others (and future you) to understand.",
      "userId": "u1",
      "tags": ["t4"]
    }
  ],
  "comments": [
    {
      "id": "c1",
      "postId": "p1",
      "userId": "u2",
      "body": "Great intro, thanks!"
    },
    {
      "id": "c2",
      "postId": "p1",
      "userId": "u3",
      "body": "This was helpful."
    },
    {
      "id": "c3",
      "postId": "p2",
      "userId": "u1",
      "body": "Hooks took me a while to get used to!"
    }
  ],
  "tags": [
    {
      "id": "t1",
      "name": "JavaScript"
    },
    {
      "id": "t2",
      "name": "Frontend"
    },
    {
      "id": "t3",
      "name": "React"
    },
    {
      "id": "t4",
      "name": "Best Practices"
    }
  ]
}
```

## 🧼 Git Ignore Note

This project adds `db.json` to `.gitignore` so you can use custom mock data for each project without polluting version control.

## 📄 License

MIT
