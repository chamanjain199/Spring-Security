Spring security Part 1 : Basic/Login Form Spring security
1) Add Spring Boot Starter Security dependency in your POM
2) Spring provide default user with username : user and password will be Random UUID, that will be printed out in your log
   Ex: Using generated security password: b604c794-ac6e-4ac4-8601-858140cf07e7
   
3)Spring security default auto-configuration support both Basic and Login form based authentication.

Basic Authentication: Each time you need to send an authorization header with value Basic base64 encoded username:password
    Ex: 
     Authorization Basic dXNlcjpiNjA0Yzc5NC1hYzZlLTRhYzQtODYwMS04NTgxNDBjZjA3ZTc=
     you can encode your username and password in base64 from https://www.base64encode.org/
     
Login Form: Firstly user login with a login form by submitting username and password and get a cookie named JSESSIONID
     then user need to send this cookie in other apis
     
