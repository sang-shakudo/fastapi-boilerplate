# FastAPI Template Project

This project is a FastAPI-based backend template using **uv** for virtual environment and dependency management.

---

## Prerequisites

- Python 3.11+
- `uv` installed  

```bash
pip install uv
```

---

## Initial Setup (Required)

After checking out the newly created project, you **must** run the following two steps.

### 1. Create Virtual Environment

```bash
uv venv
```

If prompted to overwrite the existing `.venv` directory, type **yes** and continue.

---

### 2. Install & Sync Dependencies

```bash
uv sync
```

This will install all required dependencies defined in the project.

---

## Running the Application

```bash
uv run uvicorn app.main:app --reload
```

- API: http://localhost:8000  
- Swagger UI: http://localhost:8000/docs  
- ReDoc: http://localhost:8000/redoc  

---

## Project Structure (Example)

```
.
├── app/
│   ├── main.py
│   ├── api/
│   ├── core/
│   └── models/
├── .venv/
├── pyproject.toml
└── README.md
```

---

## Notes

- Dependency versions are managed by `uv`
- Do not manually activate `.venv`; always use `uv run`

---
