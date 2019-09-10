<template>
  <div>
    <p>Editor page</p>
    <Editor />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import { Component } from 'vue-property-decorator'
import Editor from '@/components/Editor.vue'
@Component({ components: { Editor } })
export default class EditorPage extends Vue {
  // Data property
  myDataProperty: string

  // Lifecycle hook
  mounted() {
    this.myDataProperty = 'Boop'
  }
}
</script>