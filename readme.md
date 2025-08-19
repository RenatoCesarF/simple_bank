Create postgres docker container
`docker run --name postgres12 -p 5432:5432 -e POSTGRES_HOST_AUTH_METHOD=trust -e POSTGRES_USER=root -e POTGRES_PASSWORD=secret -d postgres:12-alpine`

Migration creation
`migrate create -ext sql -dir db/migration -seq init_schema`
