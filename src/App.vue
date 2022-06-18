<template>
  <div id="app">
    <TreeView
      id="patientSampleTree"
      title="Patient Tree"
      :data="treedata.children"
    />
  </div>
</template>

<script>
import TreeView from "./components/TreeView";
import treedata from "./assets/data.json";

export default {
  name: "App",
  data() {
    return {
      treedata: treedata,
    };
  },
  components: {
    TreeView,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #252525;
  box-sizing: padding-box;
  padding: 1.5em;
}
</style>
