Quick API endpoint to compile sass via a REST endpoint. 



**Start the server**

```
yarn install 
node src/index.js
```

**Make a request against the server**

```
curl --location --request POST 'localhost:3001/compile' \
--header 'Content-Type: application/json' \
--data-raw '{
    "sass": ".foo {button {border: solid 1px red;}}"
}'
```

Response: 

```
{"css":".foo button {\n  border: solid 1px red;\n}\n"}
```




