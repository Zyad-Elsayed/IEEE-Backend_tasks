`hyper text transfer protocol` which is responsible for communication between web server and clients. that means every time you open you web browser and start visiting website, this http protocol is the  way for this connection otherwise there would be no connection and these data would be reachless

HTTP is stateless in other words every request is independant and it can't remeber or store any previous actions like logging in so there are other functionality to enhance user experience like cookies which contains user sessions and other data 

### HTTP vs HTTPS

they are almost same sturcture the only difference between the two protocols is that **HTTPS uses TLS (SSL) to encrypt normal HTTP requests and responses, and to digitally sign those requests and responses**. As a result, HTTPS is far more secure than HTTP. Thus, allows only authorized people to see these data which may contains credentials and other sensitive information.
+ S in HTTPS stands for secure 

### HTTP methods 
there are many diffrent methods of http requests but the most known are 
+ **GET** : used for retrieve data from the server 
+ **Post** : used to submit data to the server 
+ **Put** : update data already on the server 
+ delete data from the server 

### HTTP consists of two aspects, requests and responces

- ##### Requests
	requests consists of there parts 
	1. request line: it is the first line of the HTTP request.
	It specifies the request method, the requested URL "path", and the version of HTTP used. headers, there are many methods or requests like get or post request 
	`GET /software/htp/cics/index.html HTTP/1.1`
	2. request headers 
	These are the rest of lines and used to pass additional information about the request to the server. This allows the server to customize results sent to the client.
	3. body which is optional depending on the method. If you are passing data to the server on not like in Post method
+ ##### Responses 
1. A status line.
	the first line in the response message. It consists of three items:
	`HTTP/1.1 200 OK`
	+ The HTTP version number, showing the HTTP specification to which the server has tried to make the message comply.
	+ A **status code**, which is a three-digit number indicating the result of the request.
	+ A **reason phrase**, also known as status text, which is human-readable text that summarizes the meaning of the status code.
2.  A series of HTTP headers, or header fields.
3.  A message body, which is usually needed.

### Status code
-  The range 100-199 is classed as Informational.
```
the initial part of the request has been received by the server and that the client should proceed with the request.
```
-   200-299 is Successful.
-   300-399 is Redirection.
-   400-499 is Client error.
-   500-599 is Server error.

#### Common status code 
+ 200 - ok 
+ 201 - ok created
+ 301 - moved tonew url 
+ 304 - cashed version 
+ 400 - bad request 
+ 401 - unauthorized
+ 404 - not found 
+ 500  - internal server error 

For more info [IBm](https://www.ibm.com/docs/en/cics-ts/5.2?topic=concepts-http-protocol) 