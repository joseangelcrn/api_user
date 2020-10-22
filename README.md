<h1>Test API REST for authenticate users (Usage example) </h1>

<p>
    <b>POST - Sign Up</b> [ <i>https://api-auth-user.herokuapp.com/api/signup</i> ]
</p>

       //Request Body
       {
           "name":"test",
           "email":"test@gmail.com",
           "password":"test"
       }

       //Backend Response 

       {
           "message": "Successfully created user!"
       }

<p>
    <b>POST - Login</b> [ <i>https://api-auth-user.herokuapp.com/api/login</i> ]
</p>


       //Request Body
       {
           "email":"test@gmail.com",
           "password":"test"
       }

       //Backend Response 

       {
            "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9........",
            "token_type": "Bearer",
            "expires_at": "2021-10-22 17:05:21"
        }


<p>
    <b>GET - Home</b> [ <i>https://api-auth-user.herokuapp.com/api/user</i> ]
</p>


       //Request Header
        Content-Type : application/json
        X-Requested-With: XMLHttpRequest
        Authorization: Bearer [Token]'

       //Backend Response 
       {
             "id": 4,
             "name": "test",
             "email": "teest@gmail.com",
             "email_verified_at": null,
             "created_at": "2020-10-22T17:04:34.000000Z",
             "updated_at": "2020-10-22T17:04:34.000000Z"
       }


<p>
    <b>GET - Logout</b> [ <i>https://api-auth-user.herokuapp.com/api/logout</i> ]
</p>
                

       //Request Header
         Content-Type : application/json
         X-Requested-With: XMLHttpRequest
         Authorization: Bearer [Token]'

       //Backend Response 

       {
         "message": "Successfully logged out"
       }
