#Create a proto
protoc --proto_path=proto/consignment --micro_out=. --go_out=. consignment.proto

#Build a docker image
docker build -t shippy-service-consignment .

#Run Docker image
docker run -p 50051:50051 -e MICRO_SERVER_ADDRESS=:50051 shippy-service-consignment