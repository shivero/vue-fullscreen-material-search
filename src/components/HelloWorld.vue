
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
          <ul>
<li><strong>Jupiter is the fourth brightest object in the solar system.</strong><br>
Only the Sun, <a href="https://space-facts.com/the-moon/">Moon</a> and <a href="https://space-facts.com/venus/">Venus</a> are brighter. It is one of five planets visible to the naked eye from Earth.</li>
<li><strong>The ancient Babylonians were the first to record their sightings of Jupiter.</strong><br>
This was around the 7<sup>th</sup>&nbsp;or 8<sup>th</sup>&nbsp;century BC. Jupiter is named after the king of the Roman gods. To the Greeks, it represented Zeus, the god of thunder. The Mesopotamians saw Jupiter as the god Marduk and patron of the city of Babylon. Germanic tribes saw this planet as Donar, or Thor.</li>
<li><strong>Jupiter has the shortest day of all the planets.</strong><br>
It turns on its axis once every 9 hours and 55 minutes. The rapid rotation flattens the planet slightly, giving it an oblate shape.</li>
<li><strong>Jupiter orbits the Sun once every 11.8 Earth years.</strong><br>
From our point of view on <a href="https://space-facts.com/earth/">Earth</a>, it appears to move slowly in the sky, taking months to move from one constellation to another.</li>
<li><strong>Jupiter has unique cloud features.</strong><br>
The upper atmosphere of Jupiter is divided into cloud belts and zones. They are made primarily of ammonia crystals, sulfur, and mixtures of the two compounds.</li>
<li><strong>The Great Red Spot is a huge storm on Jupiter.</strong><br>
It has raged for at least 350 years. It is so large that three Earths could fit inside it.</li>
<li><strong>Jupiter’s interior is made of rock, metal, and hydrogen compounds.</strong><br>
Below Jupiter’s massive atmosphere (which is made primarily of hydrogen), there are layers of compressed hydrogen gas, liquid metallic hydrogen, and a core of ice, rock, and metals.</li>
<li><strong>Jupiter’s moon Ganymede is the largest moon in the solar system.</strong><br>
Jupiter’s moons are sometimes called the Jovian satellites, the largest of these are Ganymeade, Callisto Io and Europa. Ganymeade measures 5,268 km across, making it larger than the planet <a href="https://space-facts.com/mercury/">Mercury</a>.</li>
<li><strong>Jupiter has a thin ring system.</strong><br>
Its rings are composed mainly of dust particles ejected from some of Jupiter’s smaller worlds during impacts from incoming comets and asteroids. The <a href="https://space-facts.com/gas-giants/#rings">ring system</a> begins some 92,000 kilometres above Jupiter’s cloud tops and stretches out to more than 225,000 km from the planet. They are between 2,000 to 12,500 kilometres thick.</li>
<li><strong>Eight spacecraft have visited Jupiter.</strong><br>
Pioneer 10 and 11, Voyager 1 and 2, Galileo, Cassini, Ulysses, and New Horizons missions. The Juno mission is its way to Jupiter and will arrive in July 2016. Other future missions may focus on the Jovian moons Europa, Ganymede, and Callisto, and their subsurface oceans.</li>
</ul>
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
