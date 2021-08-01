# Simple Implement Authorization Code OAuth 2.0 
## Description
Simple project using OAuth 2.0 and Github Authorization Server

## Installation
Step for installation:
```sh
# Clone this project from github
https://github.com/saptarga/spring-boot-oauth-authorization-code-example.git

# Clears the target directory and builds the project
mvn clean install
```

## Configuration
Step for configuration:
- Create OAuth Apps in Github
- Set config in `application.yml`
```yml
security:
  oauth2:
    client:
      clientId: YOUR_CLIENT_ID
      clientSecret: YOUR_CLIENT_SECRET
      accessTokenUri: https://github.com/login/oauth/access_token
      userAuthorizationUri: https://github.com/login/oauth/authorize
      clientAuthenticationScheme: form
    resource:
      user-info-uri: https://api.github.com/user
      prefer-token-info: false
```

## Run Project
You can start this project using
```sh
mvn clean spring-boot:run
```

## Author
Created and maintained by saptarga ([@saptarga](https://www.linkedin.com/in/saptarga)).