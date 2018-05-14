<template>
  <v-navigation-drawer
      v-model="drawer"
      clipped
      app
      permanent
      fixed
      overflow
      floating
      width=250
      style="padding-bottom: 0px;"
    >
      <v-toolbar flat class="transparent">
        <v-list class="pa-0">
          <v-list-tile avatar>
            <v-list-tile-avatar color="amber lighten-3">
              <span class="black--text headline">A</span>
              <!-- <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTwTCBCRFWG8b2_HpaRuXyfN90yQWygv1YHi0Y9Ir37QsyXEe1BGg" > -->
            </v-list-tile-avatar>
            <v-list-tile-content>
              <v-list-tile-title>Anime Mode</v-list-tile-title>
            </v-list-tile-content>
            <v-btn flat icon>
             <v-icon>swap_horiz</v-icon>
            </v-btn>
          </v-list-tile>
        </v-list>
      </v-toolbar>
      <v-list class="pt-0" dense>
        <v-divider></v-divider>
        <v-subheader class="mt-3 grey--text text--darken-1">MAIN</v-subheader>
          <v-list-tile @click="">
            <v-list-tile-action>
              <v-icon>list</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>
              <v-list-tile-title>
                Anime List
              </v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
          <v-list-tile @click="">
            <v-list-tile-action>
              <v-icon>bookmarks</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>
              <v-list-tile-title>
                Torrents
              </v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
          <v-list-tile @click="">
            <v-list-tile-action>
              <v-icon>ondemand_video</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>
              <v-list-tile-title>
                Streaming
              </v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
        <v-subheader class="mt-3 grey--text text--darken-1">BROWSE</v-subheader>
        <v-list dense>
          <v-list-tile @click="">
            <v-list-tile-action>
              <v-icon>date_range</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>
              <v-list-tile-title>
                Calendar
              </v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
          <v-list-tile @click="">
            <v-list-tile-action>
              <v-icon>map</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>
              <v-list-tile-title>
                Season Chart
              </v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
          <v-list-tile @click="">
            <v-list-tile-action>
              <v-icon>rss_feed</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>
              <v-list-tile-title>
                RSS
              </v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
          <v-list-tile @click="">
            <v-list-tile-action>
              <v-icon>search</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>
              <v-list-tile-title>
                Search
              </v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
          <v-subheader class="mt-3 grey--text text--darken-1">SYSTEM</v-subheader>
          <v-list-tile @click="">
            <v-list-tile-action>
              <v-icon>history</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>
              <v-list-tile-title>
                History
              </v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
          <v-list-tile @click="">
            <v-list-tile-action>
              <v-icon>equalizer</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>
              <v-list-tile-title>
                Statistics
              </v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
          <v-list-tile @click="">
            <v-list-tile-action>
              <v-icon>settings</v-icon>
            </v-list-tile-action>
            <v-list-tile-content>
              <v-list-tile-title>
                Settings
              </v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
        </v-list>
      </v-list>
    </v-navigation-drawer>
</template>

<script>
export default {
  data: () => ({
    drawer: true,
  }),
  props: {
    source: String,
  },
};
</script>
