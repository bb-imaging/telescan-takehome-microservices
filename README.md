## Welcome to the TeleScan&trade; Microservices Takehome Assignment
First off, thank you for taking the time to work on this assignment. TeleScan&trade; is a quickly growing startup with a development team that manages dynamic requirements and we're looking to bring on sharp engineers that want to work on today's latest stable frameworks. As such we utilizes [Nest](https://github.com/nestjs/nest) for our microservices architecture and Redis for our service-to-service communication along with a host of other tools to create exciting new technology that is expanding access to ultrasound imaging in underserved communities.

## The Assignment
We'd like to see you build out a simple microservice API framework using NestJS which contains 2 services and 4 data models of varying relations. The services should communicate via Redis. As an API we expect to see basic CRUD (Create, Read, Update, Delete) operations. Everything else is up to you and your creative mind. Feel free to WOW! us by adding unit tests, cascading deletion, code optimization, etc. We have outlined the services and data models below. Feel free to expand upon this architecture, just make sure to at least include what is listed.

### Service 1 Data Models
```
Doctor = {
  id: string,
  first_name: string,
  last_name: string,
}
```
```
Patient = {
  id: string,
  first_name: string,
  last_name: string,
  dob: number
}
```

### Service 2 Data Models
```
Study = {
  id: string,
  study_date: number
}
```
```
Instance = {
  measurment: string,
  image_url: string
}
```
### Model Relations
Doctor is one-to-many with Patient
Patient is one-to-one with Study
Doctor is many-to-many with Study
Study is one-to-many with Instance

## What Are We Looking For?
We like this type of technical review for candidates because it allows you to write code in the most realistic setting as you would on our team -- asynchronously and with your tools of choice. We've tried to keep the assignment relatively simple to be respectful of your time while still providing the opportunity showcase your skills. As such we like seeing clean, succinct code that is performant and maintainable.

## The Next Step
Once you've completed your application please push your repo(s) to Github and share the link(s) with your point of contact at TeleScan&trade;. We will review your code and schedule a time for you to review with one of our senior developers.