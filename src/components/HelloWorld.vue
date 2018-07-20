<template>
<div class="wrapper">


<div class='container'>
  
<div class='control' @click="expandSearch">
    <div class='btn-material'>

     <font-awesome-icon icon="search" class="icon-material-search" />

    <font-awesome-icon icon="search" class="icon-material-search" />

    </div>
  </div>
</div>
<font-awesome-icon icon="times-circle" class="icon-close" @click="collapseSearch" />


<font-awesome-icon icon="times-circle" class="icon-close" @click="collapseSearch"/>

<div class='search-input'>
  <input class='input-search' placeholder='Start Typing' type='text'>
</div>
<p>

Jupiter is the fifth planet from the Sun and the largest in the Solar System. It is a giant planet with a mass one-thousandth that of the Sun, but two-and-a-half times that of all the other planets in the Solar System combined. Jupiter and Saturn are gas giants; the other two giant planets, Uranus and Neptune, are ice giants. Jupiter has been known to astronomers since antiquity.[14] The Romans named it after their god Jupiter.[15] When viewed from Earth, Jupiter can reach an apparent magnitude of −2.94, bright enough for its reflected light to cast shadows,[16] and making it on average the third-brightest natural object in the night sky after the Moon and Venus.

Jupiter is primarily composed of hydrogen with a quarter of its mass being helium, though helium comprises only about a tenth of the number of molecules. It may also have a rocky core of heavier elements,[17] but like the other giant planets, Jupiter lacks a well-defined solid surface. Because of its rapid rotation, the planet's shape is that of an oblate spheroid (it has a slight but noticeable bulge around the equator). The outer atmosphere is visibly segregated into several bands at different latitudes, resulting in turbulence and storms along their interacting boundaries. A prominent result is the Great Red Spot, a giant storm that is known to have existed since at least the 17th century when it was first seen by telescope. Surrounding Jupiter is a faint planetary ring system and a powerful magnetosphere. Jupiter has at least 79 moons,[18] including the four large Galilean moons discovered by Galileo Galilei in 1610. Ganymede, the largest of these, has a diameter greater than that of the planet Mercury.

Jupiter has been explored on several occasions by robotic spacecraft, most notably during the early Pioneer and Voyager flyby missions and later by the Galileo orbiter. In late February 2007, Jupiter was visited by the New Horizons probe, which used Jupiter's gravity to increase its speed and bend its trajectory en route to Pluto. The latest probe to visit the planet is Juno, which entered into orbit around Jupiter on July 4, 2016.[19][20] Future targets for exploration in the Jupiter system include the probable ice-covered liquid ocean of its moon Europa.
</p>
=======
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
