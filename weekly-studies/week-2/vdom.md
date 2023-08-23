---
description: VDOM(Virtual DOM)에 대하여.
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

# 📘 VDOM

## DOM이란?

&#x20; JavaScript와 관련된 웹 브라우저의 개념으로써, Document Object Model의 두문자어이다. W3C의 표준 규격으로 정립되어 있으며, HTML과 같은 웹 문서의 구조를 JavaScript의 객체로써 다룰 수 있게 해준다.

&#x20; 각 구성 요소는 트리와 노드들로 이루어진 계층적 구조로써 설명될 수 있다.



## DOM과 Virtual DOM의 차이

### &#x20;_정의_

&#x20; React에게 있어서, VDOM(Virtual DOM)은 React Element 트리 구조를 포함하면서, DOM 구조와 긴밀한 관계를 가지는 개념으로써 설명될 수 있다.



### &#x20;_기능_

&#x20; React Element들에 변화가 생길 때마다 웹 브라우저에서 전체 DOM의 구조를 다시 렌더링하는 것은 굉장히 비효율적이다.

&#x20; React의 Virtual DOM을 쓰면 이러한 변화들을 React Element 트리 구조(i.e. VDOM 구조)에 우선 반영한 후, 이전 상태의 트리 구조와의 차이를 분석해서 효율적으로 실제 DOM 트리를 변경할 수 있게 된다.
