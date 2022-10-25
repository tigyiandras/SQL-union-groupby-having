# SQL-union-groupby-having

1. Feladat
Az orders tábla ship_state_province mezőjének értékeit fésüld össze a customers tábla state_province mezőjének értékeivel úgy, hogy
- minden érték csak egyszer szerepeljen,

    SELECT ship_state_province FROM orders
    UNION
    SELECT state_province FROM customers; 
    
2. Feladat
A products táblában számold meg kategóriánként (category mező) a termékek számát!

    SELECT COUNT(category), category 
    FROM products 
    GROUP BY category; 
    
3. Feladat
A orders táblában számold meg városonként (ship_city mező) a rendelések számát!

    SELECT COUNT(ship_city), ship_city
    FROM orders
    GROUP BY ship_city;

4. Feladat
A customers táblából kérd le az ügyfelek számát városonként, ha az eléri legalább a 3-at!

    SELECT COUNT(city), city FROM customers GROUP BY citi HAVING COUNT(city) >=3;














































