FROM alpine:3.7

COPY . /app
WORKDIR /app

RUN apk add --update \
    python \
    python-dev \
    py-pip
RUN /bin/sh -c "pip install --upgrade pip"
RUN /bin/sh -c "pip install -r requirements.txt"

ENTRYPOINT ["python"]
CMD ["hello.py"]