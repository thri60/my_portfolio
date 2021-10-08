<template>
  <q-layout class="bg-primary" view="hHh lpR fFf">

       <q-header elevated class="bg-primary transparent text-accent">
      <q-toolbar class=" ">
        <q-btn flat round dense icon="menu" class="q-mr-sm lt-sm" />

        <q-toolbar-title class="text-left">
          <q-avatar>
            <img src="~assets/me.jpg" />
          </q-avatar>
        </q-toolbar-title>
        <q-space />
                <div class="gt-sm text-right">
          <q-btn class="text-weight-light" no-caps flat text-color="accent" label="Home" />
          <q-btn class="text-weight-light" no-caps flat text-color="accent" label="About" />
          <q-btn class="text-weight-light" no-caps flat text-color="accent" label="Services" />
          <q-btn class="text-weight-light" no-caps flat text-color="accent" label="Works" />
          <q-btn class="text-weight-light" no-caps flat text-color="accent" label="Contact" />
        </div>
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
