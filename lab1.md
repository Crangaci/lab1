# Sarcina nr.1. Analiza cererilor HTTP

## În fig.1. au fost introduse datele incorecte 

![fig.1.](img1.png)

1. *Ce metodă HTTP a fost utilizată pentru a trimite cererea?*

Metoda HTTP utilizată pentru a trimite cererea de autentificare este **POST**. Aceasta metodă este folosită pentru a trimite date către server, mai ales când se transmit informații sensibile, cum ar fi datele de autentificare (username și password).

2. *Ce anteturi au fost trimise în cerere?*

- content-type: `application/x-www-form-urlencoded; charset=UTF-8`
- user-agent: `Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/128.0.0.0 Safari/537.36`
- accept: `*/*`
- host: `sandbox.usm.md`

3. *Ce parametri au fost trimiși în cerere?*

- username: `student`
- password: `studentpass`

4. *Ce cod de stare a fost returnat de server?*

A fost returnat codul de stare **401 Unauthorized**.

5. *Ce anteturi au fost trimise în răspuns?*

- content-type: `text/plain;charset=UTF-8`
- user-agent: `Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/128.0.0.0 Safari/537.36`
- accept: `*/*`
- host: `sandbox.usm.md`

## În fig.2. au fost introduse datele corecte

![fig.1.](img2.png)

1. *Ce metodă HTTP a fost utilizată pentru a trimite cererea?*

Metoda HTTP utilizată pentru a trimite cererea de autentificare este **POST**. Aceasta metodă este folosită pentru a trimite date către server, mai ales când se transmit informații sensibile, cum ar fi datele de autentificare (username și password).

2. *Ce anteturi au fost trimise în cerere?*

- content-type: `application/x-www-form-urlencoded; charset=UTF-8`
- user-agent: `Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/128.0.0.0 Safari/537.36`
- accept: `*/*`
- host: `sandbox.usm.md`

3. *Ce parametri au fost trimiși în cerere?*

- username: `admin`
- password: `password`

4. *Ce cod de stare a fost returnat de server?*

A fost returnat codul de stare **200 OK**.

5. *Ce anteturi au fost trimise în răspuns?*

- content-type: `application/x-www-form-urlencoded; charset=UTF-8`
- user-agent: `Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/128.0.0.0 Safari/537.36`
- accept: `*/*`
- host: `sandbox.usm.md`
