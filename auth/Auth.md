# Get Auth Request
Perform authorization request to get token


Method: `POST`  
URL: `https://thongtindaotao.sgu.edu.vn/api/auth/login`  

Body:  
 ```
 username={username}&password={password}&grant_type=password
 ```

Variables:  
 - `{username}` : student id
 - `{password}` : password, what do you expect?


Response:
 ```ts
type AuthResponse = {
    access_token: string,
    token_type: "bearer",
    expires_in: number,
    refresh_token: string,
    userName: "{username}",
    id: string,
    logtime: string,
    code: string,
    result: "true" | "false",
    passtype: "0",
    name: string,
    principal: string,
    idpc: string,
    roles: "SINHVIEN" | "GV",
    wcf: "0",
    .expires: string,
    .issued: string
}  
 ```