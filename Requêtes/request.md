## Request :

PREFIX schema: <https://schema.org/>

SELECT ?city (COUNT(?transaction) AS ?numTransactions)
WHERE {
  ?transaction a schema:PurchaseAction ;
               schema:location ?loc .
  ?loc schema:name ?city .
}
GROUP BY ?city
ORDER BY DESC(?numTransactions)
LIMIT 1

### Result :
Sydney,128

## Request :

PREFIX schema: <https://schema.org/>
PREFIX foaf: <http://xmlns.com/foaf/0.1/>

SELECT ?memberTier (COUNT(?transaction) AS ?numTransactions)
WHERE {
  ?transaction a schema:PurchaseAction ;
               schema:customer ?cust .
  ?cust schema:memberTier ?memberTier .
}
GROUP BY ?memberTier
ORDER BY DESC(?numTransactions)
LIMIT 1

### Result :
Bronze,808

