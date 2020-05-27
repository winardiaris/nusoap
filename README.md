<h1 align=center>NuSOAP - Custom</h1>

<p align=center>
NuSOAP is a rewrite of SOAPx4, provided by NuSphere and Dietrich Ayala. It is a set of PHP classes - no PHP extensions required - that allow developers to create and consume web services based on SOAP 1.1, WSDL 1.1 and HTTP 1.0/1.1.
</p>

<p align=center>
🕹 <a href="http://www.winardiaris.xyz/">winardiaris</a>
</p>

<p align=center>
  All credits belongs to official authors, take a look at <a href="https://sourceforge.net/projects/nusoap/">sourceforge.net/projects/nusoap/</a>
</p>

<p align=center>
    <a href="https://travis-ci.org/winardiaris/nusoap"><img src="https://img.shields.io/travis/winardiaris/nusoap.svg?style=flat-square"></a>
    <a href="https://packagist.org/packages/winardiaris/nusoap"><img src="https://img.shields.io/packagist/l/winardiaris/nusoap.svg?style=flat-square"></a>
    <a href="https://packagist.org/packages/winardiaris/nusoap"><img src="https://img.shields.io/packagist/dt/winardiaris/nusoap.svg?style=flat-square"></a>
    <a href="https://packagist.org/packages/winardiaris/nusoap"><img src="https://img.shields.io/packagist/v/winardiaris/nusoap.svg?style=flat-square"></a>
</p>

---

## Versions

| State       | Version       | Branch    | PHP      |
| ----------- | ------------- | --------- | -------- |
| stable      | `~0.9.7.1`    | `master`  | `>= 5.4` |
| development | `dev-develop` | `develop` | `>= 5.6` |

## Installation

To install this pkg use Composer.

```sh
composer require winardiaris/nusoap
```

### `Stable`

Solid rock version is `~0.9.7`.

```sh
composer require winardiaris/nusoap
```

### `Development`

Total refactored version (split into more files, CI, etc).

```json
{
  "require": {
    "econea/nusoap": "dev-develop"
  },
  "minimum-stability": "dev",
  "prefer-stable": true
}
```

## Usage

```php
// Config
$client = new nusoap_client('example.com/api/v1', 'wsdl');
$client->soap_defencoding = 'UTF-8';
$client->decode_utf8 = FALSE;

// Calls
$result = $client->call($action, $data);
```

## Experimental

Take a look at `develop` branch. There will be new features and modernizations.

Minimal version is set to PHP 5.6.

```sh
composer require winardiaris/nusoap:dev-develop
```

## Help

[![Join the chat](https://img.shields.io/gitter/room/econea/econea.svg?style=flat-square)](http://bit.ly/ecogitter)

## Maintainers

<table>
  <tbody>
    <tr>
      <td align="center">
        <a href="https://nusoap.sourceforge.net">
            <img width="150" height="150" src="https://via.placeholder.com/320x320?text=NuSOAP">
        </a>
        </br>
        <a href="https://nusoap.sourceforge.net">NuSOAP</a>
      </td>
      <td align="center">
        <a href="https://github.com/f3l1x">
            <img width="150" height="150" src="https://avatars2.githubusercontent.com/u/538058?v=3&s=150">
        </a>
        </br>
        <a href="https://github.com/f3l1x">Milan Felix Šulc</a>
      </td>
    </tr>
  <tbody>
</table>

---

Thank you for testing, reporting and contributing.
