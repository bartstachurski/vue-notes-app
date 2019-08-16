<template>
  <div class="note-selector active">
    <p class="note-selector-title">Note title...</p>
    <p class="note-selector-timestamp">Timestamp here...</p>
  </div>
</template>

<script>
export default {
  name: 'note-selector'
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