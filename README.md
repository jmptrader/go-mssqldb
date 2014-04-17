# A pure Go MSSQL driver for Go's database/sql package

## Install

    go get github.com/denisenkom/go-mssqldb

## Tests

`go test` is used for testing. A running instance of MSSQL server is required.
Environment variables are used to pass login information.

Example:

    env HOST=localhost SQLUSER=sa SQLPASSWORD=sa go test

## Connection Parameters

* server - host or host\instance
* user id
* password
* database

Example:

    db, err := sql.Open("mssql", "server=localhost;user id=sa")

## Features

* Can be used on linux and on Mac OS X
* Supports new date/time types: date, time, datetime2, datetimeoffset
* Supports string parameters longer that 8000 characters
