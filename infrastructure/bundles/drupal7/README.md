# Drupal bundle

This section contains information related to the bundle for [Drupal 7 websites](../../../apps/drupal/README.md). 

## Services

| Service | Available containers | Mandatory |
| --------------------- | ---------------------------------------------- | - |
| Backend               | [Nginx-php](../../containers/nginx-php/README.md) | ✓ |
| Database              | [MariaDB](../../containers/mariadb.md)            | ✓ |
| Cache storage         | [Redis](../../containers/redis.md)                |   |
| Search engine         | [Solr](../../containers/apache-solr.md)           |   |
| Database management   | [PhpMyAdmin](../../containers/phpmyadmin.md)      |   |
| Reverse caching proxy | [Varnish](../../containers/varnish.md)            | &nbsp; |

## Changelog

* [v3.1.0](#v310)
    * [Changes since v3.0.0](#changes-since-v300)
    * [Upgrade policy](#upgrade-policy-v310)
* [v3.0.0](#v300)

### v3.1.0

Minimal [server infrastructure version](../../versioning.md) v3.0.0 is required.

#### Changes since v3.0.0

* [Nginx](../../containers/nginx-php/nginx.md) upgraded to 1.10.1 
* [PHP 5.6](../../containers/nginx-php/php.md) upgraded to 5.6.22
* [Postfix](../../containers/nginx-php/postfix.md) upgraded to 3.1.1
* [MariaDB](../../containers/mariadb.md) upgraded to 10.1.14
* [Redis](../../containers/redis.md) upgraded to 3.2.0
* Default option `always_populate_raw_post_data = -1` added to php.ini of [PHP 5.6](../../containers/nginx-php/php.md) 
* Added mysql_extension (in addition to mysqli_extension) to [PHP 5.6](../../containers/nginx-php/php.md)
* Fixed the bug in all [PHP containers](../../containers/nginx-php/php.md) with an incorrect value of `error_reporting` for dev instances 

Release date: `June 24th, 2016`

#### Upgrade policy v3.1.0

[Contact our support team](../../../product/support.md) to schedule the upgrade. Instance downtime ~10 minutes.

### v3.0.0

Initial bundle version.