<h1>Test API REST for authenticate users</h1>
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
    <b>GET - Logout</b> [ <i>https://api-auth-user.herokuapp.com/api/logout</i> ]
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
