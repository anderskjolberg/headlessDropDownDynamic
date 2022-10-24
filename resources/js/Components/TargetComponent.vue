<script setup>

import Dropdown from "./DropListHeadless.vue";
import {ref} from "vue";
 
const people = [
  {value: 1, label: "Option 1"},
  {value: 2, label: "Option 2"},
  {value: 3, label: "Option 3"},
  {value: 4, label: "Option 4"},
  {value: 5, label: "Option 5"},
  {value: 6, label: "Option 6"},
];

const form = ref({
  person_id: null,
  role_ids: []
});

</script>

<template>
  <div>
    <div class="p-6 sm:px-20 bg-white border-b border-gray-200">
      <Dropdown
        id="target"
        placeholder="Select person"
        v-model="form.person_id"
        :options="people"
      />
    </div>
  </div>
</template>
<script>
import { defineComponent } from "vue";

export default defineComponent({
  setup() {},
  mounted() {},
  props: {},
  data() {
    return {};
  },
  methods:{
    testLog(){
      
    }
  }
});
</script>
