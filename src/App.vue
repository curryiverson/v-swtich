<script lang="ts" setup>
import VSwtich from './components/VSwtich.vue';
let name: string = ''
name = 'foo'
</script>

<template>
  <div>
    <v-swtich :case="name">
      <template #foo>
        <div> foo </div>
      </template>
      <template #bar>
        <div> bar </div>
      </template>
      <template #default>
        <div> 我是默认的 </div>
      </template>
    </v-swtich>
  </div>
</template>