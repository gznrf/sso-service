## Auth-Service Project Description

This project utilizes Protobuf-proto: [https://github.com/gznrf/sso-protos](https://github.com/gznrf/sso-protos)

### Before Using:

The following steps are required to set up the project:

1.  Create a directory for the project:

    ```bash
    mkdir sso
    cd sso
    ```

2.  Clone the `sso-service` and `sso-protos` repositories:

    ```bash
    git clone https://github.com/gznrf/sso-service
    git clone https://github.com/gznrf/sso-protos
    ```

3.  Navigate to the `sso-service` directory and tidy the Go modules:

    ```bash
    cd sso-service/sso
    go mod tidy
    ```
    
4. Navigate to the `sso-protos` directory and tidy the Go modules:

    ```bash
    cd sso-protos/protos
    go mod tidy
    ```

### Running Migrations:

1.  Navigate to the `sso-protos` directory:

    ```bash
    cd sso-protos/protos
    ```

2.  Run migrations using `task`:

    ```bash
    task migrate
    ```

### Running the Application:

To start the application, execute the following command:

```bash
go run cmd/sso/main.go --config=./config/local.yaml
```

---