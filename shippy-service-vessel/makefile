Proto:
#Create a proto
protoc --proto_path=proto/vessel --micro_out=. --go_out=. proto/vessel/vessel.proto

build:
#Build a docker image
docker build -t shippy-service-vessel .

run:
#Run Docker image
docker run -p 50052:50051 -e MICRO_SERVER_ADDRESS=:50051 shippy-service-vessel