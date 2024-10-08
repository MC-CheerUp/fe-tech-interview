# 웹팩

최신 프런트엔드 프레임워크에서 가장 많이 사용되는 모듈 번들러 (Module Bundler)

## 모듈 이란?

- 프로그래밍 관점에서, 특정 기능을 갖는 작은 코드 단위를 의미한다.

- 웹팩에서 모듈은, 웹 애플리케이션을 구성하는 자원 을 의미한다. 
  - (HTML, CSS , JS, Image, Font 등)

## 모듈 번들러란?

> 웹 애플리케이션을 구성하는 자원을 모아, 하나의 파일로 병합 및 압축해주는 도구를 말한다.
> 
> `빌드`, `변환`, `번들링` 은 같은 의미로 사용된다.

# 왜 웹팩을 사용하는지?

- 페이지의 자원을 있는 그대로, 로드 혹은 다운로드 받을 경우 로딩 시간이 지나치게 커질 수 있어, 애플리케이션 성능에 문제가 생길 수 있다.

- 여러 파일을 하나로 병합 및 압축할 경우 서버로의 요청을 줄일 수 있어, 네트워크에 부담을 줄인다.
 

# 웹팩으로 해결하려는 문제점
- HTTP 요청 최소화
  - 브라우저 별로 서버로 전송하려는, HTTP 최대 요청 횟수에 제한이 있다.
  - HTTP 요청을 보내려면, TCP/IP 연결이 선행되어야 한다.

- Dynamic Loading & Lazy Loading
  - 동적으로 원하는 순간에 원하는 모듈을 로드하는 것은 어렵다.

# 웹팩의 4가지 속성

## entry
- 모듈 변환의 최초 진입점, JS 파일 경로

## output
- `빌드` 된 (= 웹팩이 적용된) 결과물의 파일 경로

## loader
- 로더는 JS 파일이 아닌 웹 자원(HTML, CSS, Images, Font 등) 을 변환할 수 있도록 한다.
- 로더의 적용순서는 오른쪽부터 왼쪽 순으로 순차적 적용이 이뤄진다.
- 자주 사용하는 로더로는 `babel-loader`, `CSS-loader`, `TS Loader` 등이 있다.

## plugin
-  웹팩의 기본적인 동작에 추가적인 기능을 제공하는 속성이다.
