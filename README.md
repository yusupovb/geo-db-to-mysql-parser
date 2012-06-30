# Geo databases to MySql database

A set of bash scripts to parse geo databases into mysql database

 * Automates the updating of geo databases
 * Supports MaxMind, GeoNames
 * Small and simple to customize scripts

## Requirements

 * mysql-server, mysql-client
 * wget
 * unzip, gunzip

## Usage

chmod +x script_name.sh
./script_name.sh mysql options

Example: ./geonames_admin1_codes.sh -uroot -pPASSWORD -h127.0.0.1

## Scripts description

### Geonames.org ###

geonames_allcountries.sh - all countries combined in one file

geonames_country.sh - features for country with iso code XX, structure similar to all countries file. You will be prompted for country code in script

geonames_cities1000.zip - all cities with a population > 1000 or seats of adm div (ca 80.000), see 'geoname' table for columns

geonames_cities5000 - all cities with a population > 5000 or PPLA (ca 40.000), see 'geoname' table for columns

geonames_cities15000 - all cities with a population > 15000 or capitals (ca 20.000), see 'geoname' table for columns

geonames_admin1_codes.sh - ascii names of admin divisions

geonames_alternate_names.sh - alternate names with language codes and geonameId
