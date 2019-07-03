[TOC]

# jap

- 按实际打开了
- 看手机阿里的

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<body>
aaaa
</body>
</html>
```

```java
package com.example.mysecond.controller;

import com.example.mysecond.domain.Computer;
import com.example.mysecond.domain.ComputerReposity;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.data.jpa.repository.Query;
import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.PostMapping;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

import java.util.Map;

@Controller
public class tcontroller {

    @Autowired
    private ComputerReposity computerReposity;
    @PostMapping("addComputer")
    public void addComputer(Computer computer){
        computerReposity.save(computer);
    }
    @RequestMapping("daa")
    public String daa(Map<String ,Object> map){
        Computer computer = new Computer();
        computer.setCname("aaa");
        map.put("name","zhang");
        return  "index.html";
    }
}

```

## 法兰克苏建大佬课教案可视对讲

#### 接口六角恐龙

