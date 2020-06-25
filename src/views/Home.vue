import JQuery from 'jquery' let $ = JQuery

<template>
  <div class="hello">
    <section class="hero is-primary is-gray is-fullheight">
      <div class="hero-head">
        <nav class="navbar">
          <div class="container">
            <div class="navbar-brand">
              <a class="navbar-item">
                <span>
                  osu!mania Thailand Tournament
                </span>
              </a>
              <span class="navbar-burger burger" data-target="navbarMenuHeroB">
                <span></span>
                <span></span>
                <span></span>
              </span>
            </div>
            <div id="navbarMenuHeroB" class="navbar-menu">
              <div class="navbar-end">
                <a class="navbar-item is-active">
                  Home
                </a>
                <a class="navbar-item">
                  Credit
                </a>
              </div>
            </div>
          </div>
        </nav>
      </div>

      <div class="hero-body">
        <div class="container has-text-centered">
          <p class="title is-abitmargin">
            Please Select Tournament
          </p>
          <div class="columns is-mobile is-centered">
            <div class="column is-5">
              <a
                class="tile is-child notification is-omthpl2020bg"
                href="http://localhost:8080"
              >
                <p class="title is-4 is-justblacktext" id="bowie">
                  OMTHPL 2020
                </p>
                <img
                  style="width:30%"
                  src="../assets/omthpl2020logo.png"
                  alt="fak i should download photoshop lol"
                />
                <p class="subtitle is-6 is-justblacktext">
                  First Tournament League System in Thailand
                </p>
              </a>
            </div>
          </div>
          <p class="subtitle">
            Yeah Select it
          </p>
        </div>
      </div>

      <div class="hero-foot"></div>
    </section>
  </div>
</template>

<script>
import $ from "jquery";

export default {
  mounted() {
    $("#bowie").remove();
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

<style lang="css">
.is-omthpl2020bg {
  background: url(../assets/bgwithout.png);
  background-position: top;
  transition: 0.2s;
}
.hero.is-primary {
  background-color: #5d5b65;
  color: white;
}
.is-gray {
  background-color: gray;
}
.is-justblacktext {
  color: rgb(0, 0, 0) !important;
}
.is-abitmargin {
  margin: 10px !important;
}
.is-omthpl2020bg:hover {
  transition: 0.2s;
  background: linear-gradient(
      rgba(255, 255, 255, 0.5),
      rgba(255, 255, 255, 0.5)
    ),
    url(../assets/bgwithout.png);
  background-position: center;
}
</style>
