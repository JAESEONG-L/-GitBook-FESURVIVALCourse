---
description: React Element에 대하여.
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

# 📘 React Element

## React Element 트리

&#x20; React 애플리케이션의 구조를 표현하는 데 사용되는 개념이다.

&#x20; React에서, UI는 React Element들로 구성되며, 이러한 Element들은 트리 구조로 구성되어 화면에 렌더링 된다. React의 렌더링 엔진은 이 Element 트리를 사용하여 실제 DOM 트리를 생성하고, 필요할 때마다 업데이트한다.



## 정의

&#x20; React.createElement 또는 JSX 문법을 사용하여 만들어지는 객체로써, DOM 구조에 반영되어 브라우저에 드러나는 성분에 대한 정보들(성질들)을 가지고 있다. 앞서 공부했었던 React Component의 근본적인 역할이 바로 새로운 React Element를 제작하는 것이다.

&#x20; 이렇게 만들어진 React Element들은 ReactDOM 모듈 등을 사용해 Virtual DOM 구조에 반영되고, 궁극적으로는 실제 DOM과 렌더링 결과에 반영된다.
