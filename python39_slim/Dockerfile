FROM python:3.9-slim
RUN pip install --upgrade pip
COPY ./requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

ENV LC_ALL C.UTF-8
ENV PYTHONPATH=/usr/local/lib/python3.9/site-packages/