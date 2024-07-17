<h1> Proxy Server</h1>

The server must process incoming HTTP requests from clients, receive data from them, send requests to other services, receive their responses, and return the client's result in JSON format.

 <h3> Installation<h3>
 1) git clone https://github.com/Sanzhar017/hl-proxy 
   <br>
 2) cd awesomeProject

 <h5>Request post on url postman http://localhost:8081/proxyl, content-type application json <br>
 JSON:
   
```json
 {
  "method": "GET",
  "url": "https://jsonplaceholder.typicode.com/todos/1",
  "headers": {
    "Accept": "application/json"
  }
}
```

Response 
```json
 {
    "id": "678d64cf-0db5-4f25-a74e-f4a6361be6fa",
    "status": 200,
    "headers": {
        "Access-Control-Allow-Credentials": "true",
        "Age": "27458",
        "Alt-Svc": "h3=\":443\"; ma=86400",
        "Cache-Control": "max-age=43200",
        "Cf-Cache-Status": "HIT",
        "Cf-Ray": "8a4b4a113a9681f6-SIN",
        "Content-Type": "application/json; charset=utf-8",
        "Date": "Wed, 17 Jul 2024 15:33:15 GMT",
        "Etag": "W/\"53-hfEnumeNh6YirfjyjaujcOPPT+s\"",
        "Expires": "-1",
        "Nel": "{\"report_to\":\"heroku-nel\",\"max_age\":3600,\"success_fraction\":0.005,\"failure_fraction\":0.05,\"response_headers\":[\"Via\"]}",
        "Pragma": "no-cache",
        "Report-To": "{\"group\":\"heroku-nel\",\"max_age\":3600,\"endpoints\":[{\"url\":\"https://nel.heroku.com/reports?ts=1717832738&sid=e11707d5-02a7-43ef-b45e-2cf4d2036f7d&s=w8QgS%2BC9op2ojd3a1nD0%2Ff4yUkyWbu%2B4sdu1Ce%2Bncng%3D\"}]}",
        "Reporting-Endpoints": "heroku-nel=https://nel.heroku.com/reports?ts=1717832738&sid=e11707d5-02a7-43ef-b45e-2cf4d2036f7d&s=w8QgS%2BC9op2ojd3a1nD0%2Ff4yUkyWbu%2B4sdu1Ce%2Bncng%3D",
        "Server": "cloudflare",
        "Vary": "Origin, Accept-Encoding",
        "Via": "1.1 vegur",
        "X-Content-Type-Options": "nosniff",
        "X-Powered-By": "Express",
        "X-Ratelimit-Limit": "1000",
        "X-Ratelimit-Remaining": "999",
        "X-Ratelimit-Reset": "1717832767"
    },
    "length": 83
}
```

<h5>On render url https://hl-proxy.onrender.com</h5>
  


