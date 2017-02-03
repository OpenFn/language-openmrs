Language OpenMRS
==============

Language Pack for building expressions and operations for working with
the [OpenMRS API](https://wiki.openmrs.org/display/docs/API).

Documentation
-------------

## Create new person

```js
person(
  fields(
    field("gender", "M"),
    field("names", function(state) {
      return [{
        "givenName": dataValue("form.first_name")(state),
        "familyName": dataValue("form.last_name")(state)
      }]
    })
  )
)
```

## Create new patient

```js
patient(
  fields(
    field("gender", "M"),
    field("names", function(state) {
      return [{
        "patient_id": dataValue("form.patientId")(state),
        "creator": dataValue("form.user")(state)
      }]
    })
  )
)
```


[Docs](docs/index)


Development
-----------

Clone the repo, run `npm install`.

Run tests using `npm run test` or `npm run test:watch`

Build the project using `make`.
