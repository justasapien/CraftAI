# CraftAI - AI-Powered SaaS

CraftAI is a full-stack Software-as-a-Service (SaaS) application that leverages the power of multiple AI APIs to provide a suite of tools for content generation, image manipulation, and document analysis. The application features a secure, tiered subscription model, offering both free and premium plans to users.

## 🚀 Live Demo

You can view the live project here:

[![View Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20Now-brightgreen)](https://craft-ai-two.vercel.app/)

## ✨ Features

* **AI Content Generation**:
    * **Write Article**: Generate full-length articles from a simple prompt.
    * **Blog Titles**: Create catchy and SEO-friendly blog titles.
* **Advanced Image Manipulation**:
    * **Generate Images**: Create images from text descriptions using the Clipdrop API.
    * **Remove Background**: Automatically remove the background from any image.
    * **Remove Object**: Erase any unwanted object from an image by providing a text prompt.
* **Document Analysis**:
    * **Review Resume**: Upload a resume in PDF format and receive AI-powered constructive feedback.
* **User Management**:
    * **Secure Authentication**: Robust user sign-up, sign-in, and profile management handled by Clerk.
    * **Tiered Subscription Model**: A free plan with usage limits and a premium plan with unrestricted access to all features.
* **Community Hub**: A dedicated space for users to view and share AI-generated images.

## 🛠️ Tech Stack

| Category           | Technologies & Services                                                                                               |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------- |
| **Frontend** | React.js, React Router                                                                            |
| **Backend** | Node.js, Express.js                                                                               |
| **Database** | PostgreSQL                                                                                                   |
| **Authentication** | Clerk                                                                                                        |
| **AI Services** | Google Gemini API, Clipdrop API, Cloudinary AI                                           |
| **File Handling** | Multer, pdf-parse                                                                                 |

## 🚀 Getting Started

Follow these instructions to set up and run the project locally.

### Prerequisites

* Node.js (v18 or later)
* npm or yarn
* A PostgreSQL database
* API keys for:
    * Clerk (Publishable Key, Secret Key)
    * Google Gemini
    * Clipdrop
    * Cloudinary (Cloud Name, API Key, API Secret)

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/craft-ai.git](https://github.com/your-username/craft-ai.git)
    cd craft-ai
    ```

2.  **Install server dependencies:**
    ```bash
    cd server
    npm install
    ```

3.  **Set up server environment variables:**
    Create a `.env` file in the `server` directory and add the following variables:

    ```env
    PORT=3000

    # PostgreSQL Database Connection URL
    POSTGRES_URL="your_postgres_connection_url"

    # Clerk Authentication
    CLERK_PUBLISHABLE_KEY="your_clerk_publishable_key"
    CLERK_SECRET_KEY="your_clerk_secret_key"

    # AI & Cloud Services
    GEMINI_API_KEY="your_gemini_api_key"
    CLIPBOARD_API_KEY="your_clipboard_api_key"
    CLOUDINARY_CLOUD_NAME="your_cloudinary_cloud_name"
    CLOUDINARY_API_KEY="your_cloudinary_api_key"
    CLOUDINARY_API_SECRET="your_cloudinary_api_secret"
    ```

4.  **Install client dependencies:**
    ```bash
    cd ../client
    npm install
    ```

5.  **Set up client environment variables:**
    Create a `.env` file in the `client` directory and add your Clerk publishable key:

    ```env
    VITE_CLERK_PUBLISHABLE_KEY="your_clerk_publishable_key"
    ```

### Running the Application

1.  **Start the backend server:**
    From the `server` directory, run:
    ```bash
    npm run dev
    ```
    The server will start on `http://localhost:3000` (or the port you specified).

2.  **Start the frontend client:**
    From the `client` directory, run:
    ```bash
    npm run dev
    ```
    The React application will be available at `http://localhost:5173`.

## Contact

For any questions or suggestions, feel free to open an issue or contact me at [vikash.sharma.nsit@gmail.com](mailto:vikash.sharma.nsit@gmail.com).
