# Infraestructuras_Servicios_Nube

## Run the API locally

Install the dependencies and start the FastAPI server:

```bash
uv sync
uv run uvicorn main:app --reload
```

The API is available at `http://127.0.0.1:8000`. Interactive documentation is
available at `/docs`, and `/health` returns the service health status.

## Run with Docker

Build and start the container:

```bash
docker build -t infraestructuras-servicios-nube .
docker run --rm -p 8000:8000 infraestructuras-servicios-nube
```

The API will be available at `http://127.0.0.1:8000`.