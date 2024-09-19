
# Sarcina nr.1. Analiza cererilor HTTP

 În *fig.1.* au fost introduse datele incorecte

![](Aspose.Words.fb82daef-b398-4aaf-8f33-c5e51d370e78.001.jpeg)
*fig.1.*

1) *Ce metodă HTTP a fost utilizată pentru a trimite cererea?*

Metoda HTTP utilizată pentru a trimite cererea de autentificare este **POST**. Aceasta metodă este folosită pentru a trimite date către server, mai ales când se transmit informații sensibile, cum ar fi datele de autentificare (username și password).

2) *Ce anteturi au fost trimise în cerere?*

- content-type: `application/x-www-form-urlencoded; charset=UTF-8`
- user-agent: `Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/128.0.0.0 Safari/537.36`
- accept: `*/*`
- host: `sandbox.usm.md`

3) *Ce parametri au fost trimiși în cerere?*

- username: `student`
- password: `studentpass`

4) *Ce cod de stare a fost returnat de server?*

A fost returnat codul de stare **401 Unauthorized**

5) *Ce anteturi au fost trimise în răspuns?*

- content-type: `text/plain;charset=UTF-8`
- user-agent: `Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/128.0.0.0 Safari/537.36`
- accept: `*/*`
- host: `sandbox.usm.md`

În *fig.2.* au fost introduse datele corecte

![](Aspose.Words.fb82daef-b398-4aaf-8f33-c5e51d370e78.002.jpeg)
*fig.2.*

1) *Ce metodă HTTP a fost utilizată pentru a trimite cererea?*

Metoda HTTP utilizată pentru a trimite cererea de autentificare este **POST**. Aceasta metodă este folosită pentru a trimite date către server, mai ales când se transmit informații sensibile, cum ar fi datele de autentificare (username și password).

2) *Ce anteturi au fost trimise în cerere?*

- content-type: `application/x-www-form-urlencoded; charset=UTF-8`
- user-agent: `Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/128.0.0.0 Safari/537.36`
- accept: `*/*`
- host: `sandbox.usm.md`

3) *Ce parametri au fost trimiși în cerere?*

- username: `admin`
- password: `password`

4) *Ce cod de stare a fost returnat de server?*

A fost returnat codul de stare **200 OK**

5) *Ce anteturi au fost trimise în răspuns?*

- content-type: `text/plain;charset=UTF-8`
- user-agent: `Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/128.0.0.0 Safari/537.36`
- accept: `*/*`
- host: `sandbox.usm.md`

# Sarcina nr. 2. Crearea cererilor HTTP

1) *Cerere **GET***
```http
GET / HTTP/1.1

Host: sandbox.com

User-Agent: Crangaci Sabina
```

2) *Cerere **POST***
```http
POST /cars HTTP/1.1

Host: sandbox.com

Content-Type: application/x-www-form-urlencoded make=Toyota&model=Corolla&year=2020
```

3) *Cerere **PUT***
```http
PUT /cars/1 HTTP/1.1

Host: sandbox.com User-Agent: Crangaci Sabina Content-Type: application/json {

"make": "Toyota",

"model": "Corolla",

"year": 2021

}
```

4) *Posibile răspunsuri*
- Cerere *PUT*
```http
HTTP/1.1 200 OK Content-Type: application/json {

"id": 1,

"make": "Toyota",

"model": "Corolla",

"year": 2021

}
```

- Cerere *POST*
```http
HTTP/1.1 201 Created Content-Type: application/json {

"id": 1,

"make": "Toyota",

"model": "Corolla",

"year": 2020

}
```

*Situații în care serverul poate returna coduri de stare HTTP*

- ***200 OK***: Cererea a fost procesată cu succes..
- ***201 Created***: Cererea POST a fost procesată cu succes și a fost creată o nouă resursă.
- ***400 Bad Request***: Cererea este invalidă, de exemplu, parametrii lipsă sau format incorect.
- ***401 Unauthorized***: Autentificarea este necesară și a eșuat sau nu a fost furnizată.
- ***403 Forbidden***: Serverul a înțeles cererea, dar refuză să o autorizeze.
- ***404 Not Found***: Resursa solicitată nu a fost găsită pe server.
- ***500 InternalServer Error***: Serverul a întâmpinat o eroare neașteptată care l-a împiedicat să proceseze cererea.

6) *Cerere **DELETE***
```http
DELETE /cars/1 
HTTP/1.1 
Host: sandbox\.com 
User-Agent: Crangaci Sabina
```

Metoda **DELETE** este potrivită pentru a șterge o resursă  de pe server.De exemplu, dacă dorim să ștergem date, utilizăm metoda DELETE pentru a indica serverului să elimine acea resursă.

