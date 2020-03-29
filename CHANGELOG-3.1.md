# Running release notes for Craft Commerce 3.1

### Added
- Added variants GraphQL queries. 
- States can now be re-ordered. ([#1284](https://github.com/craftcms/commerce/issues/1284))
- Added `availableForPurchase` to product GraphQL fields and arguments.
- Added `defaultPrice` to product GraphQL fields and arguments.
- Added `craft\commerce\elements\Variant::getGqlTypeName()`.
- Added `craft\commerce\elements\Variant::gqlScopesByContext()`.
- Added `craft\commerce\elements\Variant::gqlTypeNameByContext()`.
- Added `craft\commerce\gql\arguments\elements\Variant`.
- Added `craft\commerce\gql\arguments\interfaces\Variant`.
- Added `craft\commerce\gql\arguments\queries\Variant`.
- Added `craft\commerce\gql\arguments\resolvers\Variant`.
- Added `craft\commerce\gql\arguments\types\elements\Variant`.
- Added `craft\commerce\gql\arguments\types\generators\VariantType`.

### Changed
- The amount of base discount in a discount action is now spread across the line items from highest priced to lowest.
- A line item‘s `price` and `salePrice` are now rounded before being multiplied by the quantity.
- Discount and Tax calculations are now more accurate.
- The commerceCurrency twig filter now rounds consistently with currency rounding
- Fixed an error that could occur when querying product GraphQL using product type. 