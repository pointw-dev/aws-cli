FROM python:3.10.4
MAINTAINER michael@pointw.com

RUN pip install --no-cache-dir awscli==1.36.0
RUN apt-get update && apt-get install -y \
    groff \
    && rm -rf /var/lib/apt/lists/*

CMD ["bash"]
