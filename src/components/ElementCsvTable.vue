<template>
  <table>
    <tr v-if="showHeader">
      <th v-for="d of headers" :key="d" v-html="d"></th>
    </tr>
    <tr v-for="r of records" :key="r[keyIndex]">
      <td v-for="d of r" :key="d" v-html="d"></td>
    </tr>
  </table>
</template>

<script>
import parse from "csv-parse/lib/sync";
import MD from "markdown-it";

export default {
  name: "ElementCsvTable",
  props: {
    filePath: {
      type: String,
      required: true
    },
    showHeader: {
      type: Boolean,
      default: false
    },
    keyIndex: {
      type: Number,
      required: true
    }
  },
  data() {
    return {
      records: [],
      headers: []
    }
  },
  mounted() {
    const md = new MD();

    fetch(this.filePath, {method: "GET"}).then(data => data.text()).then(rawText => {
      const csvData = parse(rawText, {
        skip_empty_lines: true
      });

      this.headers = csvData[0].map(d => md.render(d));
      this.records = csvData.slice(1).map(row => row.map(d => md.render(d)));
    });
  }
}
</script>

<style scoped>
table {
  text-align: left;
  table-layout: fixed;
  font-size: 0.8rem;
}

td, th{
  padding: 5px;
  word-wrap: break-word;
  overflow-wrap : break-word;
}
</style>
