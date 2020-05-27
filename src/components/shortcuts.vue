<template>
  <q-list
    no-border
    link
    inset-delimiter
  >
    <q-list-header>Raccourcis</q-list-header>
    <q-item @click.native="onHome">
      <q-item-side icon="home" />
      <q-item-main label="Acceuil" />
    </q-item>
    <q-item @click.native="onDesktop">
      <q-item-side icon="desktop_windows" />
      <q-item-main label="Bureau" />
    </q-item>
    <q-item @click.native="onDocuments">
      <q-item-side icon="folder" />
      <q-item-main label="Documents" />
    </q-item>
    <q-item @click.native="onDownloads">
      <q-item-side icon="vertical_align_bottom" />
      <q-item-main label="Téléchargement" />
    </q-item>
    <q-item @click.native="onPictures">
      <q-item-side icon="image" />
      <q-item-main label="Images" />
    </q-item>
    <q-item @click.native="onMusic">
      <q-item-side icon="music_note" />
      <q-item-main label="Musique" />
    </q-item>
    <q-item @click.native="onMovies">
      <q-item-side icon="local_movies" />
      <q-item-main label="Films" />
    </q-item>
  </q-list>
</template>

<script>
export default {
  name: 'Shortcuts',

  data () {
    return {}
  },

  methods: {
    onHome: function () {
      this.$emit('selected', 'home')
    },
    onDesktop: function () {
      this.$emit('selected', 'desktop')
    },
    onDocuments: function () {
      this.$emit('selected', 'documents')
    },
    onDownloads: function () {
      this.$emit('selected', 'downloads')
    },
    onPictures: function () {
      this.$emit('selected', 'pictures')
    },
    onMusic: function () {
      this.$emit('selected', 'music')
    },
    onMovies: function () {
      this.$emit('selected', 'videos')
    }
  }
}
</script>

<style>
</style>
