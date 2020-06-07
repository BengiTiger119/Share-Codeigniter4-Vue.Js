# CodeIgniter 4.0.4 + Vue-Cli 4.4.1

---

## 개발시

- cd vuejs

- npm run serve

- 브라우져 접속 .. http://localhost:8080/

- 현재 샘플 결과 화면

![serve](https://user-images.githubusercontent.com/15817249/83961216-fa562b00-a8cb-11ea-8bda-4122ecefc891.jpg)

---

## Codeigniter View 에 삽입

- cd vuejs

- npm run buildv ( production 으로 파일 생성 )

  - 생성되는 결과 디렉토리 : /public/dist
  - VueJs 수정시 **npm run buildv** 을 다시 해주셔야 합니다.

- View 적용 위치 : /app/Views/welcome_message.php

```html
<html>
  <body>
    <!-- ----------------- 원하시는 위치에  3 라인 추가 시작 -->

    <div id="appvue">
      <app></app>
    </div>

    <!-- ----------------- 원하시는 위치에  3 라인 추가 끝 -->

    <br />
    <br />
    <br />
    <br />
    <br />

    <!-- ----------------- 제일 아래 페이지에 추가 시작 -->

    <script src="https://unpkg.com/vue"></script>
    <script src="/dist/vuejs.umd.js"></script>
    <script>
      new Vue({
        components: {
          app: vuejs,
        },
      }).$mount("#appvue");
    </script>

    <!-- ----------------- 제일 아래 페이지에 추가 끝 -->
  </body>
</html>
```

- 현재 샘플 결과 화면

![2](https://user-images.githubusercontent.com/15817249/83961228-13f77280-a8cc-11ea-8851-93a49fa438a0.jpg)

---

## 디렉토리

![7](https://user-images.githubusercontent.com/15817249/83961830-0d6bf980-a8d2-11ea-9059-c6ccc485e5fc.jpg)

---

## 간단 설명

- Vue 개발후, Ci 에 나오는 결과 화면을 보시면 됩니다.

  - npm run serve ( vue 작업시 )
  - npm run buildv ( Codeigniter 적용 )

- Vue-Cli 을 이용해서 설치

- Vue.js 설치후 사용하는 방법과 완전히 동일

- Vuejs 디렉토리 : 순수 소스 원본 자체

- VueJs 안에 사용한 css 은 별도로 생성하지 않고, js 안에 포함

  - 기본 설정은 별도 분리지만, 처음 하시는분들을 위해 포함

- 한번에 위의 개발과 빌드 작업이 편하게 가능하지만, 처음하시는분들에게 복잡하게 할것 같아 제외
