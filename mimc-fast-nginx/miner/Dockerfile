# syntax=docker/dockerfile:1
FROM rust:1.53
WORKDIR /code
ENV RUST_LOG=info
RUN cargo install --git https://github.com/projectsophon/darkforest-rs --bin mimc-fast --force --branch=main
EXPOSE 8000
COPY . .
CMD ["mimc-fast"]
