# Todo Application with FastAPI and PostgreSQL

## Project Overview
A backend Todo application using FastAPI, SQLAlchemy, and PostgreSQL.

## Setup Instructions

### Prerequisites
- Python 3.9+
- PostgreSQL
- pip

### Installation Steps
1. Clone the repository
2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Configure Database
- Update `DATABASE_URL` in `app/database.py` with your PostgreSQL credentials
- Create a database named `todoapp`

### Running the Application
```bash
uvicorn app.main:app --reload
```

### Running Tests
```bash
pytest tests/
```

### API Endpoints
- `POST /todos/`: Create a new todo
- `GET /todos/`: List all todos
- `GET /todos/{id}`: Get a specific todo
- `PUT /todos/{id}`: Update a todo
- `DELETE /todos/{id}`: Delete a todo

## Technologies Used
- FastAPI
- SQLAlchemy
- PostgreSQL
- Pydantic
- Pytest