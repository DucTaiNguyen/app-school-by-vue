<template>
  <div id="app">
    <Statistics />
  </div>
</template>

<script>
import Statistics from "./components/Statistics";

export default {
  name: "App",
  components: {
    Statistics,
  },
};
</script>

<style>
:root {
  --dl-color-gray-white: #fff;
  --dl-color-success-700: #00997a;
  --dl-space-space-halfunit: 0.5rem;
  --dl-space-space-unit: 1rem;
  --dl-space-space-doubleunit: 2rem;
  --dl-space-space-tripleunit: 3rem;
  --main-cl: #263b6e;
  --red-cl: #9c1a07;
}
#app {
}
</style>
