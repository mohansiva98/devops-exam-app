FROM python:3.10-slim

WORKDIR /app/backend

COPY backend/ /app/backend/
COPY db/ /app/db/

RUN pip install -r requirements.txt

ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0

CMD ["flask", "run"]
