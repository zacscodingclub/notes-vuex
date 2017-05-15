<template lang="html">
  <div class="app">
    <toolbar></toolbar>
    <notes-list></notes-list>
    <editor></editor>
  </div>
</template>

<script>
import Toolbar from './Toolbar.vue'
import NotesList from './NotesList.vue'
import Editor from './Editor.vue'

export default {
  components: {
    Toolbar,
    NotesList,
    Editor
  }
}
</script>

<style lang="css">
</style>
