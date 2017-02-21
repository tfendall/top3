<template>
  <div class="hello">
    <h1>What are your top 3 types of Colgate brand toothpaste?</h1>
    <ul class="list">
      <li v-for="item in items">
        <mdl-textfield :floating-label="item.label" v-model="item.value"></mdl-textfield>
      </li>
    </ul>
    <mdl-button>Submit</mdl-button>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data() {
    return {
      items: [
        { label: 'One' },
        { label: 'Two' },
        { label: 'Three' },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
  max-width: 800px;
  margin: 0  auto;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
