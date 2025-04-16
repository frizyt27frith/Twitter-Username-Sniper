You need to add your secrets into here. 

You can get your api key and api secret and all other stuff from here: 

https://developer.twitter.com/en/portal/dashboard



FAQ: 
Frequently Asked Questions: 

how many requests does the script send per second


The number of requests that the script sends per second depends on the number of threads that are used and the length of the delay between requests. With the current code, the number of requests per second can be calculated as follows:
requests per second = threads * (1 / delay)
For example, if the script is using 10 threads and has a delay of 0.1 seconds between requests, the number of requests per second would be:
requests per second = 10 * (1 / 0.1) = 100 requests per second
If the delay is increased, the number of requests per second will decrease, and if the delay is decreased, the number of requests per second will increase.
It's important to note that sending a large number of requests to a server can potentially overwhelm the server and potentially cause issues. As a result, it's generally a good idea to use a reasonable number of threads and a reasonable delay between requests to avoid overloading the server.

What Proxies are supported?


In the current code, the script supports three types of proxies: HTTP, SOCKS4, and SOCKS5. These proxies are used to send requests to the Twitter API through the specified proxy server, which can help to mask the IP address of the client and potentially bypass restrictions or censorship.
To use a proxy with the script, the user must specify the type of proxy to use (HTTP, SOCKS4, or SOCKS5) when starting the program, and provide a list of proxy addresses in a text file called "proxies.txt". The script will then read the proxy addresses from the text file and use them to send requests to the API.
It's important to note that the use of proxies may not always be successful, and the reliability and performance of the proxies can vary. In addition, the use of proxies may be restricted or prohibited by some websites or services, and it's the user's responsibility to ensure that they are using proxies in compliance with the terms of service of the website or service they are accessing.

ebelfc