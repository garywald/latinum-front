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
        { number: '2', message: 'Nyaraa-2' },
        { number: '3', message: 'Usponso' },
        { number: '4', message: 'Alexandre' },
        { number: '5', message: 'adrienbgcz' },
        { number: '6', message: 'MaximeWallart' },
        { number: '7', message: 'Lucas-BAJEUX' },
        { number: '8', message: 'Isaac Leclercq' },
        { number: '9', message: 'Killian-Zouareg' },
        { number: '10', message: 'Tristan-Dussart-fr' },
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
