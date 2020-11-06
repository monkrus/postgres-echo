# postgres-echo
Golang postgres echo connectivity with Echo framework and Gorm

1. Echo is a highly scalable API development framework

2. GoLang Object Relation Mapping/DB connectivity

3. `go mod init github.com/monkrus/postgres-echo.git`

4. `go get github.com/labstack/echo/v4 `(install Echo)

5. Use sample code provided by Echo in `main.go`

6. `go run main.go`

7. `go get -u gorm.io/gorm`

8. Install `docker` and `docker-compose` https://docs.docker.com/compose/install/

9. Run `docker-compose up` for pg admin page

9. Run `ifconfig |grep inet` to display your ip address xxx.xxx.x.x 

10. Notes:

- docker_postgres_init.sql creates an initial students table
- docker-compose.yml file sets an environment for PG Admin
- db.go (config) configures user, password, host etc.
- student.go (model) consists of student struct (id and name)
- db.go (storage) configures new DB, gets an error if if does not start properly
- student.go (controller) displays student`s records as a JSON using GetRepoStudents (fetching the table students)
- main.go has echo instance, middleware, server start etc.




