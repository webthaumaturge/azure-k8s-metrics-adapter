all: clean build ; 
build:
	go build -o ./bin/producer ./producer/main.go
	go build -o ./bin/consumer ./consumer/main.go
clean:
	go clean && rm -rf ./bin
dev:
	skaffold dev
consumer-container:
	docker build -t jsturtevant/queue-consumer-external-metric .