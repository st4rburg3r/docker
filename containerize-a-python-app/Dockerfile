FROM python:3.10-slim

WORKDIR /app

COPY req.txt .

RUN pip install --no-cache-dir -r req.txt
# none of the caches are used so that the image is as small as possible

COPY . .

EXPOSE 3000

CMD ["python", "main.py"]