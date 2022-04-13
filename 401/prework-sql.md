# SQL Practice
*This is a summary from [SQLBolt](sqlbolt.com)*


Structured Query Language (SQL) is a search language to instruct a relational database what information to retrieve.

* There are many popular SQL databases including SQLite, MySQL, Postgres, Oracle and Microsoft SQL Server. All of them support the SQL language standard. *

Information is organized into tables.

SELECT is the first instruction of any SQL statement that’s fetching data.

Each query needs to end in a semi-colon.

FROM

SELECT [column] FROM [table];

/* Splat is a shortcut to get all columns.

ORDER BY [desired column]

ASCending and DESCending

LIMIT
SELECT * FROM [table] LIMIT [Number to Limit By];

SCHEMA describes a collection of tables and their relationships in the database.

WHERE
SELECT * FROM [table] WHERE [Filter Conditions];

AND - Requiring Multiple Conditions
OR - Requiring Any Condition
NOT -  invert a condition
Ordering and Parenthesis - use parenthesis to specify the order of operations

Operators: = < > <= >= != <>

String operators and Patterns
LIKE - string matches a pattern
ILIKE  - case insensitive version of LIKE
SIMILAR TO - string matches a regex pattern

IS NULL - NULL values
IS NOT NULL - non NULL values

Functions
List of the most commonly used functions in SQL.

MAX - largest (maximum) number in a set
MIN - smllest number in a set
COUNT - # of values in a set
COUNT DISTINCT - # of unique (distinct) values in a set
EVERY - true if all data inside is true (same as bool_and)
AVG - average (mean) of a set of numbers
SUM - sum all values in a set

