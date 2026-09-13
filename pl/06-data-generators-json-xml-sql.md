Jesteś generatorem danych JSON. Utwórz tablicę zawierającą 5 obiektów JSON i sprawdź, czy rzeczywiście zostało utworzonych 5 obiektów JSON, zanim wypiszesz wyniki.
* Każdy parametr jest oznaczony znakiem %.
* Każda kolumna jest opisana w kolejności: klucz, typ danych i opcje, przy użyciu znaku |.
* Jeśli opcją danych jest random, generuj losowe dane na podstawie sugerowanego formatu i nazwy kolumny
Oto instrukcje:
% room_name | string | random
% type | string | 'single' or 'double'
% beds | integer | 1 to 6
% accessible | boolean | true or false
% image | string | random url
% description | string | random max 20 characters
% features | array[string] | 'Wifi', 'TV' or 'Safe'
% roomPrice | integer | 100 to 200

Jesteś generatorem danych XML. Utwórz tablicę zawierającą 3 obiekty XML i sprawdź, czy rzeczywiście zostały utworzone 3 obiekty XML, zanim wypiszesz wyniki.
* Nazwa elementu głównego jest oznaczona znakiem #
* Każdy element jest oznaczony znakiem %
* Każda kolumna jest opisana w kolejności: nawa elementu, typ danych i opcje, przy użyciu znaku |.
* Jeśli opcją danych jest random, generuj losowe dane na podstawie sugerowanego formatu i nazwy kolumny
Oto instrukcje:
# rooms
% room_name | string | random
% type | string | 'single' or 'double'
% beds | integer | 1 to 6
% accessible | boolean | true or false
% image | string | random url
% description | string | random max 20 characters
% features | array[string] | 'Wifi', 'TV' or 'Safe'
% roomPrice | integer | 100 to 200

Jesteś transformatorem JSON na SQL. Przekształć obiekt JSON ograniczony trzema haszami w instrukcję SQL, która:
1 Tworzy tabelę SQL do wstawienia przekształconych rekordów
2 Tworzy instrukcje INSERT dodające poszczególne rekordy do bazy danych
Przed wypisaniem wyników sprawdź, czy każda instrukcja SQL uwzględnia wszystkie aspekty pliku JSON
###
[{
    "firstname": "Sally",
    "lastname": "Wilson",
    "totalprice": 229,
    "depositpaid": false,
    "bookingdates": {
        "checkin": "2017-02-20",
        "checkout": "2019-07-05"
    },
    "additionalneeds": "Breakfast"
},...]
###

Jesteś generatorem danych JSON. Wygeneruj tablicę JSON zawierającą 3 losowe obiekty JSON zgodne ze schematem OpenAPI ograniczonym trzema haszami. Przed wypisaniem wyników upewnij się, że wszystkie 3 obiekty JSON są zgodne z regułami schematu OpenAPI.
###
openapi: 3.0.0
components:
  schemas:
    Room:
      title: Room
      type: object
      properties:
        accessible:
          type: boolean
        description:
          type: string
        type:
          type: string
          pattern: Single|Double|Twin|Family|Suite
        features:
          type: array
          items:
            type: string
            pattern: WiFi|TV|Radio|Refreshments|Safe|
        image:
          type: string
        roomNumber:
          type: string
        roomPrice:
          type: integer
          format: int32
          minimum: 0
          maximum: 999
          exclusiveMinimum: true
          exclusiveMaximum: false
        roomid:
          type: integer
          format: int32
      required:
        - accessible
        - description
        - features
        - image
        - roomNumber
        - roomPrice
###

(Further JSON/XML/SQL generator examples and contact form test code preserved in original format)
