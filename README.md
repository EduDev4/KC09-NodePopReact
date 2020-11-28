# Twittereact

Backend project:
https://github.com/davidjj76/nodepop_web_avanzado
Database installed in .\Data\DB

## Configure backend

Put backend project under .\backend folder.

    cd backend

#### Install dependencies

    npm install

### Configure mongoose and Initialize database

    mongod.exe --dbpath .\data\db
    npm run installDB

### Configure .env

    Create your .env file following the .env.example structure.
    
#### Run an instance (Default port: 30001)
   
    npm start
    
#### Obtain Token

    API requests requires a token that can be obtained at /apiv1/auth/login
    Sample user user@example.com and password 1234
    
    Send these parameters in the body of a POST request
      email = user@example.com
      password = 1234

Sample response:
    
    {
    "ok": true,
    "token": "eyJhbGciOiJIUCCC6IkpXVCJ9.eyJfaWQiOiI1ZmMwMGZiNjA3ODU0NDUxZWM0ZDY0YjUiLCXXXCI6MTYwNjU5NTg5NX0.Ef1MpBQoHu2zXXXhHt9Fhw3WNzAT20368s"
    }
    
## Start main project (Front Single Page Application)

To start a single instance:
    
    npm start

