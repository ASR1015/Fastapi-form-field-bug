# FastAPI Form Field Metadata Bug

This repository demonstrates a bug in FastAPI where form field metadata (like `description`) is lost when using `Depends`.

## 🐛 Problem

When using `Form()` inside a dependency function with `Depends`, the metadata provided (e.g., `description`) does not appear in the OpenAPI schema.

## 📁 Files

- `form_dependency_test.py`: Demonstrates the issue using `Depends`
- `form_metadata_repro.py`: Shows correct behavior when not using `Depends`

## ▶️ How to Run

1. Install dependencies:
   ```bash
   pip install fastapi uvicorn
