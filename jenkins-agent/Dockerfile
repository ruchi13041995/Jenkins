FROM maven:3.9.9-eclipse-temurin-17

USER root

RUN apt-get update && \
    apt-get install -y docker.io git curl && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

WORKDIR /workspace

CMD ["bash"]