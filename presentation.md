---
title: HTTP(s)
author: Yannik Hellmuth & Philipp Skott
---

Gliederung
==========

1. Grundlagen
2. Geschichte
3. Funktionsweiße HTTP
4. TCP
5. SSL/TLS

Grundlagen
==========
- HTTP steht für Hypertext Transfer Protocol
- zustandsloses Protokoll
- Hauptsächlich für die Übertragung von Webseiten genutzt

Geschichte
==========

![](./geschichte.png)

Funktionsweiße HTTP
===================

Verbindungsaufbau
-----------------
1. Verbindungsaufbau über TCP
2. HTTP Anfrage
3. HTTP Antwort
4. Schließen der Verbindung


Funktionsweiße HTTP
===================

Aufbau einer Anfrage
--------------------
\<Methode\> \<betreffende Resource\> \<Protokolversion\>\
\<HEADER\>\
Beispiel:\
\> GET /infotext.html HTTP/1.1\
\> Host: www.example.net

Funktionsweiße HTTP
===================

HTTP-Anfragemethoden:
---------------------

- GET
- POST
- HEAD
- PUT
- PATCH
- DELETE
- TRACE
- OPTIONS
- CONNECT

Funktionsweiße HTTP
===================

Aufbau einer Antwort
--------------------

Beispiel:\
> HTTP/1.1 200 OK \
> Server: Apache/1.3.29 (Unix) PHP/4.3.4 \
> Content-Length: 123456 (Größe von infotext.html in Byte) \
> Content-Language: de (nach RFC 3282 sowie RFC 1766) \
> Connection: close \
> Content-Type: text/html 


Funktionsweiße HTTP
===================

Statuscodes
-----------

| Code | Bedeutung    |
|----|--------------|
| 1xx | Informationen |
| 2xx | Erfolgreiche Operation |
| 3xx | Umleitung |
| 4xx | Client-Fehler |
| 5xx | Server-Fehler |


Funktionsweiße HTTP
===================

Mögliche Header Inhalte:
------------------------
- Host
- Content-Language
- Content-Type
- Date

TCP
===

![](./TCP.png)

SSL/TLS
=======

- Verschlüsselung von HTTP -> HTTPS
- Arbeitet auf der Transportschicht (Transport Layer Security)
