---
description: JSX의 역사에 대하여.
layout:
  title:
    visible: false
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 📘 JSX의 역사

## React에서 JSX를 사용하는 목적

> &#x20; JSX 또는 **JavaScript XML**은 Facebook에서 자체 서비스 개발을 위해 React를 만들어내는 과정에서, 웹 UI의 구조를 더 잘 표현하려는 목적으로 탄생했었다. 그리고, UI 컴포넌트들을 정의하는 용도로만 쓰여왔던 과거와는 다르게, 최근에는 JavaScript의 범용적인 확장으로써 다양한 방식으로 활용되고 있다.



### &#x20;_Syntactic sugar_

&#x20; 보통 "문법적 설탕"으로 번역되는데, 프로그래밍 언어 측면에서 추가되는 기능이나 능력의 가미가 전혀 없는 상태에서 가독성이나 편리함 등을 위해 추가된 프로그래밍 언어의 문법을 뜻하는 말이다.

&#x20; React.createElement에 대한 "문법적 설탕"으로써 XML-like한 JSX 문법이 추가되었다.



### &#x20;_JSX Runtime_

&#x20; React 17에서 새로운 JSX Transform으로써 소개된 모듈인데, 기존의 JSX Transform 방식으로 JSX 문법을 사용하기 위해서 명시적으로 React 모듈을 추가해야 했던 단점 및 확장성을 고려해서 도입되었다.

&#x20; 오래된 JSX Transform 방식도 아직 유효하고, JSX 문법에도 차이가 없기 때문에, 기존 방식을 지속적으로 사용할 수도 있다.

{% tabs %}
{% tab title="기존 방식" %}
```javascript
import React from 'react';

function App() {
  return React.createElement('h1', null, 'Hello world');
}
```
{% endtab %}

{% tab title="새로운 방식" %}
```javascript
// Inserted by a compiler (don't import it yourself!)
import {jsx as _jsx} from 'react/jsx-runtime';

function App() {
  return _jsx('h1', { children: 'Hello world' });
}
```
{% endtab %}
{% endtabs %}



## React.createElement

:link: [https://react.dev/reference/react/createElement](https://react.dev/reference/react/createElement)
