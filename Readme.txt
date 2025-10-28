Deploy backend to Railway : 
Step 1 : go to the package.json file, change "scirpts"{start : noname server} 
        to : 
        "scripts": {
    "start": "node server.js"
  },
Step 2 : in the server.js change from : 
app.use(
    cors({
        origin: "http://localhost:3000",
        credential: true
    })
)
to : 
app.use(
    cors({
        origin: "*",
        credential: true
    })
)
Step 2 : Commit and replace all file in the git hub
Step 3 : Re-deploy into Railway.
