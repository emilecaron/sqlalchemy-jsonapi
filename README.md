# SQLAlchemy-JSONAPI: *Ember-data compat*
Forked from https://github.com/ColtonProvias/sqlalchemy-jsonapi

The goal of this fork is to achieve [Ember-data](https://github.com/emberjs/data) compatibility, using the new default JSONApi adapter.
This requires many small tweaks, mostly around the serializer.

### Build status
[![Build Status](https://travis-ci.org/emilecaron/sqlalchemy-jsonapi.svg?branch=master)](https://travis-ci.org/emilecaron/sqlalchemy-jsonapi)

### Key changes:
* Expect and send dash case in data, while models fields are still declared using underscore case
* Tolerance for data fields missing in the model: skip it instead of raising an error
