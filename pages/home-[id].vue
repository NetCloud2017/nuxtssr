<script>
import { reactive, toRefs } from "vue";
import { useRoute } from "~/.nuxt/vue-router";
export default {
  setup() {
    const state = reactive({
      count: 0,
    });
    let route = useRoute();
    console.log(route.params.id, "id");
    return {
      ...toRefs(state),
    };
  },
};
</script>

<template>
  <div>home</div>
</template>
