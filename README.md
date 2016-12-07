# dot.net.server.research

A brief of research for open source based backend system for a game server which is much suitable on cloud environment like aws or azure.

## Server

front-end socket server with *supersocket* and *orleans* for logic framwork combination seems to be a considerable server-side solution.

### [orleans](https://github.com/dotnet/orleans)

* [orleans](https://github.com/dotnet/orleans) - looks better than Akka.Net as an actor framework.

### [supersocket](https://github.com/kerryjiang/SuperSocket)

* [supersocket](https://github.com/kerryjiang/SuperSocket) seems to be available  being used as front-end socket server with orleans. It supports TCP, UDP even Websocket.

## Database

Some of libraries which prevents from doing tedious and dirty job on SQL database such as writing sql-query, stored-procedure etc.

### [Dapper](https://github.com/StackExchange/dapper-dot-net)

* [Dapper](https://github.com/StackExchange/dapper-dot-net) - a simple object mapper for .Net which make it easy to access Sql server without complex POCO and stored-procedure.
  * See also other Dapper related projects such as Dapper.Extension, Dapper.Extention.Linq and so on.
* ~~[How to use Dapper with Linq](http://stackoverflow.com/questions/38826292/how-to-use-dapper-with-linq): stackoverflow thread.~~
  * See [Dapper.Contrib](https://github.com/StackExchange/dapper-dot-net/tree/master/Dapper.Contrib) which contains a number of helper methods for inserting, getting, updating and deleting records.

### [SQLinq](https://sqlinq.codeplex.com/)

Easily generate ad-hoc SQL code using LINQ in a strongly typed manner that allows for compile time validation of sql scripts.

### [linq2db](https://github.com/linq2db/linq2db)

looks simple but it requires POCO.

### Excel with SQL 

* [Excel data files with Microsoft SQL Server Integration Services](http://dougbert.com/blog/post/excel-in-integration-services-part-1-of-3-connections-and-components.aspx) - series of posts about working with Excel and MS-SQL.
* [How to Import an Excel Spreadsheet into a SQL Server Database Table Using the SQL Server Import and Export Wizard](http://www.66pacific.com/sql_server_import_from_excel.aspx)

### Tools

* [LinqPad](https://www.linqpad.net/) - enables doing query via LINQ.
* Tools written with Go language
  * [sql2xlsx](https://github.com/bwmarrin/sql2xlsx) - A simple program to convert SQL rows into Microsoft Excel XLSX files.
  * [go-mssqldb](https://github.com/denisenkom/go-mssqldb) - A pure Go MSSQL driver for Go's database/sql package
  * [xlsx](https://github.com/tealeg/xlsx) - xlsx is a library to simplify reading and writing the XML format used by recent version of Microsoft Excel in Go programs.

### Database-Drivers

...

## Serialization

* [ZeroFomatter](https://github.com/neuecc/ZeroFormatter) - fast and Unity3D supported serialization library.

> Note that one of the widely used serialization library as a network protocol, [protobuf](https://github.com/google/protobuf) does not support inheritance.

Also need some sorta of data tracking code such as waht Torque-Network-Engine does for its serialization. (instead of sending whole object but only serializing changed data)

## Etc

* [Unity Networking Extension](https://bitbucket.org/Unity-Technologies/networking) - bitbucket project page. It contains client side network syncronization code such as history based interpolation and extrapolation.
