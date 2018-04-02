
## 1. Load config variables from config file


__Properties.java__
```java
package com.tatarshaov.web.config;

import lombok.Getter;
import lombok.Setter;
import org.springframework.boot.context.properties.ConfigurationProperties;
import org.springframework.context.annotation.Configuration;

@Getter
@Setter
@Configuration
@ConfigurationProperties("soap.service")
public class Properties {
    public String url;
    public String refererUrl;
}
```

__application.properties__
```
soap.service.url=https://soap.domain.name
soap.service.refererUrl=http://myweb.domain.name
```
