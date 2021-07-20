
# Defaults

The simplified input format does not need to include _all_ information,
since some can be generated with processing.
When omitting field values,
the following defaults are implied (and generated automatically).

## For classes

### in Metadata

- (name: the name of the class -- top header in the file) ?
- id: `${NAMESPACE_id}/${NAME_OF_CLASS}`
- Instantiability: Concrete
- Status: Stable

### in Properties

- minCount: 0
- maxCount: *

## For properties

### in Metadata

- (name: the name of the property -- top header in the file) ?

## For vocabularies

### in Metadata

- (name: the name of the property -- top header in the file) ?

