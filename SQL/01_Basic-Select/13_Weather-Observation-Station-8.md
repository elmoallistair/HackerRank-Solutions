[comment]: <> (Written: 23-Mar-2020)

<b>TASK<b>
> Query the list of CITY names from STATION which have vowels (i.e., a, e, i, o, and u) as both their first and last characters. Your result cannot contain duplicates.
>
> Station's Table: 
> | Field  | Type         |
> |--------|--------------|
> | ID     | NUMBER       |
> | CITY   | VARCHAR2(21) |
> | STATE  | VARCHAR2(2)  |
> | LAN_N  | NUMBER       |
> | LONG_W | NUMBER       |

<b>SOLUTION (MySQL)</b>
> SELECT DISTINCT(city) FROM station WHERE city REGEXP '^[aeiou].+[aeiou]$';<br><br>
> [Reference](https://www.tutorialspoint.com/mysql/mysql-regexps.htm)