# Restrictions for making the information accceptable

## Valid SSN for employees

### Description

All employees must have a valid SSN.

### Shape
- Class: Employee
- Property: ssn
- MinCount: 1
- MaxCount: 1
- Pattern: "^\\d{3}-\\d{2}-\\d{4}$"

## Phone for employees

### Description

All employees must have a phone number.

### Shape
- Class: Employee
- Property: hasPhone
- MinCount: 1

## Valid discounts

### Description

Discounts for all customers must be between 0% and 100%.

### Shape
- Class: Customer
- Property: hasDiscount
- MinInclusive 0.0
- MaxInclusive 1.0

