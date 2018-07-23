
<template>
  <div class="wrapper">


    <div class="container">
      <div class="row">
        <div class="col-12">
          <div class='control' @click="expandSearch">
            <div class='btn-material'>
              <font-awesome-icon icon="search" class="icon-material-search" />
            </div>
          </div>
          <font-awesome-icon icon="times-circle" class="icon-close" @click="collapseSearch" />

          <div class='search-input'>
            <input class='input-search' placeholder='Start Typing' type='text'>
          </div>
        </div>
        <div class="col-12">

          <p>
            Jupiter is the fifth planet from the Sun and the largest in the Solar System.
          </p>
        </div>
        <div class="col-6">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Corporis, id.
        </div>
        <div class="col-6">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Corporis, id.
        </div>
      </div>
    </div>


  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      body: document.body,
      msg: 'Welcome to Your Vue.js App',
    };
  },
  methods: {
    expandSearch() {
      this.body.classList.add('search-active');
      const input = document.querySelector('.input-search');
      input.focus();
    },
    collapseSearch() {
      this.body.classList.remove('search-active');
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
@import '../components/hello.scss';

h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
  li {
    display: inline-block;
    margin: 0 10px;
  }
}
a {
  color: #42b983;
}
</style>
