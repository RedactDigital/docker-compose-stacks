FROM ubuntu:22.04

RUN apt-get update && apt-get install -y \
    curl \
    vim \
    build-essential


RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y

ENV PATH="/root/.cargo/bin:${PATH}"

WORKDIR /usr/src/app

CMD ["sh", "-c", "cargo run"]

