# Notes:
Languages the web understands:
- HTML,
- CSS and
- JS.
- transpiling to convert from these languages to the web

First web browser: Mosaic, was developed for those with money, military, university scholars (PHD)

		     Netscape was next.
Netscape vs Explorer: Explorer won because Microsoft created windows that came preloaded with explorer. 

Vista version, windows 7, windows 10, windows 11.
- Windows took off in 1998.

- Google chrome took over after 2011 – 2012 because of android phones.

- IE now Microsoft edge

- The server’s (back-end) main job is to deliver data to the right person.

Inspect the page: click networks: then filter for CSS: Right click on the css file and click “block request URL”, this blocks the css from loading; you will only get the html. We learned how to go to networks panel and block css.

## What happens when you click www.google.com?
-	Google lives in the USA
-	Your computer sends a request to the domain name system (DNS) server, which functions as an address book for all domain names. The DNS server then returns the precise IP address of the server that https://www.google.com points to.
-	With this IP address, your computer then creates a connection with the server via the IP address. This connection type is called TCP (Transmission Control Protocol), and your computer can establish this connection through the IP (Internet Protocol). This entire process is known as a "handshake."
-	If your computer is situated behind a firewall, the firewall verifies that the specific request you are making is authorized before granting it. Additionally, if the server you are attempting to access is also behind a firewall, a similar check will be conducted before you can ultimately connect to the server.
-	Once the connection is established, your browser sends a request for the webpage using a security protocol like SSL (Secure Sockets Layer) or TLS (Transport Layer Security) to encrypt the data that will be exchanged between your computer and the server. This encryption is responsible for the "s" in "https" (Hypertext Transfer Protocol Secure), indicating a secure connection.

IP Addresses: ISP (Afrihost for South Africa) gives us the IP address.
-	Public – Used by ISP
-	Private – Banks/government would want this, no one hears what they say (privacy purposes). Your Router
-	Static – Does not change. Used by Banks/Government.
-	Dynamic – Cheaper for the business because they can assign you whatever number they want.
MAC address of a phone, go to a hp store to see who bought it.
IMEI number does not change in your phone.

## The TCP handshake
TCP uses a three-way handshake to establish a reliable connection. The connection is full duplex, and both sides synchronize (SYN) and acknowledge (ACK) each other. The exchange of these four flags is performed in three steps—SYN, SYN-ACK, and ACK—as shown in Figure. 

 <img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTLPCT-9SI237JX_H4bpGUK3B_wppQQf9CJcuAOygYKZ0ZBvkBIZI5X0WvBp18Z6ceWHiI&usqp=CAU'/>


- TCP (FTP, web browsing, email) is slower but more reliable transfer and unicast, while UDP (live streaming, online games, VoIP) is faster but not guaranteed transfers and multicast.

- High ping means slower browsing and laggy responses during online gaming. 
Use UDP on games because of less lagging.
- South Africa is connected to the US through wire cables under the ocean. The government does the cables. Then ISP (Afrihost) connects the cables from where they end to your home.
- Send 1GB file into 100 packets of 10mb.
- Unicast – Talk to one person.
- Multicast – Talk to multiple people.


## HTTP Timeline:
-	HTTP/1.0 – Open connection, Send the file, then close the connection. Separate connections.
-	HTTP/1.1 – persistent connections, request queuing, 6 requestion for one connection.
-	HTTP/1.1 – Pipelining, response queuing, head-of-line blocking (Have to wait for one to finish).
-	HTTP/2 – multiplexing over single connection.


- v2 get the certificate -> first get the index.html
- HTML understands the DOM tree so it uses it
We are requesting http2 by getting a certificate, by a trusted person. – Used a demo http://www.http2demo.io/
-The user interface -> anything outside the webpage (refresh, back, front buttons)
- Backend UI - Style of the radio buttons e.g.,

## Assignment: 
What was the issue in http2 and what was fixed in http3.
Hint: Problem head of the line blocking.
- Although HTTP/2 uses multiplexing it still suffers from another kind of HOL (Head-OF-Line), namely on the TCP level. One lost packet in the TCP stream makes all streams wait until that packet is re-transmitted and received. This HOL is being addressed with the QUIC protocol.

-  If a single TCP packet is lost, then the TCP connection must request it be resent and wait for that packet to be retransmitted successfully before it can process subsequent TCP packages

- QUIC is a "TCP-like" protocol implemented over UDP where each stream is independent so that a lost packet only halts the particular stream to which the lost packet belongs, while the other streams can go on.

HTTP/3 is being done over QUIC instead of TCP and TLS.

<img src = 'https://images.ctfassets.net/ee3ypdtck0rk/iKEoL7owBtLGeeIN1Asxp/7a67adafee7e1ff744a61cdab224ff40/Screen_Shot_2021-01-28_at_13.18.02.png?w=1335&h=703&q=50&fm=webp'/>

<img src = 'https://images.ctfassets.net/ee3ypdtck0rk/3wxbRHFSG1Otb148Syb8AZ/4c29cf416dbb2a645b22b10d29ee224f/Screen_Shot_2021-01-28_at_18.35.51.png?w=1336&h=1215&q=50&fm=webp'/>


- Should learn marked down format.

## Status Codes:
-	Informational responses (100 – 199)
-	Successful responses (200 – 299)
-	Redirection messages (300 – 399)
-	Client error responses (400 – 499)
-	Server error responses (500 – 599)

### CRUD (Create, Read, Update, Delete)

- Website: GET and POST.
- CSSOM – Cascading Style Sheet.
- HTML Elements – HTML Body Element – Paragraph element (Text) and Div element (Image element)

- Structure of a Web Browser: User Interface -> Browser (-> Storage (Cookies)) and rendering engine.
- Browser engine – Delegate the stuff
- UI Backend – Determine the style (e.g., radio buttons, checkboxes)
- Inspect -> Applications (Storage of data) -> Can also be used for tracking.
Use the same chromium browser – Microsoft edge, chrome, opera.

## What is the difference between a web app and a mobile app?
-	mobile apps are platform-specific - each platform needs a specific one unless you decide on hybrid app development,
-	one web app works on every platform, device, and system's version, so web apps are quicker and easier to build,
-	mobile apps are faster and tend to be more complex in terms of features and functionalities,
-	mobile apps are built using platform-specific technologies, so your developers need to be experts in a particular technology,
-	web apps are built using technologies like JavaScript, CSS, HTML, .NET, Python - it makes easier to find developers.

### Web App Vs Website
- Web app – if you can change your experience or others, like YOUTUBE (when you unlike a video many times. It might end up not showing on other people’s dashboard – changed other people’s experience). Dynamic.
- Website – Static (does not change). The experience is the same for every person.

- Web architecture: Python + Flask, Java + bootstrap.

## HTML Code

<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title>replit</title>
  <link href="style.css" rel="stylesheet" type="text/css" />
  <style>
    h1 {
      color: crimson
    }
    img {
      width: 50%;
    }
  </style>
</head>

<body>
  <h1>Hi, Guys 😍 </h1>
  <img src = 'https://ssec.si.edu/sites/default/files/blogpost/images/BUTTERFLY%20WING%20OPTICS.png' />
  <script src="script.js"></script>
</body>

</html>

## Python Fundamentals
- repl -> Read Evaluate Print Loop
- type(variableName) -> to get type 
- True = 1, False = 0
- String literals -> "Hello my name is"
- You can use f{} to format the output. The brackets are called the "interpolation"

### Task
- Given a temperature in ferenheit convert to degrees.

```python
temperature = float(input("Please enter a temperature in ferenheit "))
convert = (temperature - 32) * (5 / 9)
print("Temperature in celsius " + str(convert))
```

- Get the age from the year they were born
```python
birth_year = input("Enter the year you were born in ")
age = 2024 - int(birth_year)
print(f"You are {age} years old")
```

- Calculate area of circle given radius
```python
import math
r = input("Enter radius ")
area = math.pi*float(r)**2
print(f"The area of the circle is {area}")
```

- Given an input: Give output percentage
```python
num = input("Enter a number ")
eq = int(num) // 10
spaces = 10 - eq
print(f'[{"=" * eq} {" " * spaces}] {num}%')
```
- array = "I love python"
- Slicing: array[2:6] -> starts at position 2 until position 5 -> "love"

           array[7:] -> Starts at 7 until end of array

           quote[-6:] -> to get "python"

           quote[::3]

