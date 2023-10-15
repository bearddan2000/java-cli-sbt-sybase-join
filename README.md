# java-cli-sbt-sybase-join

## Description
Creates a small database table
called `dog`. This table, `dog`, has 2 non-clustered
index and has been normalized to 3NF.

Two new tables have been added, `breedLookup` and `colorLookup`.
Creates a new table `dog_expanded` that joins
`dog`, `breedLookup` and `colorLookup`.

## Tech stack
- docker-wait
- java
- sbt
  - log4j
  - sybase driver

## Docker stack
- hseeberger/scala-sbt:11.0.2-oraclelinux7_1.3.5_2.12.10
- datagrip/sybase

## To run
`sudo ./install.sh -u`

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`

## Credit
- [Sybase driver and connection example](https://razorsql.com/docs/help_sybase.html)
