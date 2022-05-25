FROM rust:1.61 as builder
COPY . .
RUN cargo build --release
ENV ROCKET_ADDRESS=0.0.0.0
EXPOSE 8000
CMD ["./target/release/rest-api"]