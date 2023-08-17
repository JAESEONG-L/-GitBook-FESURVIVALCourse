---
description: React에 대하여.
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

# 📘 React

## React란?

&#x20; 자바스크립트 라이브러리의 하나로써, 사용자 인터페이스를 만들기 위해 사용된다. 페이스북과 개별 개발자 및 기업들 공동체에 의해 유지보수된다.\
[**<1> https://en.wikipedia.org/wiki/React\_(software)**](https://en.wikipedia.org/wiki/React\_\(software\))



## React 컴포넌트

### &#x20;정의

&#x20; React를 사용해서 UI를 개발하는 도구이자 애플리케이션을 이루는 구성 요소로써, 상위 컴포넌트 아래에 하위 컴포넌트들이 존재하는 구조로 이루어져 있다. 각각의 컴포넌트들은 최대한 독립적으로 기능할 수 있도록 설계되어야 하며, 상호의존성을 줄임으로써 향후에 자유롭게 수정하거나 더 작은 단위의 컴포넌트들로 재구성할 수 있도록 만들어야 한다.



### &#x20;컴포넌트의 특징

> #### 내용물

<table data-view="cards"><thead><tr><th></th><th></th><th data-hidden data-card-cover data-type="files"></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td></td><td>Data passed to the component from a parent component.</td><td><a href="../../.gitbook/assets/React Props.png">React Props.png</a></td><td><a href="https://www.w3schools.com/react/react_props.asp">https://www.w3schools.com/react/react_props.asp</a></td></tr><tr><td></td><td>Internal data specific to a component.</td><td><a href="../../.gitbook/assets/State and Lifecycle.png">State and Lifecycle.png</a></td><td><a href="https://legacy.reactjs.org/docs/state-and-lifecycle.html">https://legacy.reactjs.org/docs/state-and-lifecycle.html</a></td></tr></tbody></table>

> #### 함수 컴포넌트와 클래스 컴포넌트

&#x20; Hooks가 도입되기 전에, 클래스 컴포넌트는 React에서 State 및 Lifecycle Method들을 처리하는 주된 방법으로 쓰여 왔습니다.



{% code title="컴포넌트의 예 (함수 컴포넌트)" %}
```javascript
function Car() {
  return <h2>Hi, I am a Car!</h2>;
}
```
{% endcode %}

***



{% code title="컴포넌트의 예 (클래스 컴포넌트)" %}
```javascript
class Car extends React.Component {
  render() {
    return <h2>Hi, I am a Car!</h2>;
  }
}
```
{% endcode %}



## IoC(Inversion of Control)

&#x20; 컴포넌트를 \<Car />와 같이 사용할 수 있는 것과 관련있다. :bookmark\_tabs:<mark style="color:green;background-color:orange;">**추가 계획중.**</mark>
