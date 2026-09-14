<script setup>
const props = defineProps({
  title: {
    type: String,
    default: 'Section'
  }
})
</script>

<template>
  <section>
            <h3>{{title}}</h3>
            <slot></slot>
        </section>
</template>

<style scooped>
section {
    margin-top: 16px;
}

Section h3{
    margin: 0 0 6px;
    font-size: 14px;
    color: #ca0a0a;
}
</style>