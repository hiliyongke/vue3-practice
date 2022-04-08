<template>
  <ol>
    <li v-for="item in list" :key="item.msg" v-html="item.msg" />
  </ol>
</template>

<script>
export default {
  setup() {
    return {
      list: [
        {
          msg: "在前端领域中，tree-shaking指的是消除没被引用的模块代码，减少代码体积大小，以提高页面的性能。",
        },
        {
          msg: '<a href="https://v3.cn.vuejs.org/guide/migration/global-api-treeshaking.html" target="_blank">https://v3.cn.vuejs.org/guide/migration/global-api-treeshaking.html</a>',
        },
      ],
    };
  },
};
</script>
