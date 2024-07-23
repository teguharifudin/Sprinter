![](https://www.teguharief.com/img/teguh-arief.png)

# Sprinter

Spring Boot Maven plugin implements JWT authentication with MySQL, and Docker.

## Installation

### From source

```
git clone git@github.com:teguharifudin/Sprinter.git
```
```
cd Sprinter
```

## Developing

### MySQL in Docker
```
docker run -d -e MYSQL_ROOT_PASSWORD=secret -e MYSQL_DATABASE=taskdb --name mysqldb -p 3307:3306 mysql:8.0
```

### Running app
```
mvn install
```
```
mvn spring-boot:run
```

## Usage in Postman: to get Token

POST http://localhost:8005/auth/signup
```
{
    "email": "teguh.arifudin@gmail.com",
    "password": "123456",
    "fullName": "Teguh Arief"
}
```

POST http://localhost:8005/auth/login
```
{
    "email": "teguh.arifudin@gmail.com",
    "password": "123456"
}
```

## Contributing

### Bug Reports & Feature Requests

Please use the [issue tracker](https://github.com/teguharifudin/Sprinter/issues) to report any bugs or file feature requests.