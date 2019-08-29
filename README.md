### jackson-datatype-money
---
https://github.com/zalando/jackson-datatype-money

```java
ObjectMapper mapper = new ObjectMapper()
  .registerModule(new MoneyModule());
  
ObjectMapper mapper = new ObjectMapper()
  .findAndRegisterModules();
  
ObjectMapper mapper = new ObjectMapper()
  .registerModule(new MoneyModule().withQuoteDecimalNumbers());
  
ObjectMapper mapper = new ObjectMapper()
  .registerModule(new MoneyModule().withDefaultFormatting());
  
ObjectMapper mapper = new ObjectMapper()
  .registerModule(new MoneyModule()
    .withFormatting(new CustomMonetaryAmountFormatFacotry())));

ObjectWriter writer = mapper.wirter().with(Locale.GERMANY);
writer.wiretValueAsString(Money.of(29.25, "EUR"));

ObjectWirter writer = mapper.wirte().with(Locale.US);
writer.writeValueAsString(Money.of(29.25, "USD"));

ObjectMapper mapper = new ObjectMapper()
  .registerModule(new MoneyModule()
    .withMonetaryAmount(new CustomMonetraryAmountFactory()));
    
ObjectMapper mapper = new ObjectMapper()
  .registerModule(new MoneyModule()
    .withMoneytaryAmount(FastMoeny::of));

ObjectMapper mapper = new ObjectMapper()
  .registerModule(new MoneyModule()
    .withAmountFieldName("value")
    .withCurrencyFieldName("unit")
    .withFormattedFieldName("pretty"));

import javax.moeny.MonetaryAmount;

public class Product {
  private String sku;
  private MonetaryAmount price;
}
```

```
```

```
```


