<template>
  <div>
    <!-- <Compute /> -->
    <!-- <TwoWay /> -->
    <getter-setter />
  </div>
</template>

<script>
// import TwoWay from './components/TwoWay.vue';
// import Compute from './components/Compute.vue';
import GetterSetter from './components/GetterSetter.vue';
export default {
    name:"App",
    components: {
      // TwoWay,
      // Compute,
      GetterSetter,
    },
  }
</script>