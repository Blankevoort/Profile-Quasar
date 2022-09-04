<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <q-toolbar class="bg-primary text-white shadow-2">
        <q-img
          src="../assets/images/LinkedIn-Logo.png"
          class="bg-white"
          style="width: 24px; height: 24px"
        />

        <q-input
          dark
          dense
          standout
          v-model="text"
          input-class="text-right"
          class="q-ml-md"
        >
          <template v-slot:append>
            <q-icon v-if="text === ''" name="search" />
            <q-icon
              v-else
              name="clear"
              class="cursor-pointer"
              @click="text = ''"
            />
          </template>
        </q-input>

        <q-space />

        <q-btn stretch flat label="Link" />

        <q-btn stretch flat label="Link" />

        <q-separator dark vertical />

        <q-btn stretch flat label="Link" />
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "MainLayout",

  setup() {
    return {};
  },
});
</script>
