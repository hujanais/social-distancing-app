https://vercel.com/guides/deploying-a-mongodb-powered-api-with-node-and-vercel

1. npm init
2. npm i mongoose
3. vercel secrets add mongodb-uri mongodb+srv://<user>:<password>@my-cluster-uf345.mongodb.net/<database-name>?retryWrites=true
4. create vercel.json
   {
   "name": "social-distancing-app",
   "version": 2,
   "env": {
   "MONGODB_URI": "@mongodb-uri"
   }
   }
5. for local dev, create an .env file.

6. create a new file in /api folder: /api/data.js
