<template>
  <q-page>
    <!-- Main Page Nav -->

    <div class="flex justify-center items-center gt-sm">
      <q-bar class="bg-white" style="width: 80%; height: 50px">
        <div class="text-weight-regular q-pl-sm">
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

        <q-space />

        <div class="text-amber-7 text-h5 q-pr-lg">Try Premium For Free</div>
      </q-bar>
    </div>

    <!-- Gradient And Main Content -->

    <div class="gradient full-width"></div>

    <!-- Main Content -->

    <main class="flex justify-center items-center">
      <div style="width: 80%">
        <section>
          <div>
            <!-- Profile Picture And Connections -->

            <div class="row justify-center items-center">
              <div class="relative-position top--70 col-1">
                <q-img
                  class="shadow-3 q-mr-sm absolute"
                  src="../assets/images/LinkedIn-Logo.png"
                  width="95px"
                  height="95px"
                  style="border-radius: 50%"
                  alt="Person"
                />
              </div>
              <div class="col-5">
                <span class="text-primary">+500</span><span> Connections</span>
              </div>

              <q-space />

              <div class="q-mt-md">
                <q-btn-dropdown
                  dropdown-icon="more_horiz"
                  class="q-px-sm q-mx-sm col-6"
                  no-icon-animation
                >
                  <q-list>
                    <q-item clickable v-close-popup @click="onItemClick">
                      <q-item-section>
                        <q-item-label>Photos</q-item-label>
                      </q-item-section>
                    </q-item>
                  </q-list>
                </q-btn-dropdown>
                <q-btn
                  class="q-px-sm q-mx-sm"
                  icon="mark_email_read"
                  label="Message"
                />
                <q-btn
                  class="bg-primary q-px-sm text-white q-mx-sm"
                  icon="add"
                  label="Connect"
                />
              </div>
            </div>

            <!-- Profile -->

            <div class="q-pt-md row">
              <div class="col-8">
                <div class="text-h5 text-weight-bold">Moeen Sedaqati</div>
                <div>
                  Quasar, Vue, Laravel, Html, Css, Wordpress, Figma - Workin At
                  <a
                    href="https://aytronic.com/"
                    class="text-primary text-weight-bold"
                    >Aytronic</a
                  >
                </div>
                <div class="text-grey-6">Iran Golestan, Gonbad-E Qabus</div>
                <div>
                  <q-img
                    src="../assets/images/LinkedIn-Logo.png"
                    class=""
                    width="30px"
                    height="30px"
                    style="border-radius: 50%"
                  />
                  <span
                    >1 Mutual Connection:
                    <span class="text-grey-6">Orlando Diggs</span></span
                  >
                </div>
              </div>

              <div class="col-4 q-mt-md">
                <div class="float-right">
                  <div>
                    <q-img
                      src="../assets/images/LinkedIn-Logo.png"
                      class="q-px-md"
                      width="30px"
                      height="30px"
                      style="border-radius: 50%"
                    />
                    <span>Notion</span>
                  </div>

                  <div>
                    <q-img
                      src="../assets/images/LinkedIn-Logo.png"
                      class="q-px-md"
                      width="30px"
                      height="30px"
                      style="border-radius: 50%"
                    />
                    <span>Harvard University</span>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>

        <q-separator class="q-my-lg" />

        <!-- About -->

        <div class="row">
          <div class="col-6">
            <q-toolbar>
              <q-toolbar-title class="text-weight-bold">
                About
              </q-toolbar-title>
              <a
                href="https://moeensedaqati.ir"
                class="text-primary text-weight-medium q-mr-lg q-pr-sm"
                >moeensedaqati.ir <q-icon name="arrow_outward"
              /></a>
            </q-toolbar>
            <div>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit.
              Consequatur rerum unde incidunt id, autem pariatur, voluptate aut
              porro itaque ducimus commodi, illo amet quas voluptatibus ea. Eum
              quod nemo tempora?
            </div>

            <q-separator class="q-my-lg" />

            <div class="text-weight-bold text-h6">Experience</div>

            <q-card class="my-card" flat>
              <q-card-section horizontal>
                <q-card-section>
                  <q-avatar>
                    <img src="../assets/images/Aytronic-logo.png" />
                  </q-avatar>
                </q-card-section>
                <q-card-section class="q-pt-xs">
                  <div class="text-h5 q-mt-sm q-mb-xs">
                    <a href="http://aytronic.com">Aytronic</a>
                  </div>
                  <div class="text-grey">Part-Time</div>
                  <div class="text-grey">3 Month</div>
                  <div class="text-caption text-grey q-mt-sm">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmod tempor incididunt ut labore et dolore magna
                    aliqua.
                  </div>
                </q-card-section>
              </q-card-section>
            </q-card>
            <q-separator class="q-my-md" />
          </div>

          <q-separator vertical class="q-mx-lg" />

          <!-- People Viewed This Website -->

          <div class="col-5">
            <div class="text-weight-bolder q-ml-md">People Also Viewed</div>
            <q-item class="q-my-xs">
              <q-item-section avatar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/boy-avatar.png" />
                </q-avatar>
              </q-item-section>

              <q-item-section>
                <q-item-label>Title</q-item-label>
                <q-item-label caption> Subhead </q-item-label>
              </q-item-section>
            </q-item>
            <q-item class="q-my-xs">
              <q-item-section avatar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/boy-avatar.png" />
                </q-avatar>
              </q-item-section>

              <q-item-section>
                <q-item-label>Title</q-item-label>
                <q-item-label caption> Subhead </q-item-label>
              </q-item-section>
            </q-item>
            <q-item class="q-my-xs">
              <q-item-section avatar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/boy-avatar.png" />
                </q-avatar>
              </q-item-section>

              <q-item-section>
                <q-item-label>Title</q-item-label>
                <q-item-label caption> Subhead </q-item-label>
              </q-item-section>
            </q-item>
            <q-item class="q-my-xs">
              <q-item-section avatar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/boy-avatar.png" />
                </q-avatar>
              </q-item-section>

              <q-item-section>
                <q-item-label>Title</q-item-label>
                <q-item-label caption> Subhead </q-item-label>
              </q-item-section>
            </q-item>
            <q-item class="q-my-xs">
              <q-item-section avatar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/boy-avatar.png" />
                </q-avatar>
              </q-item-section>

              <q-item-section>
                <q-item-label>Title</q-item-label>
                <q-item-label caption> Subhead </q-item-label>
              </q-item-section>
            </q-item>

            <q-btn
              class="full-width text-black"
              icon-right="expand_more"
              label="Show More"
            />

            <q-separator class="q-my-lg" />

            <div class="q-mt-md">
              <div class="text-weight-bolder q-ml-md">People You May Know</div>
              <q-item class="q-my-xs">
                <q-item-section avatar>
                  <q-avatar>
                    <img src="https://cdn.quasar.dev/img/boy-avatar.png" />
                  </q-avatar>
                </q-item-section>

                <q-item-section>
                  <q-item-label>Title</q-item-label>
                  <q-item-label caption> Subhead </q-item-label>
                </q-item-section>
              </q-item>
            </div>
          </div>
        </div>
      </div>
    </main>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
export default defineComponent({
  name: "IndexPage",
});
</script>

<style>
.gradient {
  background: rgb(255, 248, 230);
  background: linear-gradient(
    142deg,
    rgba(255, 248, 230, 1) 0%,
    rgba(150, 205, 217, 1) 100%
  );
  height: 250px;
}

.q-bar--standard {
  padding: 0;
}

.top--70 {
  top: -70px;
}

.q-toolbar {
  padding: 0;
}

.q-toolbar__title {
  padding: 0;
}

.my-card {
  width: 60%;
}
</style>
