<template>
  <div>
    <ElementSectionTitle>{{ title }}</ElementSectionTitle>
    <div>
      <slot></slot>
    </div>
  </div>
</template>

<script>
import ElementSectionTitle from "@/components/ElementSectionTitle";

export default {
  name: "BaseSection",
  props: {
    title: {
      type: String,
      required: true
    }
  },
  components: {ElementSectionTitle},
}
</script>

<style scoped>

</style>
