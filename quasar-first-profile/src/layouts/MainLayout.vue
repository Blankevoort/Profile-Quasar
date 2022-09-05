<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <div class="flex justify-center items-center gt-md">
        <q-toolbar class="bg-primary text-white" style="width: 80%">
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
            input-class="text-left"
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

          <q-tabs
            v-model="tab"
            class="text-white"
            indicator-color="transparent"
          >
            <q-route-tab
              to="notif"
              name="mails"
              icon="notifications"
              label="Notifications"
            />
            <q-tab to="apps" name="alarms" icon="apps" label="Work" />
          </q-tabs>

          <q-separator dark vertical />

          <q-item clickable v-ripple>
            <q-item-section>
              <div class="q-ml-md">
                <q-item-label overline
                  ><q-img
                    src="../assets/images/LinkedIn-Logo.png"
                    class="bg-white"
                    style="width: 35px; height: 35px; border-radius: 50%"
                /></q-item-label>
                <q-item-label>Profile</q-item-label>
              </div>
            </q-item-section>

            <q-menu>
              <q-list dense style="min-width: 100px">
                <q-item
                  v-for="n in 1"
                  :key="n"
                  dense
                  clickable
                  class="text-center"
                >
                  <q-item-section>Logout</q-item-section>
                </q-item>
              </q-list>
            </q-menu>
          </q-item>
        </q-toolbar>
      </div>

      <div class="flex justify-center items-center lt-md">
        <q-toolbar class="bg-primary text-white">
          <q-img
            src="../assets/images/LinkedIn-Logo.png"
            class="bg-white"
            style="width: 24px; height: 24px"
          />

          <q-space />

          <q-btn flat round @click="toggleRightDrawer" icon="menu" />

          <q-drawer
            show-if-above
            v-model="rightDrawerOpen"
            side="right"
            bordered
            class="bg-primary"
          >
            <q-input
              dark
              standout
              v-model="text"
              input-class="text-left"
              class="q-ma-lg"
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

            <q-item clickable v-ripple>
              <q-item-section>
                <div class="q-ml-md">
                  <q-item-label overline
                    ><q-img
                      src="../assets/images/LinkedIn-Logo.png"
                      class="bg-white"
                      style="width: 35px; height: 35px; border-radius: 50%"
                  /></q-item-label>
                  <q-item-label>Profile</q-item-label>
                </div>
              </q-item-section>

              <q-menu>
                <q-list dense style="min-width: 100px">
                  <q-item
                    v-for="n in 1"
                    :key="n"
                    dense
                    clickable
                    class="text-center"
                  >
                    <q-item-section>Logout</q-item-section>
                  </q-item>
                </q-list>
              </q-menu>
            </q-item>
          </q-drawer>
        </q-toolbar>
      </div>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    const rightDrawerOpen = ref(false);

    return {
      text: ref(""),
      tab: ref("mails"),
      rightDrawerOpen,
      toggleRightDrawer() {
        rightDrawerOpen.value = !rightDrawerOpen.value;
      },
    };
  },
};
</script>

<style>
a {
  text-decoration: none;
  color: black;
}
</style>
