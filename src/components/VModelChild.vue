<template>
  <div style="border: 1px orange solid">
    <input
      type="text"
      :value="modelValue"
      @input="$emit('update:modelValue', $event.target.value)"
    />
    <br />
    <input
      type="text"
      :value="text"
      @input="$emit('update:text', $event.target.value)"
    />
  </div>
</template>
<script>
export default {
  //v-model冒号后面不写值，默认就是modelValue
  props: ["modelValue", "text"],
};
</script>
