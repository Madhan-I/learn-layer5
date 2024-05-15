FROM golang:1.21.10 as bd
WORKDIR /github.com/layer5io/sample-app-service
ADD . .
RUN GOPROXY=direct GOSUMDB=off go build -a -o ./main .
CMD ["./main"]