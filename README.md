## About the project

This project has 2 independent APIs that communicate with each other to demonstrate the use of the Microservices Architecture. These are:

1. The `carsInt` API which is used to communicate with internal resources
2. The `carsExt` which is the endpoint exposed publicly to be accessed by 3rd party applications

It is used as a code base for an assessment as part of Bankaks Recruitment processes for AWS Devops Engineer

### CarsInt

| Method | Endpoint  | Description                                    |
| ------ | --------- | ---------------------------------------------- |
| GET    | /         | Sanity check                                   |
| GET    | /cars     | Returns a list of cars                         |
| GET    | /cars/:id | Get the by the id specified in the route param |

### CarsExt

| Method | Endpoint        | Description                                      |
| ------ | --------------- | ------------------------------------------------ |
| GET    | /               | Sanity check                                     |
| GET    | /cars?id={\_id} | Get a car by the id specified in the query param |
