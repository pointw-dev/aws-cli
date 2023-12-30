FROM python:3.9.18
MAINTAINER michael@pointw.com

RUN pip install --no-cache-dir awscli==1.32.11
RUN apt-get update && apt-get install -y \
    groff \
    && rm -rf /var/lib/apt/lists/*

CMD ["bash"]
