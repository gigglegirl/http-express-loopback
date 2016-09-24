# Model relations

1. Manually create relations

  i. [hasOne-belongsTo](hasOne-belongsTo)

    An owner can have only one pet.

    a. Add owners

    ```
    {
      "username": "yolodude",
      "name": "Yolo Swag"
    }
    ```

    ```
    {
      "username": "mick",
      "name": "Mick Jagger"
    }
    ```

    b. Add pets

    ```
    {
      "name": "Neo",
      "type": "cat"
    }
    ```
    ```
    {
      "name": "Bud",
      "type": "dog"
    }
    ```

    By adding a _belongsTo_ relation in the other model, the relation is acknowledged; so we can get details about the _owner_ from the _pet_ model. The next example shows what happens when a corresponding _belongsTo_ is not defined.

  ii. [hasMany](hasMany)

    An owner can have many pets.

  iii. [hasManyThrough](hasManyThrough)
  iv. [hasAndBelongsToMany](hasAndBelongsToMany)

2. Use the commandline tool

  ```
  slc loopback:relation
  ```

## Links

[Model definition file - relations](https://docs.strongloop.com/display/APIC/Model+definition+JSON+file#ModeldefinitionJSONfile-Relations)
[Relation generator](https://docs.strongloop.com/display/APIC/Relation+generator)

## License

[MIT](LICENSE)
