build:
	protoc -I. --go_out=plugins=micro:. \
	  proto/consignment/consignment.proto
	docker build -t microservice-example .

run:
	docker run -p 50051:50051 \
	-e MICRO_SERVER_ADDRESS=:50051 \
	microservice-example	


#build:
#    protoc -I. --go_out=plugins=grpc:. \
#      proto/consignment/consignment.proto
