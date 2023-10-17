# Coffee Shop - server side
Live project: 

# Followed 
- Express.js: https://expressjs.com/ 
- Middleware/cors: http://expressjs.com/en/resources/middleware/cors.html
- Middleware/body-parsing: https://www.geeksforgeeks.org/express-js-req-body-property/
- DataBase/Mongodb: https://www.mongodb.com/
- PassHider/dotenv: https://www.npmjs.com/package/dotenv 
- CRUD operations: https://www.mongodb.com/docs/drivers/node/current/


- create a file : vercel.json 
and paste this code. dest=(set initial file name).

{
    "version": 2,
    "builds": [
        {
            "src": "./index.js",
            "use": "@vercel/node"
        }
    ],
    "routes": [
        {
            "src": "/(.*)",
            "dest": "index.js",
            "methods": [
                "GET",
                "POST",
                "PUT",
                "PATCH",
                "DELETE",
                "OPTIONS"
            ]
        }
    ]
}
