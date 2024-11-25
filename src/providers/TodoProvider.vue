<script setup>
import { provide } from 'vue'
import { useTodoTemplate } from '../composables/useTodoTemplate'

const { showTodoList, searchKeyword, addInputValue, handleAddTodo, handleDeleteTodo } = useTodoTemplate()

provide('showTodoList', showTodoList)
provide('searchKeyword', searchKeyword)
provide('addInputValue', addInputValue)
provide('handleAddTodo', handleAddTodo)
provide('handleDeleteTodo', handleDeleteTodo)
</script>

<template>
  <slot />
</template>
