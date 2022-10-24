<template>
  <AppLayout title="component">
    <template #header>
      <h2 class="font-semibold text-xl text-gray-800 leading-tight">
        component
      </h2>
    </template>

    <div class="py-12 min-h-screen">
      <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
        <div class="bg-white overflow-hidden shadow-xl sm:rounded-lg">
          <div>
            <p>{{ firstName }}</p>
            <button
              type="button"
              class="outline-1 bg-slate-500 hover:bg-amber-600 w-12 text-white"
              @click="testLog"
            >
              Click
            </button>
          </div>
        </div>
      </div>
    </div>
  </AppLayout>
</template>

<script>
import { defineComponent } from "vue";

import AppLayout from "@/Layouts/AppLayout.vue";
import { ref } from "vue";
// const firstName = ref("");

export default defineComponent({
  components: {
    AppLayout,
  },
  props: {},
  created() {},
  mounted() {},
  data() {
    return {
      firstName: "anders",
    };
  },
  methods: {
    testLog() {
      console.log("hello world");
    },
  },
});
</script>

<style>
#app {
  max-width: 450px;
  margin: 60px auto;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>