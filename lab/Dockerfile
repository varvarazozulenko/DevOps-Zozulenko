FROM python:3.13-slim-bookworm

WORKDIR /app
ENV PYTHONUNBUFFERED=1 PYTHONDONTWRITEBYTECODE=1

LABEL course.student="08072004"

COPY app.py index.html ./

RUN mkdir -p /data && chown -R 10001:10001 /data

USER 10001:10001
EXPOSE 8000
CMD ["python", "app.py"]
