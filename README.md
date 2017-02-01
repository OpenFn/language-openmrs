Language OpenMRS
==============

Language Pack for building expressions and operations for working with
the [OpenMRS API](https://wiki.openmrs.org/display/docs/API).

Documentation
-------------

## Create a new person
```js
person({
 name: dataValue(form.name),
 date_of_birth: dataValue(form.dob)
})
```

## Create a new patient
```js
patient({
 name: dataValue(form.name),
 date_of_birth: dataValue(form.dob)
})
```

[Docs](docs/index)


Development
-----------

Clone the repo, run `npm install`.

Run tests using `npm run test` or `npm run test:watch`

Build the project using `make`.
