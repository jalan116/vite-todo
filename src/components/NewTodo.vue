<template>
    <input
        class="text-2xl py-2 px-4 rounded-xl w-full mt-8 text-gray-800"
        type="text"
        :placeholder="placeholder"
        v-model="newTodo"
        @change="addTodo"
      />
</template>

<script setuo>
import {defineProps} from 'vue'
import {newTodo, addTodo} from '../helpers/useTodos'

define({
    placeholder: {
        type: String,
    default: 'New Todo',
    },
})
</script>