<template>
  <div>
    <v-toolbar class="white navbar">
      <v-toolbar-title class="hidden-sm-and-down black--text">
        Guilbo
      </v-toolbar-title>

      <v-btn-dropdown
        :label="$t('project-list')"
        :options="projectList"
        >
      </v-btn-dropdown>

      <v-space></v-space>

      <v-toolbar-items>
      </v-toolbar-items>
    </v-toolbar>
    <nuxt/>
  </div>
</template>

<i18n>
{
  "en": {
    "project-list": "PROJECTS"
  },
  "ja": {
    "project-list": "プロジェクト"
  }
}
</i18n>

<script>
import { mapActions, mapGetters, mapState } from 'vuex'

export default {
  data: function () {
    return {
      projectList: [
        { text: 'A' },
        { text: 'B' },
        { text: 'C' }
      ]
    }
  },

  computed: {
    ...mapGetters([
    ]),

    ...mapState([
    ])
  },

  method: {
    ...mapActions([
    ])
  }
}
</script>

<style lang="stylus">
html, body
  font-family: 'Roboto', 'Noto Sans Japanese', sans-serif;
  margin: 0
  padding: 0
</style>
