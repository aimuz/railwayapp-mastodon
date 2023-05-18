FROM golang as builder

ENV CGO_ENABLED 0

RUN go install github.com/maxmcd/webtty@latest

FROM ghcr.io/mastodon/mastodon

COPY --from=builder /go/bin/webtty /webtty

CMD ["/webtty", "-o"]
