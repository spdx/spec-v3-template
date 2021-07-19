# Element

## Summary

Base domain class from which all other SPDX-3.0 domain classes derive.

## Description

An Element is a representation of a fundamental concept either directly inherent
to the Bill of Materials (BOM) domain or indirectly related to the BOM domain
and necessary for contextually characterizing BOM concepts and relationships.
Within SPDX-3.0 structure this is the base class acting as a consistent,
unifying, and interoperable foundation for all explicit
and inter-relatable content objects.

## Metadata

- name: Element
- SubclassOf: none
- Instantiability: Abstract

## Properties

| property    | type         | minCount | maxCount | format |
| ----------- | ------------ | -------- | -------- | ------ |
| id          | idString     | 1        | 1        |        |
| name        | xsd:string   |          | 1        |        |
| summary     | xsd:string   |          | 1        |        |
| description | xsd:string   |          | 1        |        |
| comment     | xsd:string   |          | 1        |        |
| specVersion | xsd:string   |          |          |        |
| createdTime | xsd:dateTime |          |          |        |
| createdBy   | Identity     |          |          |        |
| profile     | ProfileIdentifier | 1   |          |        |
| dataLicense | xsd:string   |          |          |        |
| profile     | ProfileIdentifier | 1   |          |        |
| externalReference | ExternalReference | 0 | *    |        |
| extension   | Extension    | 0        | *        |        |
| verifiedUsing | IntegrityMethod |     |          |        |
