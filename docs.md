---
title: Mysql data types
taxonomy:
    category: docs
metadata:
    description: ' Mysql Data Types '
    keywords: ' Mysql Data Types '
---	

|[fa icon=fa-user /]     | Shirisha Sunkara / tinitiate.com  |
|-------------------------------------------------------------|
|[fa icon=file-code-o /] | Mysql-data-types.sql

The following is a list of datatypes available in MySQL, which includes string,
 numeric, date/time, and large object datatypes.

#### Numeric Data Types              

 Numeric data types can be used exact number data type and approximate numeric 
 data types including integer, fixed-point and floating point. They can be added, 
 subtracted, multiplied, and divided.   

##### The following table shows you the summary of numeric types in MySQL: 
 
|Data type  | Description |length (Bytes)| Range Low(signed) | Range High(signed) |Range Low(unsigned)|Range High (unsigned)|
|-----------|-------------|-------| ----------|------------|
|TINYINT	|A very small integer.  |1|-128	     |127       |0|255|
|SMALLINT	|A small integer.       |2|-32768	 |32767     |0|65535|
|MEDIUMINT	|A medium size integer. |3|-8388608  |8388607   |0|16777215|
|INT	    |A standard integer.    |4|-2147483648|2147483647|0|4294967295|     
|BIGINT	    |A large integer.       |8|-922337203<br>6854775808|92233720368<br>54775807|0|18446744<br>073709551615|
|DECIMAL(m,d)|A fixed decimal point number.<br>Where m is the total digits and d is the number of digits after the decimal. |Length+1 or<br> Length+2 bytes| | | | |
|FLOAT	    |A single precision floating point number. |4| -3.402823<br>466E+38 |-1.175494345<br>1E-38 | 1.1754943<br>51E-38|3.4028234<br>66E+38|    
|DOUBLE	    |A double precision floating point number.|8| -1.79769313486<br>23157E+308 |-2.2250738<br>585072014E-308 | 0, and 2.225073<br>8585072014E- 308|1.79769313<br>48623157E+ 308

#### String Data Types

In MySQL, a string can hold anything from plain text to binary data such as images and files. 

##### The following table shows you the string data types in MySQL:

|Data type | Description | Size |Range in Characters|
|----------|-------------|------|--------|
|CHAR	   |A fixed-length nonbinary string.    |string length             | The length can be any value from 0 to 255|
|VARCHAR   |A variable-length non-binary string.|string length+<br>1bytes  |The length can be any value from 0 to 255|
|TINYTEXT  |A very small non-binary string.     |string length+<br>1bytes  |A string with a maximum length of 255 characters|
|TEXT	   |A small non-binary string.          |String length+<br>2 bytes |A string with a maximum length of 65,535 characters|
|MEDIUMTEXT|A medium size non-binary string.    |String length+<br>3 bytes |A string with a maximum length of 16,777,215 characters|
|LONGTEXT  |A large non-binary string.          |String length+<br>4 bytes |A string with a maximum length of 4,294,967,295 characters|
|BINARY	   |Contains binary strings.            |string length+<br>1bytes  |The length can be any value from 0 to 255|
|VARBINARY |Contains binary strings.            |string length+<br>1bytes  |The length can be any value from 0 to 255|

#### Date and Time Data Types

MySQL provides types for date and time as well as a combination of date and time. 
In addition, MySQL supports timestamp data type for tracking the changes of a 
row in a table. If you just want to store the year without date and month, you 
can use YEAR data type.

##### The following table illustrates the MySQL date and time data types:

|Date and Time Data type | Description| Size(Bytes)|
|------------------------|------------|-----|
|DATE	  |A date value in ‘YYYY-MM-DD’ format.                  | 3 Bytes|
|TIME	  |A time value in ‘hh:mm:ss’ format.                    | 3 Bytes|
|YEAR	  |A year value in YYYY or YY format,acceptable range in the year '1901' to '2155'.| 2 digits or<br> 4 digits|                    | 
|DATETIME |A date and time value in ‘YYYY-MM-DD hh:mm:ss’ format.| 8 Bytes|
|TIMESTAMP|A timestamp value in the format of YYYY-MM-DD HH:MM:SS ,acceptable range ends in the year 2037.|4 Bytes |





