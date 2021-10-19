<template>
  <q-layout class="bg-primary" view="hHh lpR fFf">
    <q-header elevated class="bg-primary transparent text-accent">
      <q-toolbar class="">
        <q-toolbar-title class="text-left">
          <q-avatar>
            <img alt="Michael Iheajumbu" src="~assets/me.webp" />
          </q-avatar>
        </q-toolbar-title>
        <q-space />
        <!-- <div class="gt-sm text-right">
          <q-btn
            class="text-weight-light"
            no-caps
            flat
            text-color="accent"
            label="Resume"
          />
          <q-btn
            type="a"
            target="_blank"
            href="https://michaeli.netlify.app"
            class="text-weight-light"
            no-caps
            flat
            text-color="accent"
            label="Contact card"
          />
          <q-btn
            class="text-weight-light"
            no-caps
            flat
            text-color="accent"
            label="Github"
          />
        </div> -->
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>


  </q-layout>
</template>

<script>
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "MainLayout",

  components: {},

  setup() {
    const leftDrawerOpen = ref(false);

    return {
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value;
      },
    };
  },
});
</script>

<style scoped>
/* .bg {
    background: url('../assets/cool_bg.png');

} */
</style>
