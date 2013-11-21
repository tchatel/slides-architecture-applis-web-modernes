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

* <span class="red">GET</span> _(safe)_</span>
    <span class="small"> : récupère une ressource ou une collection</span>
* <span class="red">PUT</span> _(idempotent)_
    <span class="small"> : met à jour une ressource</span>
* <span class="red">DELETE</span> _(idempotent)_
    <span class="small"> : supprime une ressource</span>
* <span class="red">POST</span>
    <span class="small"> : ajoute une ressource à une collection, fait une opération sur une ressource</span>

!SLIDE bullets ============================

# retour du serveur

* status HTTP
* données de la ressource

!SLIDE bullets small ============================

# <span class="bigger">exemples de requêtes</span>

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


