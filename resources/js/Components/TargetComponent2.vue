<script setup>

import Dropdown from "./DropMenuHeadless.vue";
import {ref} from "vue";
 
const links = [
    { href: '/account-settings', label: 'Account settings' },
    { href: '/support', label: 'Support' },
    { href: '/license', label: 'License' },
    { href: '/sign-out', label: 'Sign out' },
  ]

const form = ref({
  menu_id: null,
  link_id: []
});

</script>

<template>
  <div>
    <div class="p-6 sm:px-20 bg-white border-b border-gray-200">
      <Dropdown
        placeholder="Select person"
        v-model="form.menu_id"
        :options="links"
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
});
</script>
