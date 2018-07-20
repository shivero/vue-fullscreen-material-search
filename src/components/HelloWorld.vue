<template>
<div class="wrapper">


<div class='container'>
  
<div class='control' @click="expandSearch">
    <div class='btn-material'>
    <font-awesome-icon icon="search" class="icon-material-search" />
    </div>
  </div>
</div>
<font-awesome-icon icon="times-circle" class="icon-close" @click="collapseSearch" />

<div class='search-input'>
  <input class='input-search' placeholder='Start Typing' type='text'>
</div>
<p>Lorem ipsum dolor sdit amet consectetur adipisicing elit. Culpa ratione maxime, suscipit, ab, non at architecto in est aut quo totam praesentium id ipsam porro esse iure. Enim neque, repellat magnam magni vitae recusandae, dicta quibusdam adipisci unde ratione cumque! Fuga impedit laudantium, ex eaque repellat delectus unde cupiditate, aspernatur mollitia nisi nemo veniam a, sequi aliquid cum eveniet repellendus beatae soluta sunt officia in exercitationem possimus! Animi eum expedita totam blanditiis. Consequuntur velit expedita amet, ipsa laborum aspernatur totam cumque sunt incidunt assumenda et minima, a veritatis repellat dolorum nostrum aperiam officia dolorem! Excepturi ducimus reiciendis voluptas. Quod necessitatibus omnis natus dignissimos tempora maxime perferendis ex ut in molestias similique consequuntur eius, repudiandae soluta ipsum est, praesentium deserunt animi quisquam? Eligendi ex odit perspiciatis magni, alias accusantium voluptates excepturi. Ut qui exercitationem et ad rem itaque cum vitae nostrum recusandae, porro sint, hic quae officia amet minima modi earum. Atque quae fuga esse veniam nisi magni minus quibusdam accusantium labore nemo modi quod dolorem eaque voluptatum sequi deleniti quas recusandae consequatur, impedit quo autem mollitia. Autem earum nesciunt asperiores, eius quia magni enim id quos explicabo quas laborum aperiam pariatur a tenetur, vero error in? Et possimus ipsa id.</p>
</div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      body: document.body,
      msg: "Welcome to Your Vue.js App"
    };
  },
  methods: {
    expandSearch() {
      this.body.classList.add("search-active");
      const input = document.querySelector(".input-search");
      input.focus();
    },
    collapseSearch() {
      this.body.classList.remove("search-active");
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
@import "../components/hello.scss";

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
