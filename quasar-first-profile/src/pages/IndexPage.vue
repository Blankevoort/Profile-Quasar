<template>
  <q-page>
    <div class="flex justify-center items-center gt-md">
      <q-bar class="bg-white" style="width: 80%; height: 50px">
        <div class="text-weight-regular q-pr-md q-pl-none">
          <span class="material-symbols-outlined text-h5"> home </span>Home
        </div>
        <div class="q-ml-md text-weight-regular q-px-md">
          <span class="material-symbols-outlined text-h5"> group </span
          >MyNetwork
        </div>
        <div class="q-ml-md text-weight-regular q-px-md">
          <span class="material-symbols-outlined text-h5">
            business_center </span
          >Jobs
        </div>
        <div class="q-ml-md text-weight-regular q-px-md">
          <span class="material-symbols-outlined text-h5"> chat </span>Messages
        </div>

        <q-space></q-space>

        <div class="text-amber-9 text-weight-regular q-mr-md">
          Try Premium For Free
        </div>
      </q-bar>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",
});
</script>
