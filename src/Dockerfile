FROM rust:latest

RUN curl -sL https://deb.nodesource.com/setup_14.x | bash -
RUN apt-get --yes update && apt-get --yes install pkg-config libssl-dev nodejs
RUN npm i
RUN cargo install trunk wasm-bindgen-cli
RUN rustup target add wasm32-unknown-unknown