# SQL

SELECT * 
from [Order Details] od
LEFT OUTER JOIN Products p on p.ProductID = od.ProductID 

SELECT *
from [Order Details] od
LEFT JOIN Products p on od.ProductID = p.ProductID
WHERE Discontinued = 1

SELECT CompanyName as 'Customer'
FROM Customers
Left JOIN Orders on Orders.CustomerID = Customers.CustomerID
WHERE Orders.CustomerID is NULL