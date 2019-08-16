<template>
  <div class="note-selector" v-bind:class="{active: false}" v-on:click="makeActive">
    <p class="note-selector-title">{{ note.body }}</p>
    <p class="note-selector-timestamp">{{ note.timestamp }}</p>
  </div>
</template>

<script>
export default {
  name: 'note-selector',
  props: ['note'],
  methods: {
    makeActive: function() {
      console.log("hellooooo from the makeActive function");
    }
  }
};
</script>

<style>
/*Layout*/
.note-selector {
 padding: 1em;
}
.note-selector p {
 margin: 0;
}

/*Colors*/
.note-selector {
 border-bottom: 1px solid #DCDADC;
}
.note-selector.active {
 background-color: #FCE18D;
}
.note-selector-title {
 background-color: inherit;
}
.note-selector-timestamp {
 color: #626262;
 background-color: inherit;
}

/*Typography*/
.note-selector-title {
 font-weight: bold;
}
.note-selector-timestamp {
 font-size: 0.7em;
}
</style>