FROM golang

RUN apt-get update -y && apt-get install git

RUN go get github.com/youngjun9072/tuto/protobuf
RUN go get google.golang.org/grpc 

RUN mkdir /app
ADD . /app/
WORKDIR /app
RUN go build -o main .
CMD ["/app/main"]


