# Makefile

go:
	protoc -I =. \
		-I =../../ \
		--go_out . \
		--go_opt paths=source_relative \
		--go-grpc_out . \
		--go-grpc_opt paths=source_relative \
		--grpc-gateway_out allow_delete_body=true:. \
		--grpc-gateway_opt logtostderr=true \
		--grpc-gateway_opt paths=source_relative \
		account.proto;
clean:
	rm -rf *.go
