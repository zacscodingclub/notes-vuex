<template lang="html">
  <div id="note-editor">
    <textarea
        class="form-control"
        :value="activeNoteText"
        @input="editNote">
    </textarea>
  </div>
</template>

<script>
export default {
  computed: {
    activeNoteText() {
      return this.$store.state.activeNote.text
    }
  },
  methods: {
    editNote(e) {
      this.$store.dispatch('editNote', e.target.value)
    }
  }
}
</script>

<style lang="css">
  #note-editor {
    height: 100%;
    margin-left: 380px;
  }

  #note-editor textarea {
    height: 100%;
    border: 0;
    border-radius: 0;
  }

</style>
