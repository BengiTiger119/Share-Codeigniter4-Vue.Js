<template>
  <div class="hello">
    <h3>{{ msg }}</h3>
    <a :href="'http://' + site">{{ site }}</a>
    <b>... Make Bengi</b>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
    site: String
  }
};
</script>

<style scoped>
h3 {
  margin: 27px 0 0;
  color: rgb(0, 119, 255);
  display: inline-block;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #006eff;
  margin-left: 1.5rem;
  margin-right: 1.5rem;
  font-weight: bold;
  text-decoration: none;
}
.hello {
  display: inline-block;
  vertical-align: top;
}
</style>
