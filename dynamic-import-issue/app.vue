<script setup>
const dynamicVariable = "infos";
const importedComponent = defineAsyncComponent(() =>
  import(`./dynamic/${dynamicVariable}.vue`)
);
</script>

<template>
  <Component :is="importedComponent" />
</template>
