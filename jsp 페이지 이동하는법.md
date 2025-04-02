```Java
package com.example.demo;

import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.GetMapping;

@org.springframework.stereotype.Controller
public class Controller {

    @GetMapping("/")
    public String home(){
        return "index";
    }

    @GetMapping("page1")
    public String page1(Model model){
        model.addAttribute("seoyeon", "안녕");
        return "page1";
    }

    @GetMapping("page2")
    public String page2(){
        return "page2";
    }

}

```

model이 뭔진 모르겠는데 1번째가 키값이고 2번째가 값이다.

이걸 JSP의 ${}문법에 키값을 넣어서 "안녕"이라는 텍스트를 가지고 올 수 있다.

```html
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<html>
<head>
    <title>Title</title>
</head>
<body>
  <h1>페이지 1입니다.</h1>
${seoyeon}
</body>
</html>

```