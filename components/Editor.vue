<template>
  <div>
    <p>Editor</p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import { Component } from 'vue-property-decorator'

@Component
export default class Editor extends Vue {
  // Data property
  myDataProperty: string

  // Lifecycle hook
  mounted() {
    this.myDataProperty = 'Boop'
  }

  // Component method
  updateMyProperty($event) {
    this.myDataProperty = $event.target.value
  }
}
</script>