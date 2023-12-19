# Get token form browser


1. open browser 
1. login
1. `right click -> inspect -> Console` or `pess F12`
1. pass this code and run
    ```js
    JSON.parse(sessionStorage.getItem("CURRENT_USER")).access_token
    ```