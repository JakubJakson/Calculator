<template>
  <div class="main--container">
    <Screen />
    <Buttons />
  </div>
</template>

<script>
import Buttons from "./Buttons.vue";
import Screen from "./Display.vue";

export default {
  name: "Container",
  components: { Buttons, Screen },
};
</script>

<style scoped>
.main--container {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 20em;
}
</style>
