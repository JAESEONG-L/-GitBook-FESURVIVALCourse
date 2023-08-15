---
description: 개발 환경에 대하여.
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

# 📘 개발 환경

## Node.js

&#x20; 과거의 웹 브라우저 환경에서, 주로 동적인 기능을 실행시키기 위해서 개발되었던 언어가 JavaScript였기 때문에 JavaScript의 런타임 환경은 웹 브라우저에만 국한되어 있었다.

&#x20; 웹 브라우저의 개발사들이 제각각 브라우저의 성능 향상을 목적으로 인터프리터 엔진을 개발 및 발전시켜 왔는데, Chrome의 V8 엔진도 그것들 중에 하나이며 동 엔진을 웹 브라우저 환경에 국한되지 않고 다양한 용도로 활용하기 위해 꺼내 놓은 것이 Node.js Runtime Environment.



## Shell and Terminal

&#x20; OS의 구성요소들 중, Kernel은 소프트웨어 프로세스가 하드웨어 자원들을 이용할 수 있도록 인터페이스 역할을 수행한다. 개발자들이 작업을 하기 위해서는 OS와 끊임없이 소통해야 하는데, 이때 사용하는 CLI 기반 애플리케이션이 바로 Terminal.

&#x20; Shell의 역할은 OS의 가장 바깥쪽 껍질으로써, Kernel을 비롯한 OS의 구성요소들을 감싸는 인터페이스이기 때문에 위에서 설명한 Terminal의 개념과 일맥상통한다. 하지만 Terminal은 컴퓨터의 역사를 통틀어 사람과 컴퓨터 간의 상호 작용이 이루어지는 폭넓은 의미로 통해 왔다면, Shell은 현대 운영체제들을 구성하고 있는 소프트웨어 요소라는 더 구체적인 개념인 것 같다.



## NPM(Node Package Manager)

### &#x20;정의

&#x20; 말 그대로 Node.js를 기반으로 개발하는 프로젝트를 패키지로써 관리하기 위한 프로그램이다.



### &#x20;package.json / package-lock.json

&#x20; package.json 파일은 "npm init" 명령으로 프로젝트를 초기화하는 과정에서 생성되며, 프로젝트와 관련된 메타데이터들을 포함하고 있을 뿐만 아니라 의존성 목록**(Dependencies)**, 그리고 개발 과정에서 필요로 하는 툴 등의 개발의존성 목록**(DevDependencies)**을 저장해 놓고 있다.

&#x20; 개발 및 배포, 그리고 테스트를 위해 자동화 스크립트를 package.json 파일에 미리 작성한 후, "npm run" 명령을 Terminal에 입력해서 실행시킬 수 있다. 한편, package-lock.json 파일의 주요한 역할은 프로젝트의 복잡한 의존성을 보다 엄격하게 관리함으로써, 프로젝트의 일관성을 유지하면서 개발 및 배포를 진행할 수 있도록 하는 것이다.



### &#x20;node\_modules

&#x20; 위에서 살펴봤던 package-lock.json 파일에서 프로젝트의 의존성을 보다 엄격하게 관리한다고 했던 수단 중에 하나가, 바로 node\_modules 폴더의 구조를 똑같이 저장해 놓는 것이라고 한다.

&#x20; node\_modules 폴더는 "npm install" 명령을 사용해서 모듈, 혹은 의존성이 생기게 되면 저장 공간으로써 생성되고 유지된다. 결과적으로, 개발을 진행하기 위해 필요한 의존성들을 패키지 내부에 둠으로써 효율적인 모듈 사용이 가능하다는 이점을 활용할 수 있다.



## ES Modules vs CommonJS

&#x20; Java의 Class나 Python의 Module과 유사한, JavaScript의 서로 다른 두 종류의 모듈 체계.
