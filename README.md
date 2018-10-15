# Elastic Stack

This brings up a full `ELK` stack with 2 indexes.
 
Data imported from specified mysql tables  with `Logstash` on 2 `jdbc` pipelines described in `./logstash/pipelines.yml`

This is a `quick and dity` set up. You will need to provide some additional configuration as indicated below.

## Requirements

* docker ce 18.x

* mysql db running on `localhost:3306` with the specified schema

## Set Up

* run `docker compose build`

## Running

* `docker compose up`

## Stopping

* `docker compose down`

## Additional config:

1. `conf_a.config` and `conf_b.config` contain variables like `index_a`, `schema` and `db_table`, replace these with appropriate values

## Note:

* Elastic search available on port `9200`
* Kibana available on port `5601`
