### modelmapper
---
https://github.com/modelmapper/modelmapper

```java
// core/src/test/java/org/modelmapper/functional/converter/CustomConversion.java
package org.modelmapper.functional.converter;

import org.modelmapper.*;
import org.modelmapper.spi.MappingContext;
import org.testng.annotations.BeforeMethod;
import org.testng.annotations.Test;

import static org.testng.Assert.assertEquals;

public class CustomConversion {
  @Test(groups = "functional")
  public static class When_using_member_converter extends AbstractTest {
    private ModelDTO result;
    
    public static class ModelObject {
      int value1 = 42;
      int value2 = 42;
      
      public int getValue2() {
        return value2;
      }
    }
    
    public static class ModelDTO {
      int value1;
      int value2;
      
      public void setValue2(int value2) {
        this.value2 = value2;
      }
    }
    
    Converter<Integer, Integer> converter1 = new AbstractConverter<Integer, Integer>() {
      public Integer converter(Integer source) {
        return source + 1;
      }
    };
    
    
    
    
  }
}


```

```
```

```
```
