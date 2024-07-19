# SQL Data Type

SQL data types define the type of value that can be stored in a table column. For example, if you want a column to store only integer values, you can define its data type as `int`.

SQL data types can be broadly divided into the following categories.

1. **Numeric** data types such as : `int`, `tinyint`, `bigint`, `float`, `real`, etc.
2. **Date** & **Time** data types such as : `date`, `time`, `datetime`, etc.
3. **Character** & **String** data types such as : `char`, `varchar`, `text`, etc.
4. **Unicode character string** data types such as : `nchar`, `nvarchar`, `ntext`, etc.
5. **Binary** data types such as : `binary`, `varbinary`, etc.
6. **Miscellaneous** data types - `clob`, `blob`, `xml`, `cursor`, `table`, etc.

## SQL Numeric Data Types

| Data Type | From | To |
| --- | --- | --- |
| `bit` | 1 | 0 |
| `tinyint` | 0 | 255 |
| `smallint` | -32768 | 32767 |
| `int` | -2,14,74,83,648 | 2,14,74,83,647 |
| `bigint` | -9,223,372,036,854,775,808 | 9,223,372,036,854,775,807 |
| `decimal` | -10^38 + 1 | 10^38 - 1 |
| `numeric` | -10^38 + 1 | 10^38 - 1 |
| `float` |	-1.79E+308 | 1.79E+308 |
| `real` | -3.40E+38 | 3.40E+38 |

## SQL Date & Time Data Types

| Data Type | Description |
| --- | --- |
| `date` | Stores date in the format `YYYY-MM-DD` |
| `time` | Stores time in the format `HH:MI:SS` |
| `datetime` | Stores date and time information in the format `YYYY-MM-DD HH:MI:SS` |
| `timestamp` | Stores number of seconds passed since the Unix epoch (`'1970-01-01 00:00:00' UTC`) |
| `year` | Stores year in a 2-digit or 4-digit format. Range 1901 to 2155 in 4-digit format. Range 70 to 69, representing 1970 to 2069 |

## SQL Character & String Data Types

| Data Type | Description |
| --- | --- |
| `char` | Fixed length with a maximum length of 8,000 characters |
| `varchar`	| Variable-length storage with a maximum length of 8,000 characters |
| `varchar(max)` | Variable-length storage with provided max characters |
| `text` | Variable-length storage with a maximum size of 2GB data |

## SQL Unicode Character & String Data Types

| Data Type | Description |
| --- | --- |
| `nchar` | Fixed length with a maximum length of 4,000 characters |
| `nvarchar` | Variable-length storage with a maximum length of 4,000 characters |
| `nvarchar(max)` | Variable-length storage with provided max characters |
| `ntext` | Variable-length storage with a maximum size of 1GB data |

## SQL Binary Data Types

| Data Type | Description |
| --- | --- |
| `binary` | Fixed length with a maximum length of 8,000 bytes |
| `varbinary` | Variable-length storage with a maximum length of 8,000 bytes |
| `varbinary(max)` | Variable-length storage with provided max bytes |
| `image` | Variable-length storage with a maximum size of 2 GB binary data |

## SQL Miscellaneous Data Types

| Data Type | Description |
| --- | --- |
| `clob` | Character large objects that can hold up to 2 GB |
| `blob` | For large binary objects |
| `xml` | For storing XML data |
| `json` | For storing JSON data |