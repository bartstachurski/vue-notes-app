<template>
  <div class="note-selectors">
    <NoteSelector />
    <NoteSelector />
    <NoteSelector />
  </div>
</template>

<script>
import NoteSelector from './NoteSelector.vue';

export default {
  name: 'note-selectors',
  components: {
    NoteSelector    
  }
};
</script>

<style>
/*Layout*/
.note-selectors {
 flex: 0 0 13em;
}

/*Colors*/
.note-selectors {
 border-right: 1px solid #DCDADC;
}
</style>