# Hello API

A minimal FastAPI service with a health endpoint.

## Setup

Requires Python 3.12 and `uv`.

```sh
make setup
```

## Run the app

```sh
uv run uvicorn app.main:app --port 8001
```

Then request `http://127.0.0.1:8001/health`.

## Run the tests

```sh
make test
```

Run linting, type checks, and tests together with:

```sh
make check
```
