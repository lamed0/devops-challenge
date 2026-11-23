FROM python:3.12-slim

RUN useradd --create-home --uid 10001 appuser

WORKDIR /app
COPY app/app.py .

ENV PORT=5000
EXPOSE 5000

USER 10001

CMD ["python", "app.py"]