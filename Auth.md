# Get Auth Request
Perform authorization request to get token


Method: `POST`  
URL: `https://thongtindaotao.sgu.edu.vn/api/auth/login`  
Headers:  
 - `Content-Type`: `application/json`  

Body:  
 ```
 username={username}&password={password}&grant_type=password
 ```

Variables:  
 - `{username}` : student id
 - `{password}` : password, what do you expect?


Response:
 ```json
 {
  "access_token": String,
  "token_type": "bearer",
  "expires_in": Int,
  "refresh_token": String,
  "userName": "{username}",
  "id": String,
  "logtime": String,
  "code": String,
  "result": "true" | "false",
  "passtype": "0",
  "name": String,
  "principal": String,
  "idpc": String,
  "roles": "SINHVIEN" | "GV",
  "wcf": "0",
  ".expires": String,
  ".issued": String
}
 ```