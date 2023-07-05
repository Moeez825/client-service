# client-service

The Client Service is a microservice in the Instagram clone application that handles user authentication, user actions, and user interface interactions. It provides endpoints for user login, signup, adding posts, editing posts/comments, following/unfollowing users, liking posts, and more.

## Features

- User login and authentication
- User signup
- Adding, editing, and deleting posts
- Adding and editing comments
- Following and unfollowing users
- Liking posts
- Generating user feeds
- User interface views and templates

## Getting Started

These instructions will get you a copy of the Client Service up and running on your local machine for development and testing purposes.

## Technologies Used
- Java 17
- Spring Boot 3.1.0
- Maven 4.0.0
- PostgreSQL 15.3
- Thymeleaf
## Dependencies

- [Spring Boot] 
- [Spring Web]
- [Spring Data JPA]
- [postgresql]
- [Spring Cloud]
- [Spring Cloud OpenFeign]

### Prerequisites

- [Java SE Development Kit 17.0.5] (https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Maven 4.0.0] (https://maven.apache.org/install.html)
- [Spring Boot CLI] (https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#getting-started-installing-the-cli) (Optional)

### Installation
1. Clone the repository:
```bash
git clone <repository-url>
```
2. Navigate to the project directory::
```bash
cd follow-service
```
3. Open the application.properties file and configure the database connection details:
```
spring.datasource.url=jdbc:mysql://localhost:8086/story_db
spring.datasource.username=<database-username>
spring.datasource.password=<database-password>
```
4. Build the project using Maven:
```bash
cd follow-service
```
5. Run the application:
```bash
mvn spring-boot:run
```
## API Documentation
The Client Service provides various endpoints for user actions and user interface interactions. Here are some examples:

- GET /login: Shows the login form for users to enter their credentials.
- POST /login: Handles the user login process and authenticates the user.
- GET /signup: Shows the signup form for new users to create an account.
- POST /signup: Handles the user signup process and creates a new user account.
- POST /addpost: Adds a new post to the user's profile.
- POST /addcomment: Adds a comment to a post.
- POST /followuser: Follows a user.
- POST /likepost: Likes a post.
- GET /home: Retrieves the user's home feed.
