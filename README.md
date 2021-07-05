# bearer-auth

### Author : Hatem Husnieh  

## install  
1. copy the link of the repo
1. clone the repo on your local machine by `git clone repo-url`
1. download independencies by `npm i`
1. create a `.env`, then cope the content of `.env.sample` file inside the `.env` file.
1. fill the variables of `.env`
1. run the app

## Deploy, Run and Test
- [test report](https://github.com/Hatemhusnieh/bearer-auth/actions)
- [deployed link](https://hatem-bearer-auth.herokuapp.com/)
- [Pull Request](https://github.com/Hatemhusnieh/bearer-auth/pull/1)

### Setup  
#### `.env` requirement
  - `PORT` - port number  
  - `MONGODB_URL` - port number
  - `SECRET` - a random string

#### Running the app  
- either:
  1. `npm start`
  1. `nodemon`
- connect to mongodb database
- through `postman` or `thunder client`
- Sign Up: `http://localhost:3001/signup`
  - send an `json` object as follow:  

    ![signup](./img/sup.png)  

  - returns user Object as saved in DB  

    ![Object](img/upres.png)  
- Sign In: `http://localhost:3001/signin`
  - send in headers username and password as follow :  
    ![signin](img/sin.png)  

  - returns Object  

    ![Object](img/inres.png)  
- users end point: `http://localhost:3001/users`
  - send the bearer token from the sign in process :  

    ![bearer](/img/user.png)  
  - returns Object  

    ![Object](img/userres.png)  
- secret end point: `http://localhost:3001/secret`
  - send the bearer token from the sign in process :  

    ![secret](/img/sec.png) 

  - returns Object  

    ![Object](img/secres.png)   


#### Test 
- Unit test: `npm run test`
- Lint test: `npm run lint`

### UML:  
![uml](img/bearer-auth.jpg)