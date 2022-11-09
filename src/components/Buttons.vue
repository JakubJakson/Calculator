<template>
  <div class="btn--container">
    <!-- Operators -->
    <button class="btn btn--plus" ref="plus">+</button>
    <button class="btn btn--minus" ref="minus">-</button>
    <button class="btn btn--multiply" ref="multi">X</button>
    <button class="btn btn--devide" ref="dev">/</button>

    <!-- Numbers -->
    <button @click="onClick()" class="btn btn--num" value="0" ref="button">
      0
    </button>
    <button @click="onClick()" class="btn btn--num">1</button>
    <button @click="onClick()" class="btn btn--num">2</button>
    <button @click="onClick()" class="btn btn--num">3</button>
    <button @click="onClick()" class="btn btn--num">4</button>
    <button @click="onClick()" class="btn btn--num">5</button>
    <button @click="onClick()" class="btn btn--num">6</button>
    <button @click="onClick()" class="btn btn--num">7</button>
    <button @click="onClick()" class="btn btn--num">8</button>
    <button @click="onClick()" class="btn btn--num">9</button>

    <!-- Misc -->
    <button class="btn btn--decimal" ref="deci">.</button>
    <button class="btn btn--reset" id="C">C</button>
    <button class="btn btn--compute" id="compute">=</button>
  </div>
</template>

<script>
export default {
  name: "Buttons",
  props: {},
  methods: {
    onClick() {
      console.log(this.$refs.button.value);
    },
  },
};
</script>

<style>
.btn--container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-row-gap: 10px;
  grid-column-gap: 10px;
  width: 20em;
}
.btn {
  font-size: 150%;
  border-radius: 2px;
  border: 1px solid greenyellow;
  color: greenyellow;
  background-color: black;
  height: 3em;
  cursor: pointer;
}
.btn--compute {
  background-color: greenyellow;
  color: black;
  font-weight: 800;
  grid-column-start: 2;
  grid-column-end: 4;
}
</style>
