<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <ul>
      <li id="todo-list-item" class="list-group-item" v-for="item in items" v-bind:key="item.number">{{ item.number + '-' + item.message }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Latinum',
  props: {
    msg: String,
  },
  data() {
    return {
      items: [
        {number: '👑', message: 'Garywald'},
        { number: '2', message: '' },
        { number: '3', message: '' },
        { number: '4', message: '' },
        { number: '5', message: 'adrienbgcz' },
        { number: '6', message: '' },
        { number: '7', message: '' },
        { number: '8', message: '' },
        { number: '9', message: '' },
        { number: '10', message: '' },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-position: inside;
}
#todo-list-item{
  line-height: 1.4;
  color: rgb(61, 61, 61);
  font-size: 24px;
  font-family: 'Caveat', cursive;
}

a {
  color: #42b983;
}
</style>
