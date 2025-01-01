# Semantic Image Search Engine

This project leverages **PyTorch** and **OpenAI CLIP** for advanced text-based semantic image search capabilities. The backend is built using **FastAPI**, ensuring a robust and high-performance server, while the frontend is developed with **Next.js**, providing a seamless and responsive user experience.

![Demo](https://raw.githubusercontent.com/immanuel-peter/semantic-image-search/main/demo.png)

## Features

- Text-based semantic image search using OpenAI CLIP
- Frontend built with React (Next.js) and styled with Tailwind CSS
- Backend built with FastAPI and powered by PyTorch
- Preloaded random images for demonstration purposes

## Technologies Used

- **Backend**: FastAPI, PyTorch, Hugging Face Transformers
- **Frontend**: Next.js, Tailwind CSS, React
- **Other**: Node.js, Python, OpenAI CLIP

## Prerequisites

Before running the project, make sure you have the following installed:

- **Python 3.10+**: [Download](https://www.python.org/downloads/)
- **Node.js**: [Download](https://nodejs.org/)
- **Unsplash Developer Access Key** (optional, for fetching new random images): [Get Access Key](https://unsplash.com/developers)

## Installation

### Clone the Repo

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

### Backend Setup

1. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```
2. Create a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Start the FastAPI server:
   ```bash
   uvicorn call:app --reload
   ```
   By default, the server will run at `http://127.0.0.1:8000`.

### Frontend Setup

1.  Navigate to the frontend directory:
    ```bash
    cd frontend/semantic-image-search
    ```
2.  Install dependencies:
    ```bash
    npm install
    ```
3.  Start the development server:
    ```bash
    npm run dev
    ```
    The frontend will be available at `http://localhost:3000`.

## Using Different Images

If you’d like to use different images for the project:

1.  Replace the images in the `random-images` folder:
    - Use the provided script to fetch random images from Unsplash:
      ```bash
      python backend/get-random-images.py
      ```
      **Note**: You need an Unsplash Developer Access Key to use the script. Add it to the script by replacing the placeholder `ACCESS_KEY` with your access key.
2.  Alternatively, manually replace the images in the `random-images` folder with your own collection.

## Usage

1.  Open the frontend in your browser: `http://localhost:3000`.
2.  Search for images using text queries such as "beautiful sunset," "expansive ocean," or "snowy mountains."
3.  Results will display a set of images matching the query from the preloaded random dataset.
