# CodeIgniter 4.0.4 + Vue-Cli 4.4.1

### Sorry. The problem that the vue development screen did not appear was solved and applied on June 6, 2020. ( UTC :  June 5, 2020 )

---

## When developing ( bug fix : 2020.06.09 )

- cd vuejs

- npm install

- npm run serve

- Brower Connect : http://localhost:8080/

- Current sample results screen

![serve](https://user-images.githubusercontent.com/15817249/83961216-fa562b00-a8cb-11ea-8bda-4122ecefc891.jpg)

---

## Insert in Codeigniter View

- cd vuejs

- npm run buildv ( Production file creation  )

  - Resulting directory generated : /public/dist
  - When modifying VueJs : You have to do " npm run buildv " again.

- View Apply Location : /app/Views/welcome_message.php

```html
<html>
  <body>
    <!-- ----------------- Start adding 3 lines to the desired location -->

    <div id="appvue">
      <app></app>
    </div>

    <!-- ----------------- End adding 3 lines to the desired location -->

    <br />
    <br />
    <br />
    <br />
    <br />

    <!-- ----------------- Start adding at the bottom of the page -->

    <script src="https://unpkg.com/vue"></script>
    <script src="/dist/vuejs.umd.js"></script>
    <script>
      new Vue({
        components: {
          app: vuejs,
        },
      }).$mount("#appvue");
    </script>

    <!-- ----------------- End adding at the bottom of the page -->
  </body>
</html>
```

- Current sample results screen

![2](https://user-images.githubusercontent.com/15817249/83961228-13f77280-a8cc-11ea-8851-93a49fa438a0.jpg)

---

## Directory

![7](https://user-images.githubusercontent.com/15817249/83961830-0d6bf980-a8d2-11ea-9059-c6ccc485e5fc.jpg)

---

## Brief Description

- After Vue development, you can see the result screen shown in Ci.

  - npm run serve ( when working with vue )
  - npm run buildv ( Apply Codeigniter )

- Installation using Vue-Cli

- It is exactly the same as the method used after installing Vue.js.

- Vuejs Directory : Pure source original itself

- Css used in VueJs is not created separately, but included in js

  - The default setting is separate, but included for first-time users


[![Epic Short Film](https://img.youtube.com/vi/lMj4APUZ1oU/0.jpg)](https://www.youtube.com/watch?v=lMj4APUZ1oU?t=0s "REMEMBERING THE FALLEN")


