# api-students
## Teoretisk del:
**Hur används HTTP-protokollet när du surfar in på en websida? Beskriv vilken metod, path, URI, response code och body som skickas in och svarar. Om du har svårt att bestämma dig för en url, ta ex. (http://www.smp.se/kultur-noje/) ?**
* Metod som används är GET.
* Path är /kultur-noje.
* URI (Uniform Resource Identifier) är http://www.smp.se/kultur-noje/
* Body är html

**Beskriv HTTP-protokollets vanligaste metoder och vad de gör?**
* GET - Begär fil eller data.
* POST - Lägger till data som skickas in.
* PUT - Ersätter utvald data med ny data som skickas med (all data måste ändras).
* PATCH - Modifierar utvalda delar av data, där till skillnad från PUT inte hela objectet måste ändras.
* DELETE - Raderar specifik data.

**"http://localhost:3000/users?username=something" är en URI, beskriv vilka delar den består av och vad de kallas.**
* http:// <--Scheme
* localhost:3000 <--Authority / port
* /users <-- Path
* ?username=something <-- Query

**På vilka tre sätt kan man skicka in parametrar i en HTTP-request? Ge exempel med curl.**
* curl "https://jsonplaceholder.typicode.com/users?id=2" <-- query
* curl "https://jsonplaceholder.typicode.com/users/"  -H "Content-Type: application/json; charset=utf-8" <-- Beskriver hur jag skickar min förfrågan och hur jag vill ha den tillbaka.
* curl "https://jsonplaceholder.typicode.com/users/1" <-- Path paramters