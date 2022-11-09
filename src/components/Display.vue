<template>
  <input type="text" class="calc--screen" />
</template>

<script>
export default {
  name: "Screen",
};
</script>

<style scoped>
.calc--screen {
  font-family: "Orbitron", sans-serif;
  font-size: 200%;
  text-align: right;
  color: greenyellow;
  background-color: black;
  border: 1px solid greenyellow;
  margin-bottom: 10px;
  width: 100%;
  height: 2em;
  padding: 10px;
  outline: none;
  cursor: pointer;
}
</style>
