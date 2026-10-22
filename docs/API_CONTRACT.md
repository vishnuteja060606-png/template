\# API CONTRACT



\## Standard Response



Every API must follow:



\### Success



{

&#x20; "success": true,

&#x20; "data": {},

&#x20; "error": null

}



\### Failure



{

&#x20; "success": false,

&#x20; "data": null,

&#x20; "error": {

&#x20;   "code": "ERROR\_CODE",

&#x20;   "message": "Human readable message"

&#x20; }

}



\---



\# Authentication



\## POST /api/auth/login



\### Request



{

&#x20; "email": "user@example.com",

&#x20; "password": "password"

}



\### Success



HTTP 200



{

&#x20; "success": true,

&#x20; "data": {

&#x20;   "user": {},

&#x20;   "token": "..."

&#x20; },

&#x20; "error": null

}



\### Failure



HTTP 401



{

&#x20; "success": false,

&#x20; "data": null,

&#x20; "error": {

&#x20;   "code": "INVALID\_CREDENTIALS",

&#x20;   "message": "Invalid email or password"

&#x20; }

}

