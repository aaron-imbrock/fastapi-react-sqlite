# REACT and a FastAPI backend

Here I've built a Finance application made up of a REACT form and styled with Bootstrap.
The frontend is connected to a FastAPI backend that also uses SQLITE.

![Screenshot](./screenshot.png)

## Setup

```linux
git clone git@github.com:aaron-imbrock/fastapi-react-sqlite.git
cd fastapi-react-sqlite

# Python

python3 -m venv .venv
source .venv/bin/activate
pip install -r backend/requirements.txt

# React

cd frontend/finance-app
npm i
```

## Run

From the `fastapi-react-sqlite` folder:

Terminal A:

```linux
# Python
source .venv/bin/activate
cd backend/backend
uvicorn main:app --reload
```

Terminal B:

```linux
# REACT
cd frontend/finance-app
npm start
```

Swagger UI: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

Front End: [http://127.0.0.1:3000](http://127.0.0.1:3000)
