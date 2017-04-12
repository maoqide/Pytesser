FROM debian:jessie

WORKDIR /workspace

RUN apt-get update \
  && apt-get install -y git curl python tesseract-ocr \
  && curl https://bootstrap.pypa.io/get-pip.py | python \
  && pip install opencv-python \
  && git clone --depth 1 https://github.com/maoqide/Pytesser.git \
  && apt-get purge --auto-remove -y git curl \
  && apt-get clean \
  && rm -rf /var/cache/apt/*

CMD ["/bin/bash"]
