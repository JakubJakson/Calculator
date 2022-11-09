<template>
  <Container />
</template>
<script>
import Container from "./components/Calc-container.vue";
export default {
  name: "App",
  components: { Container },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=M+PLUS+Rounded+1c:wght@500&family=Montserrat&family=Orbitron:wght@400;500;600;900&family=Poppins:wght@400;600;700&family=Roboto:wght@300;400;500;700;900&display=swap");

html {
  box-sizing: border-box;
}
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}
body {
  background-color: rgb(50, 50, 50);
}
</style>
