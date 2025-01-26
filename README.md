# PRISHA
AI-powered recruitment platform for resume analysis and candidate ranking.
## Setup Instructions

### Clone the Repository

To clone the repository, use the following command:

```bash
git clone https://github.com/nitish0shr/PRISHA.git
```

### Create Project Structure

Navigate into the cloned repository and create directories for the project:

```bash
cd PRISHA
mkdir frontend backend ai_models
```

This creates separate directories for the frontend, backend, and AI models.

### Navigate into the Project

You can now navigate into each directory to start setting up the respective components.

```bash
cd frontend
# or
cd backend
# or
cd ai_models
```

### Frontend Setup

To set up the frontend using React, navigate to the `frontend` directory and initialize a new React project:

```bash
cd frontend
npx create-react-app prisha-frontend
cd prisha-frontend
```

This will create a new React project in the `frontend` directory.

### Backend Setup

For the backend, navigate to the `backend` directory and set up a Python virtual environment and a FastAPI project:

```bash
cd ../backend
python3 -m venv venv
source venv/bin/activate
pip install fastapi uvicorn
```

Create a new file `main.py` with a basic FastAPI setup:

```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
def read_root():
    return {"Hello": "World"}
```

You can run the FastAPI server with:

```bash
uvicorn main:app --reload
```
