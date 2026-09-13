Jakie zagrożenia powinienem uwzględnić, kiedy testuję formularz kontaktowy?

Przyjmij rolę profesjonalnego testera oprogramowania i zasugeruj listę zagrożeń związanych z formularzem kontaktowym, używając następujących ograniczeń:
# Skup się na cechach jakościowych, takich jak dostępność, zgodność z przepisami i użyteczność
# Ponumeruj zagrożenia
# Poinformuj, której cechy jakościowej dotyczy zagrożenie
# Opisz każde zagrożenie najwyżej w 30 słowach

Na przykład:
1 Struktura semantyczna – Dostępność – Struktura HTML formularza powinna spełniać standardy WCAG A

Jesteś generatorem danych SQL. Wygeneruj pięć wierszy kodu SQL dla bazy danych MySQL.
* Nazwa tabeli jest określona przez znak #.
* Każda kolumna tabeli jest określona przez znak %.
* Każda kolumna jest opisana w kolejności: nazwa, typ danych i opcje danych z użyciem znaku |
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

Utwórz obiekt JSON z losowymi danymi, który zawiera następujące pola: firstname, lastname, totalprice, deposit_paid. Dołącz też obiekt o nazwie booking_dates, który zawiera daty zameldowania (checkin) i wymeldowania (checkout)

Utwórz ten obiekt w formacie YAML

Otrzymasz obiekt JSON ograniczony trzema haszami. Wyodrębnij wszystkie adresy e-mail kończące się na .com i zapisz je jako listę.
Jeśli nie istnieje adres e-mail zakończony na .com, po prostu napisz: „Nie znaleziono adresów .com”
###
[{
  "firstname": "Bret",
  "lastname": "Averay",
  "email": baveray0@apple.com
 }, {
  "firstname": "Annabel",
  "lastname": "Biswell",
  "email": abiswell2@nsw.gov.au
 },{
  "firstname": "Pavel",
  "lastname": "Itzhaki",
  "email": pitzhaki3@pagesperso-orange.fr
 },{
  "firstname": "Pail",
  "lastname": "Yandell",
  "email": "pyandell4@ning.com"
 }, {
  "firstname": "Glennis",
  "lastname": "Pentecost",
  "email": "gpentecost6@yelp.com" }]
###

Otrzymasz obiekt JSON ograniczony trzema haszami. Wyodrębnij wszystkie adresy e-mail kończące się na .com i zapisz je jako listę.
Jeśli nie istnieje adres e-mail zakończony na .com, po prostu napisz: „Nie znaleziono adresów .com”
###
[{
"firstname": "Bret",
"lastname": "Averay"
}, {
"firstname": "Annabel",
"lastname": "Biswell"
}, {
"firstname": "Pavel",
"lastname": "Itzhaki"
}, {
"firstname": "Pail",
"lastname": "Yandell"
}, {
"firstname": "Glennis",
"lastname": "Pentecost"
}]
###

Jesteś ekspertem w zakresie testowania eksploracyjnego. Utwórz trzy karty testowe dla systemu rezerwacji, które skupiają się na ryzyku związanym z datami rezerwacji. Format powinien być następujący: Eksploruj <Cel> z użyciem <Zasób>, aby odkryć <Informacje>
Na przykład:
* Eksploruj uprawnienia użytkowników z użyciem różnych kont użytkowników, aby odkryć zagrożenia związane z uprawnieniami
* Eksploruj animacje przeglądarki za pomocą różnych urządzeń, aby odkryć, jak renderowane są animacje

Otrzymasz listę instrukcji do wykonania.
1 Zidentyfikuj zagrożenia funkcjonalne, które mogą dotyczyć tekstu ograniczonego trzema haszami
2 Przekształć zagrożenia w karty testowe
3 Sformatuj każdą kartę w następujący sposób: Sprawdź <funkcja> z użyciem <zasób>, aby zweryfikować <informacje>
###
Jako użytkownik
Chcę móc obliczyć mój podatek
Żebym wiedział, jaki podatek muszę zapłacić
###

Jesteś doświadczonym programistą Javy pracującym w dziale testów. Utwórz test jednostkowy dla następującej metody:
public class AuthService {
 
    public HttpStatus deleteToken(Token token) throws SQLException {
        Boolean successfulDeletion = authDB.deleteToken(token);
        if(successfulDeletion){
            return HttpStatus.OK;
        } else {
            return HttpStatus.NOT_FOUND;
        }
    }
}

Jesteś doświadczonym programistą Javy pracującym w dziale testów. Utwórz test jednostkowy dla zamieszczonej niżej metody. Zanim wypiszesz testy jednostkowe, sprawdź, czy asercja w każdym teście zwraca deterministyczny wynik.
public class AuthService {
 
    public HttpStatus deleteToken(Token token) throws SQLException {
        Boolean successfulDeletion = authDB.deleteToken(token);
        if(successfulDeletion){
            return HttpStatus.OK;
        } else {
            return HttpStatus.NOT_FOUND;
        }
    }
}
