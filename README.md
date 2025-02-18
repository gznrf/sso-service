Protobuf-proto: https://github.com/gznrf/sso-protos

before using:

mkdir sso
cd sso
git clone https://github.com/gznrf/sso-service
git clone https://github.com/gznrf/sso-protos
cd sso-service
go mod tidy

to start migrations:

cd sso-protos
task migrate

to run the app:

go run cmd/sso/main.go --config=./config/local.yaml 

