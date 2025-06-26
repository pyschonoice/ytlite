
# 🎬 ytlite

A modern, full-stack YouTube clone built with the MERN stack, featuring video streaming, playlists, social interactions, and more. This project demonstrates a complete end-to-end application with a secure authentication system, cloud-based media management, and a responsive UI.
- [ytlite-backend](https://github.com/pyschonoice/ytlite-backend)
- [ytlite-frontend](https://github.com/pyschonoice/ytlite-frontend)


## Screenshots
![image](https://github.com/user-attachments/assets/9307af11-3765-4992-b96f-0c2637903a67)
![image](https://github.com/user-attachments/assets/a9bb4106-f52f-4743-b252-de2c94066104)

## ✨ Key Features

-   **🔐 Secure Authentication**: JWT-based authentication with access and refresh tokens stored in HttpOnly cookies.
-   **👤 User Profiles & Channels**: Customizable user profiles with avatars, cover images, and dedicated channel pages.
-   **📹 Video Management**: Upload, stream, edit, and delete videos. Includes view count, likes, and comments.
-   **📝 Social Posts (Tweets)**: Create, edit, and delete short text-based posts on your profile.
-   **▶️ Playlists**: Full CRUD functionality for creating and managing video playlists.
-   **👍 Social Interaction**: Like/unlike videos, subscribe/unsubscribe to channels, and comment on videos.
-   **📜 User Activity**: View your watch history and a list of all liked videos.
-   **☁️ Cloud Media Storage**: All media (videos, thumbnails, avatars) is handled by Multer and stored on Cloudinary.
-   **🚀 Responsive UI**: A clean and modern user interface built with Tailwind CSS and Shadcn/UI.

## 🛠️ Tech Stack

| Frontend                                                                                             | Backend                                                                                             |
| ---------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| [React](https://reactjs.org/)                                                                        | [Node.js](https://nodejs.org/)                                                                      |
| [Vite](https://vitejs.dev/)                                                                          | [Express.js](https://expressjs.com/)                                                                |
| [Tailwind CSS](https://tailwindcss.com/)                                                             | [MongoDB](https://www.mongodb.com/)                                                                 |
| [Shadcn/UI](https://ui.shadcn.com/)                                                                  | [Mongoose](https://mongoosejs.com/)                                                                 |
| [React Query](https://tanstack.com/query/latest)                                                     | [JWT (JSON Web Tokens)](https://jwt.io/)                                                            |
| [Axios](https://axios-http.com/)                                                                     | [Cloudinary](https://cloudinary.com/)                                                               |
| [React Hook Form](https://react-hook-form.com/) & [Zod](https://zod.dev/)                            | [Multer](https://github.com/expressjs/multer) & [Cookie Parser](https://github.com/expressjs/cookie-parser) |

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

-   [Node.js](https://nodejs.org/en/download/) (v18.x or higher recommended)
-   `npm` or `yarn`
-   A [MongoDB](https://www.mongodb.com/try/download/community) instance (local or a free Atlas cluster)
-   A [Cloudinary](https://cloudinary.com/users/register/free) account for media storage

### Installation

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/your-username/ytlite.git
    cd ytlite
    ```

2.  **Set up the Backend:**
    ```sh
    cd ytlite-backend
    npm install
    ```
    Create a `.env` file in the `ytlite-backend` directory and add the environment variables (see below).

3.  **Set up the Frontend:**
    ```sh
    cd ../ytlite-frontend
    npm install
    ```
    Create a `.env` file in the `ytlite-frontend` directory and add the environment variables.

### Environment Variables

You'll need to create `.env` files for both the frontend and backend.

**Backend (`ytlite-backend/.env`):**
```env
PORT=3005
MONGODB_URI=your_mongodb_connection_string
CORS_ORIGIN=http://localhost:5173
ACCESS_TOKEN_SECRET=your_strong_access_token_secret
ACCESS_TOKEN_EXPIRY=1d
REFRESH_TOKEN_SECRET=your_strong_refresh_token_secret
REFRESH_TOKEN_EXPIRY=10d

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

**Frontend (`ytlite-frontend/.env`):**
```env
VITE_BACKEND_URL=http://localhost:3005/api/v1
```

### Running the Application

1.  **Start the Backend Server:**
    ```sh
    # From the ytlite-backend directory
    npm run dev
    ```
    The backend should be running on `http://localhost:3005`.

2.  **Start the Frontend Development Server:**
    ```sh
    # From the ytlite-frontend directory
    npm run dev
    ```
    The frontend will be available at `http://localhost:5173`.


---
*Created with ❤️ by pyschonoice*
