<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="bg-red-10 text-black" align="center">
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="leftDrawerOpen = !leftDrawerOpen"
        />

        <q-toolbar-title>All Red Dead</q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-drawer
      v-model="leftDrawerOpen"
      show-if-above
      bordered
      content-class="bg-accent"
    >
      <q-list>
        <q-item clickable v-ripple>
          <q-item-section avatar>
            <q-avatar class="shadow-18">
              <img
                src="https://static1.thegamerimages.com/wordpress/wp-content/uploads/2019/12/Red-Dead-Meme-Feature.jpg"
              />
            </q-avatar>
          </q-item-section>

          <q-item-section>Welcome Stranger</q-item-section>
        </q-item>

        <q-item-label header class="text-black"> Useless Links </q-item-label>
        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import EssentialLink from "components/EssentialLink.vue";

const linksData = [
  {
    title: "Rockstar Page",
    caption: "rockstar.page",
    icon: "home",
    link: "https://www.rockstargames.com/reddeadredemption2/restricted-content/agegate/form?redirect=https%3A%2F%2Fwww.rockstargames.com%2Freddeadredemption2%2F&options=&locale=en_us",
  },
  {
    title: "Github",
    caption: "github.com/topics/rockstargames",
    icon: "fa-brands fa-github",
    link: "https://github.com/topics/rockstargames",
  },
  {
    title: "SupportChannel",
    caption: "support.rockstar",
    icon: "warning",
    link: "https://support.rockstargames.com/br/categories/200013106",
  },
  {
    title: "Ballas Forum",
    caption: "forum.rockstar",
    icon: "record_voice_over",
    link: "https://socialclub.rockstargames.com/crew/forum_drive_ballas/wall",
  },
  {
    title: "Twitter",
    caption: "@rockstargames",
    icon: "fa-brands fa-twitter",
    link: "https://twitter.com/rockstargames",
  },
  {
    title: "Facebook",
    caption: "@RockstarGamesBra",
    icon: "facebook",
    link: "https://pt-br.facebook.com/RockstarBra/",
  },
  {
    title: "Social Club",
    caption: "Community",
    icon: "favorite",
    link: "https://socialclub.rockstargames.com/",
  },
];

export default {
  name: "MainLayout",
  components: {
    EssentialLink,
  },
  data() {
    return {
      leftDrawerOpen: false,
      essentialLinks: linksData,
    };
  },
};
</script>
