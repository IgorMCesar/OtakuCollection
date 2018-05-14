<template>
  <v-app
    id="inspire"
    dark
  >
    <SideNavAnime></SideNavAnime>
    <TitleBar></TitleBar>
    <v-content>
      <v-container fill-height fill-width>
        <v-layout justify-center align-center>
          <v-flex shrink>
            <v-tooltip right>
              <v-btn
                slot="activator"
                :href="source"
                icon
                large
                target="_blank"
              >
                <v-icon large>code</v-icon>
              </v-btn>
              <span>Source</span>
            </v-tooltip>
            <v-tooltip right>
              <v-btn slot="activator" icon large href="https://codepen.io/johnjleider/pen/YeRKwQ" target="_blank">
                <v-icon large>mdi-codepen</v-icon>
              </v-btn>
              <span>Codepen</span>
            </v-tooltip>
          </v-flex>
        </v-layout>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
  import TitleBar from '@/components/TitleBar/TitleBar1';
  import SideNavAnime from '@/components/SideNavMenu/SideNavAnime';
  import Buttons from '@/components/TitleBar/Buttons';
  import User from '@/components/TitleBar/User';

  export default {
    components: { User, SideNavAnime, Buttons, TitleBar },
    data: () => ({
      drawer: true,
      items: [
        { icon: 'trending_up', text: 'Most Popular' },
        { icon: 'subscriptions', text: 'Subscriptions' },
        { icon: 'history', text: 'History' },
        { icon: 'featured_play_list', text: 'Playlists' },
        { icon: 'watch_later', text: 'Watch Later' },
      ],
      items2: [
        { picture: 28, text: 'Joseph' },
        { picture: 38, text: 'Apple' },
        { picture: 48, text: 'Xbox Ahoy' },
        { picture: 58, text: 'Nokia' },
        { picture: 78, text: 'MKBHD' },
      ],
    }),
    props: {
      source: String,
    },
  };
</script>

<style lang="scss">
  .clip-right{
    margin-right: 0px !important;
  }
</style>
