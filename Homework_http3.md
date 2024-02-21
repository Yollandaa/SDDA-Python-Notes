# Homework

## Assignment: 
What was the issue in http2 and what was fixed in http3.
Hint: Problem head of the line blocking.
- Although HTTP/2 uses multiplexing it still suffers from another kind of HOL (Head-OF-Line), namely on the TCP level. One lost packet in the TCP stream makes all streams wait until that packet is re-transmitted and received. This HOL is being addressed with the QUIC protocol.

-  If a single TCP packet is lost, then the TCP connection must request it be resent and wait for that packet to be retransmitted successfully before it can process subsequent TCP packages

- QUIC is a "TCP-like" protocol implemented over UDP where each stream is independent so that a lost packet only halts the particular stream to which the lost packet belongs, while the other streams can go on.

HTTP/3 is being done over QUIC instead of TCP and TLS.

<img src = 'https://images.ctfassets.net/ee3ypdtck0rk/iKEoL7owBtLGeeIN1Asxp/7a67adafee7e1ff744a61cdab224ff40/Screen_Shot_2021-01-28_at_13.18.02.png?w=1335&h=703&q=50&fm=webp'/>

<img src = 'https://images.ctfassets.net/ee3ypdtck0rk/3wxbRHFSG1Otb148Syb8AZ/4c29cf416dbb2a645b22b10d29ee224f/Screen_Shot_2021-01-28_at_18.35.51.png?w=1336&h=1215&q=50&fm=webp'/>
