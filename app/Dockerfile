FROM python:3.9
WORKDIR /app
COPY . .
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
ENV FLASK_APP main.py
ENV PORT 5000
EXPOSE 5000
CMD [ "flask", "run", "--host=0.0.0.0" ]