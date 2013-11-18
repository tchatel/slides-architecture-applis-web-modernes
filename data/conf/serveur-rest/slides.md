!SLIDE subsection ====================================================================================

# API REST


!SLIDE bullets ============================

# REpresentational State Transfer

* sans état
* mise en cache
* ressources

!SLIDE bullets ============================

# URI

* /users/123/cards
* /users/123/cards/456

!SLIDE bullets ============================

# HTTP request method

* GET _(safe)_ : récupère une ressource ou une collection
* PUT _(idempotent)_ : met à jour une ressource
* DELETE _(idempotent)_ : supprime une ressource
* POST : ajoute une ressource à une collection, fait une opération sur une ressource

!SLIDE bullets ============================

# retour du serveur

* status HTTP
* données de la ressource

!SLIDE bullets ============================

# exemples de requêtes

* GET /users/123/cards
* GET /users/123/cards/456
* GET /users/123/cards?status=active
* POST /users/123/cards
* PUT /users/123/cards/456
* POST /users/123/cards/456?action=charge&amount=9.99



!SLIDE ============================

# JSON
## vs
# XML / SOAP

!SLIDE ============================

# XML / SOAP

    <?xml version="1.0"?>
    <soap:Envelope
         xmlns:soap="http://www.w3.org/2003/05/soap-envelope">
      <soap:Header>
      </soap:Header>
      <soap:Body>
        <m:GetStockPrice
             xmlns:m="http://www.example.org/stock">
          <m:StockName>IBM</m:StockName>
        </m:GetStockPrice>
      </soap:Body>
    </soap:Envelope>

![](dinosaure-minuscule.png)

!SLIDE ============================

# JSON

    {"stockName": "IBM"}

!SLIDE image ============================

![](monitoring.png)


