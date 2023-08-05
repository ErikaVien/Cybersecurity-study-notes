# HTTP
- TCP/IP
- TTP1.0/1.1/2.0/3.0

HTTP1.0 : does not support keep-alive, refresh page have to re-establish handshake

DNS -> 3way handshake -> HTTP request -> respond -> HTML code,JS,CSS,image -> Output

**HOST** : domain name

**User-Agent** : what os using
 
**ACCEPT** - accept what type - */*, HTML, XML, application, etc

**COOKIES** : identitfy you (验证身份)

**SET-COOKIES** - from server

**Referer** : from where, which site

**Location** : redirect to/jump to

**Server** : Apache, JSP3, etc

**HTTPS**
-secure with encryption
-SSL protocol
-decrypt using private key and public key
-client can decrypt using SSLlog

### HTTP Request:
- **GET** : after URL is "?" + parameter (参数)=value  
	http://sidepage.com/get.php?arg1=value1
- **POST** : contains data,data-type </br>
	packet head contains data </br>
	accept content-type : application/x-www-form-urlencoded, text/xML, application/json, multipart/form-data, txt/plain
- **OPTIONS** : server respond accepting which type of request only
- **PUT** : use to upload, now become POST
- **DELETE**





