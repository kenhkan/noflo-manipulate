# Advanced manipulation of objects, packets, and groups in NoFlo <br/>[![Build Status](https://secure.travis-ci.org/kenhkan/noflo-manipulate.png?branch=master)](http://travis-ci.org/kenhkan/noflo-manipulate) [![Dependency Status](https://gemnasium.com/kenhkan/noflo-manipulate.png)](https://gemnasium.com/kenhkan/noflo-manipulate) [![NPM version](https://badge.fury.io/js/noflo-manipulate.png)](http://badge.fury.io/js/noflo-manipulate) [![Stories in Ready](https://badge.waffle.io/kenhkan/noflo-manipulate.png)](http://waffle.io/kenhkan/noflo-manipulate)

This package contains more arcane manipulation of objects, packets, and groups
in NoFlo. Core packages like `noflo-objects`, `noflo-packets`, and
`noflo-groups` should not depend on other packages so this package is created
to contain graphs that depend on multiple packages.

## Usage

### GroupValueByAnother

Take in an object, extract some value by key and group that with another value
of the object.

In-ports

* `GROUPING`: The key of the value to be used for the group
* `ENCLOSED`: The key of the value to be grouped
* `IN`: Take in a JavaScript object

Out-ports

* `OUT`: The enclosed value grouped by the grouping value
