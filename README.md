SELECT DISTINCT TOP (100) NickName, UserName, SUM(Money) AS Expr1
FROM            Charge_Money
WHERE        (MONTH(Date) = 11) AND (DAY(Date) >= 28) AND (MONTH(Date) = 04) AND (DAY(Date) <= 12)
GROUP BY NickName, UserName
ORDER BY Expr1 DESC
