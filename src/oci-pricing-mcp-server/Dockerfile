FROM python:3.11-slim
WORKDIR /app
COPY . /app
RUN pip install --no-cache-dir uv && \
    uv --no-cache sync --locked --all-extras
CMD ["uv", "run",  "oci-pricing-mcp-server.py"]
