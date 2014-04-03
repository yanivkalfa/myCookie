myCookie
========

Simple jquery plugin to handle js cookies in a very simple way.

Although you are able to use objects as cookie value with the plugin keep in mind the 4k limit per domain(which is about 1000-4000 characters) exceeding this will couse problems.

<strong>Setting a cookie: </strong>
```javascript
var cookie = {
  cName : "newCookie",
  cVal : "newCookie",
};
$.fn.myCookie(cookie); 
```
Will create a new cookie named newCookie with the value newCookie<br><br>


<strong>Setting a cookie with expiration (in seconds): </strong>
```javascript
var cookie = {
  cName : "newCookie",
  cVal : "newCookie",
  exp : 300//seconds
};
$.fn.myCookie(cookie);
```
Will create a new cookie named newCookie with the value newCookie and will expire in 300 seconds<br><br>

<strong>Retrieving a Cookie: </strong>
```javascript
$.fn.myCookie({cName: "newCookie"});
```
Will return the value "newCookie" in our case <br>

<strong>Deleting a Cookie: </strong>
```javascript
$.fn.myCookie({cName: "newCookie", del:true});

// Or:

$.fn.myCookie({cName: "newCookie", exp:0});
```
Both cases will delete the cookie "newCookie" <br>

