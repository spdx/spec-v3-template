# Notes on the spec

- Model and profiles are in separate directories
- Namespaces are in separate directories inside the model
- Classes are written in PascalCase, properties are in camelCase.

- Refer to other elements in running text by using `@Element` or `@Namespace:Element`.

## Explanations

### "Properties"

OWL has "object properties" and "data properties".
Object properties are relationships between two entities
and data properties are relations between an entity and a data type
(like `xsd:string`).

To understand these, the following presents rough equivalents
in Entity-Relationship and Object Oriented models:

OWL| object properties | data properties
--- | --- | ---
E-R| relations | attributes
OOP| range is class | range is datatype

As an example, think of something like "a person has a gender",
which in E-R might be implemented as
"the class `Person` has an attribute `gender`".

In OWL, a model might be:
there are classes `Person` and `Gender`
and an object property `hasGender` that connects
a Person with a Gender.
The property (hasGender) has a domain (Person) and a Range (Gender).
One can also think of an inverse property,
with domain and range exchanged;
in this case a property `isGenderOf` connecting a Gender to a Person.

The same way classes may be subclasses of other classes,
property may be subproperties of other properties.
Think of classes like `Father` and `Parent`
and of properties like `hasFather` and `hasParent`.

In writing the specification, object properties
are all placed in a separate file `properties.md`.
Datatype properties are placed in the class.

### Enumerated classes

When a property has a (small) finite set of possible values,
it can be useful to create a class to represent those values.
The class is general, but each of the values is a separate instance.

In writing the specification, instances are listed
in a separate section in the class file.

