
# 🌐 Social Media Web App - MERN Stack

A full-stack social media application built with MongoDB, Express, React, and Node.js. Features include user authentication, posts, likes, follow/unfollow, and more!

## ✨ Features

- 🔐 User Authentication (JWT)
- 👤 User Profiles
- 📝 Create, Read, Update Posts
- ❤️ Like/Unlike Posts
- 👥 Follow/Unfollow Users
- 🖼️ Image Upload
- 📱 Responsive Design
- 🐳 Docker Support

## 🚀 Quick Start

### Prerequisites

- Node.js 16+ or Docker
- MongoDB Atlas account (or local MongoDB)

### Option 1: Run with Docker (Recommended)

```bash
# Clone the repository
git clone https://github.com/Mr-kashif/Socialmediaapp_Assignment.git
cd Socialmediaapp_Assignment

# Start with Docker Compose
docker-compose up -d

# Access the app
# Frontend: http://localhost
# Backend API: http://localhost/api
```

### Option 2: Run Locally

#### Backend Setup
```bash
cd Server
npm install
# Create .env file (see below)
npm start
```

#### Frontend Setup
```bash
cd client
npm install
npm start
```

## 🔧 Environment Variables

Create `Server/.env`:
```env
MONGO_DB=your_mongodb_connection_string
PORT=4000
JWT_KEY=your_secret_jwt_key
```

## 📦 Project Structure

```
├── client/                 # React Frontend
│   ├── src/
│   │   ├── Components/     # Reusable components
│   │   ├── Pages/          # Page components
│   │   ├── api/            # API calls
│   │   ├── actions/        # Redux actions
│   │   └── reducers/       # Redux reducers
│   ├── Dockerfile          # Frontend Docker config
│   └── nginx.conf          # Nginx configuration
│
├── Server/                 # Node.js Backend
│   ├── Controllers/        # Request handlers
│   ├── Models/             # Database models
│   ├── Routes/             # API routes
│   ├── Middleware/         # Custom middleware
│   ├── public/             # Static files
│   └── Dockerfile          # Backend Docker config
│
├── docker-compose.yml      # Docker Compose config
├── DEPLOYMENT.md           # Deployment guide
└── README.md               # This file
```

## 🌍 Deployment

See [DEPLOYMENT.md](./DEPLOYMENT.md) for complete AWS EC2 deployment instructions.

### Quick Deploy to EC2

```bash
# On EC2 instance
git clone https://github.com/Mr-kashif/Socialmediaapp_Assignment.git
cd Socialmediaapp_Assignment
docker-compose up -d
```

## 📡 API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user

### Users
- `GET /api/user/:id` - Get user by ID
- `PUT /api/user/:id` - Update user
- `GET /api/user` - Get all users
- `PUT /api/user/:id/follow` - Follow user
- `PUT /api/user/:id/unfollow` - Unfollow user

### Posts
- `GET /api/post/:id/timeline` - Get timeline posts
- `POST /api/post` - Create post
- `PUT /api/post/:id/like_dislike` - Like/Unlike post

### Upload
- `POST /api/upload` - Upload image

## 🛠️ Technologies Used

### Frontend
- React 18
- Redux (State Management)
- Axios (HTTP Client)
- React Router DOM
- CSS3

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- JWT Authentication
- Bcrypt (Password Hashing)
- Multer (File Upload)
- CORS

### DevOps
- Docker
- Docker Compose
- Nginx
- AWS EC2

## 👥 Usage

1. **Register/Login**: Create account or login
2. **Create Posts**: Share your thoughts with images
3. **Interact**: Like posts, follow users
4. **Profile**: Update your profile information

## 🐛 Troubleshooting

### Docker Issues
```bash
# View logs
docker-compose logs

# Rebuild containers
docker-compose down
docker-compose build
docker-compose up -d
```

### API Not Responding
- Check if backend container is running: `docker ps`
- View backend logs: `docker logs social-media-server`
- Ensure MongoDB connection string is correct

### Frontend Not Loading
- Clear browser cache
- Check nginx logs: `docker logs social-media-client`

## 📄 License

This project is open source and available under the MIT License.

## 👤 Author

**Muhammad Kashif**
- GitHub: [@Mr-kashif](https://github.com/Mr-kashif)

## 🙏 Acknowledgments

- MongoDB Atlas for database hosting
- AWS for cloud infrastructure
- Docker for containerization

---

**Made with ❤️ using MERN Stack** Web App

This project is a full-stack social media web application 🌐 that has been developed using the **MERN stack 🖥️** and **Rest API 🚀**, In this social media platform where you can share posts, like/unlike posts, Follow/Unfollow users and more.

## 🖥️ Technologies :
  
 **Frontend:**
 
- **React Js**
- **Material-Ui**
- **CSS**
- **React-Router-Dom**
- **Redux**

**Backend:**

- **Node JS**
- **Express Js**
- **MongoDB**
- **Rest API**
- **JWT Authentication**


## 🚀 Features :

- SignUp/Register Page.
- Login Page.
- Share New Post.
- Posts Include Text(Caption).
- Like/Unlike Posts.
- Suggested Users.
- Follow/Unfollow Users.
- View No Of Followers/Following Of User.
- View Other Posts By Follow Users And React On That Posts.
- Update/Edit Profile Page User Data.


### **SignUp/Register Page**  :

![SignUp](https://github.com/Faizan2911/Social-Media-Web-App-Mern-Stack-/assets/117813967/5b901509-12cc-4e6e-a4e7-ebc21b90a7f2)

### **Login Page**  :

![Login](https://github.com/Faizan2911/Social-Media-Web-App-Mern-Stack-/assets/117813967/4666edc8-5ae0-48b8-8570-9b16106d83ab)


### **Home Page :** 
 
![Home1](https://github.com/Faizan2911/Social-Media-Web-App-Mern-Stack-/assets/117813967/7ff2b394-b96d-4cba-8464-044ecda3076a)

![postShare](https://github.com/Faizan2911/Social-Media-Web-App-Mern-Stack-/assets/117813967/44eb4a60-a0fa-4d38-8991-a5dc405f2ee3)

![Home2](https://github.com/Faizan2911/Social-Media-Web-App-Mern-Stack-/assets/117813967/04ab0731-3e2d-40f5-8177-be234366a563)

### **User Profile Page**  :

![profilePage](https://github.com/Faizan2911/Social-Media-Web-App-Mern-Stack-/assets/117813967/e4ced6cd-e05d-4a19-8cc2-c952e2c80f3b)

![upateInfo](https://github.com/Faizan2911/Social-Media-Web-App-Mern-Stack-/assets/117813967/921938ac-e382-4ef5-b6dd-191b85bed1ca)

![pp2](https://github.com/Faizan2911/Social-Media-Web-App-Mern-Stack-/assets/117813967/6b2ad995-87f9-4698-ac58-7fc0baac81e1)

![pp3](https://github.com/Faizan2911/Social-Media-Web-App-Mern-Stack-/assets/117813967/315caa30-0009-4c36-bd60-05ac97cb64d1)





#### **What you need to run this application:**

 - Install NodeJs
 - MongoDB or MongoDB Atlas
 - Install Vs Code
 

#### **How to run this application**

- Make sure MongoDB is running on your system or online.
- Clone this repository
- Open command line in the cloned folder,
    - To install dependencies for frontend , run  `npm install` in `/client` folder.
    - To run frontend type command `npm start` in `/client` folder.
    - To install dependencies for backend, run  `npm install` in `/server` folder.
    - To run backend type command `nodemon` in server folder.
    