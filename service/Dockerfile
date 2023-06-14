FROM golang:1.19.8 as bd
WORKDIR /github.com/layer5io/sample-app-service
ADD . .
RUN GOPROXY=direct GOSUMDB=off go build -a -o ./main .
CMD ["./main"]