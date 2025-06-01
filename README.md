# Course Selling Application Backend

Welcome to the backend of your very own course selling platform! This server is your gateway to managing users, courses, and admin operations—all secured with robust token-based authentication.

## 🚀 Key Features

- **Token-Based Auth:** Every user and admin action is protected using JWT (JSON Web Tokens), ensuring secure access and data protection.
- **User Management:** Register, login, update profiles, and manage user data.
- **Course Operations:** Create, browse, update, and delete courses—perfect for educators and learners.
- **Admin Superpowers:** Admins can manage users, courses, and perform privileged actions.
- **RESTful API:** Clean, predictable endpoints for seamless integration with any frontend.

## 🔗 API Endpoints

| Route Prefix            | Description                  | Example Endpoints                  |
|------------------------|------------------------------|------------------------------------|
| `/api/v1/user`         | User registration & login    | `/api/v1/user/register`, `/login`  |
| `/api/v1/course`       | Course management            | `/api/v1/course/create`, `/list`   |
| `/api/v1/admin`        | Admin-only actions           | `/api/v1/admin/users`, `/courses`  |

**All sensitive endpoints require a valid JWT token in the request headers!**

## 🛠️ Getting Started

### Prerequisites

- **Node.js** (v14+ recommended)
- **npm** or **yarn**
- **MongoDB** (or your preferred database)
- **A sprinkle of curiosity!**

### Installation

1. **Clone the repo**
   ```bash
   git clone 
   cd 
   ```
2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
  
3. **Set up your environment**
   - Copy .env.example to .env
   - Fill in your secrets: DB_URI, JWT_SECRET, etc.

### 🔥 Fire Up the Server

```bash
npm start
# or
yarn start
```
The server should now be running on http://localhost:3000 (or your configured port).

## 🔒 Security

- **Token-Based Authentication:** Every request to protected routes must include a valid JWT in the `Authorization` header.
- **Role-Based Access:** Admins enjoy extra privileges, while regular users can only perform permitted actions.

## 📚 API Documentation

Check out the [Postman Collection](#) or [Swagger UI](#) (if available) for detailed API specs and examples.

## 💡 Tips

- **Keep your JWT secret safe!** Never commit it to your repository.
- **Test your endpoints** using Postman or your favorite API client.

