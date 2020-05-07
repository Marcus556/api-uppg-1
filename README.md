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

# Praktisk del:
## Installation:
1. git clone git@github.com:Marcus556/api-uppg-1.git
2. cd /api-uppg-1/
3. npm install
4. npm start

### GET /api/students
req:
```
curl localhost:3001/api/students | jq
```
res: 
```
  {
    "student": {
      "address": {
        "street": "gatasdaanf 22",
        "zipCode": "21313",
        "city": "lessadsebo"
      },
      "email": "bölagasd@asda.se",
      "name": "Nisadasse"
    },
    "_id": "5eb341797853cc16bcbd9665",
    "__v": 0
  },
  {
    "student": {
      "address": {
        "street": "gågatqweqweqeqweqweqqean 23",
        "zipCode": "21qweqwewqeqweqwe313",
        "city": "åmåqweqwewqeqweqeql"
      },
      "email": "tsqweqewqweqweqweqweqse",
      "name": "ingrid Oqwewqeqwewqeqweqwelsson"
    },
    "_id": "5eb3b1a02b32fb53a073b423",
    "__v": 0
  }
```




