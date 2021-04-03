<template>
  <BaseSection title="Works">
    <h3>Exhibition / Events</h3>
    <ElementCsvTable file-path="/csv/exhibition-events.csv" :key-index="1" :show-header="true"/>

    <h3>Publication</h3>
    <ElementPublicationList/>

    <h3>VJ</h3>
    <ElementCsvTable file-path="/csv/vj.csv" :key-index="1" :show-header="true"/>

  </BaseSection>
</template>

<script>
import BaseSection from "@/components/BaseSection";
import ElementCsvTable from "@/components/ElementCsvTable";
import ElementPublicationList from "@/components/ElementPublicationList";

export default {
  name: "Works",
  components: {BaseSection, ElementCsvTable, ElementPublicationList}
}
</script>

<style scoped>
h3 {
  margin-top: 20px;
}
</style>
