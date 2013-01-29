# Mantle

Just a regular Mantle with additional Rails date formatter, no need to write own
MTLValueTransformer. If you've got createdAt property that is NSDate and is generated
by date string provided by Rails simply use:

```objc
+ (NSValueTransformer *)createdAtTransformer
{
    return [NSValueTransformer valueTransformerForName:MCRailsDateValueTransformerName];
}
```
