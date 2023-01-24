FROM python:3.9-slim AS build
RUN pip install --upgrade pip
COPY ./requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

FROM gcr.io/distroless/python3-debian10
COPY --from=build /usr/local/lib/python3.9/site-packages/ /usr/local/lib/python3.9/site-packages/

ENV LC_ALL C.UTF-8
ENV PYTHONPATH=/usr/local/lib/python3.9/site-packages/