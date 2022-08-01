<template>
  <div id="#test">
    <input v-model="value" />
    <input type="checkbox" id="one" value="one" v-model="checkedName" />
    <label for="one">ONE</label>
    <input type="checkbox" id="TWO" value="TWO" v-model="checkedName" />
    <label for="TWO">TWO</label>
    <input type="checkbox" id="THERE" value="THERE" v-model="checkedName" />
    <label for="THERE">THERE</label>
    <input type="checkbox" id="FOUR" value="FOUR" v-model="checkedName" />
    <label for="FOUR">FOUR</label>
    <br />
    <span>Write: {{ value }}</span>
    <br />
    <span>Check: {{ checkedName }}</span>
  </div>
</template>

<script>
import { defineComponent } from "vue";

const TypeTest = defineComponent({
  id: "#test",
  data() {
    return { value: "", checkedName: [] };
  },
});

export default TypeTest;
</script>
