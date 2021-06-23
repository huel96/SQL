# `SQL`

`SELECT *` 
`from [Order Details] od`
`LEFT OUTER JOIN Products p on p.ProductID = od.ProductID` 

`SELECT *`
`from [Order Details] od`
`LEFT JOIN Products p on od.ProductID = p.ProductID`
`WHERE Discontinued = 1`

`SELECT CompanyName as 'Customer'`
`FROM Customers`
`Left JOIN Orders on Orders.CustomerID = Customers.CustomerID`
`WHERE Orders.CustomerID is NULL`

`select top 2 UnitPrice,` 
`Quantity,` 
`Discount,` 
`UnitPrice*Quantity as 'Gross Total', 
UnitPrice*Quantity*(1- Discount) as 'Net Total'` 
`from [Order Details]` 
`order by 'Net Total' DESC`

