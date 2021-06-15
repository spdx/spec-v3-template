# hasBase

##Description

This is about the hasBase property.

## Metadata

SubclassOf: hasIngredient
Domain: Pizza
Range: PizzaBase


# hasIngredient

##Description

This is about the hasIngredient property.


# hasSpiciness

##Description

This is about the hasSpiciness property.

## Metadata

Domain: PizzaTopping
Range: Spiciness


# hasSpicinessPreference

##Description

This is about the hasSpicinessPreference property.

## Metadata

Domain: Customer
Range: Spiciness


# hasTopping

##Description

This is about the hasTopping property.

## Metadata

SubclassOf: hasIngredient
Domain: Pizza
Range: PizzaTopping

# isBaseOf

##Description

This is about the isBaseOf property.

## Metadata

SubclassOf: isIngredientOf
Domain: PizzaBase
Range: Pizza

# isIngredientOf

##Description

This is about the isIngredientOf property.


# isMilderThan

##Description

This is about the isMilderThan property.

## Metadata

Domain: Spiciness
Range: Spiciness




# isSpicierThan

##Description

This is about the isSpicierThan property.

## Metadata

Domain: Spiciness
Range: Spiciness


# isToppingOf

##Description

This is about the isToppingOf property.

## Metadata

SubclassOf: isIngredientOf
Domain: PizzaTopping
Range: Pizza


# purchasedByCustomer

##Description

This is about the purchasedByCustomer property.

## Metadata

Domain: Pizza
Range: Customer


# purchasedPizza

##Description

This is about the purchasedPizza property.

## Metadata

Domain: Customer
Range: Pizza

