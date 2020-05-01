ARG BASE_IMAGE=gcr.io/cloud-builders/java/javac:8
FROM ${BASE_IMAGE}

RUN wget -q -O /usr/bin/install-clojure \
    https://download.clojure.org/install/linux-install-1.10.1.536.sh \
    && chmod +x /usr/bin/install-clojure

RUN install-clojure

RUN mkdir /app
WORKDIR /app

ENTRYPOINT ["clj"]
