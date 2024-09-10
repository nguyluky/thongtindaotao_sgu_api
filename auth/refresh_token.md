# Refresh Token
get new token when token time out


Method: `POST`  
URL: `https://thongtindaotao.sgu.edu.vn/api/auth/login`  

Body:  
 ```
 refresh_token={refresh_token}&grant_type=refresh_token
 ```

Variables:  
 - `{refresh_token}` : refresh token


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
