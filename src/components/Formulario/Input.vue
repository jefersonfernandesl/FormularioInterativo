<script>
export default {
  props: {
    type: {
      type: String,
      default: 'text'
    },
    name: {
      type: String,
      required: true
    },
    id: {
      type: String,
      required: true
    },
    placeholder: {
      type: String,
      default: ''
    },
    labelText: {
      type: String,
      default: 'Label Text'
    },
    inputId: {
      type: String,
      required: true
    },
    modelValue: {
      type: String,
      required: false
    }
  },
  emits: ['update:modelValue']
}
</script>

<template>
  <section class="w-1/3 flex flex-col">
    <label class="w-full text-black border-solid border-b-2 border-gray-200 p-1 mb-2":for="inputId">{{ labelText }}</label>
    <input class="w-full bg-gray-200 text-black rounded p-1 focus:outline-gray-400" :type="type" :name="name" :id="id"
      :placeholder="placeholder" />
  </section>
</template>