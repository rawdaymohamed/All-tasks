<template>
  <div class="card mt-2" v-if="tasks.length > 0">
    <ul class="list-group list-group-flush" v-for="task in tasks" :key="task.id">
      <Task :task="task" />
    </ul>
  </div>
</template>
<script setup>
import Task from './Task.vue'

defineProps({
  tasks: Array
})
</script>
