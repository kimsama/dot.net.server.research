# dot.net.server.research

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

## Serialization

* [ZeroFomatter](https://github.com/neuecc/ZeroFormatter) - fast and Unity3D supported serialization library.

> Note that one of the widely used serialization library as a network protocol, [protobuf](https://github.com/google/protobuf) does not support inheritance.
