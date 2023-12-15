<script>
import Card from "./Card.vue";
export default {
  name: "AppProject",
  data() {
    return {
      cardItems: [
        {
          image: {
            path: "../../Boolando.png",
            alt: "Boolando-img",
          },
          video: {
            path: "../../videos/Booleando.mp4",
            alt: "Boolando-video",
          },
        },
        {
          image: { path: "../../Boolflix.png", alt: "Boolflix-img" },
          video: {
            path: "/../../videos/Boolflix.mp4",
            alt: "Boolflix-video",
          },
        },
        {
          image: { path: "../../Boolzapp.png", alt: "Boolzapp-img" },
          video: {
            path: "../../videos/Boolzapp.mp4",
            alt: "Boolzapp-video",
          },
        },
        {
          image: {
            path: "../../dc-comics.png",
            alt: "Dc-Comics-img",
          },
          video: {
            path: "../../videos/VideoComics.mp4",
            alt: "Dc-Comics-video",
          },
        },
        {
          image: { path: "../../Discord.png", alt: "Discord-img" },
          video: { path: "../../videos/Discord.mp4", alt: "Discord-video" },
        },
        {
          image: { path: "../../Spotify.png", alt: "spotify-img" },
          video: { path: "../../videos/Spotify.mp4", alt: "spotify-video" },
        },
      ],
    };
  },
  components: {
    Card,
  },
};
</script>
<template lang="">
  <div id="project" class="d-flex justify-content-center align-items-center">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <div class="text-center">
            <h2 class="section mb-3">My Skills</h2>
            <div class="w-100">
              <ul
                class="d-flex align-items-center justify-content-center w-100"
              >
                <li>
                  <img src="../assets/images/html5.png" alt="" />
                </li>
                <li>
                  <img id="css" src="../assets/images/css3.png" alt="" />
                </li>
                <li>
                  <img src="../assets/images/Bootstrap.png" alt="" />
                </li>
                <li>
                  <img src="../assets/images/JavaScript-logo.png" alt="" />
                </li>
                <li>
                  <img src="../assets/images/vue-js-icon.png" alt="" />
                </li>
                <li>
                  <img src="../assets/images/vitejs.png" alt="" />
                </li>
                <li>
                  <img src="../assets/images/sass.png" alt="" />
                </li>
                <li>
                  <img src="../assets/images/PHP.png" alt="" />
                </li>
                <li>
                  <img src="../assets/images/laravel.png" alt="" />
                </li>
                <li>
                  <img src="../assets/images/PhpMyAdmin.png" alt="" />
                </li>

                <li>
                  <img src="../assets/images/MySQL.png" alt="" />
                </li>
              </ul>
            </div>
          </div>
        </div>

        <div class="text-center mt-5">
          <div class="pt-2 fw-bold">
            Qui potrai vedere alcuni dei miei progetti!
          </div>
          <h2 class="section my-4">My Projects</h2>
        </div>

        <div class="d-flex flex-wrap justify-content-center">
          <Card v-for="(item, index) in cardItems" :key="index" :data="item" />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#project {
  background-color: whitesmoke;
  color: black;
  padding-top: 70px;
  min-height: 100vh;

  ul {
    padding: 0;
    flex-wrap: wrap;
    list-style: none;
    img {
      width: 60px;
      transition: transform 0.3s ease-in-out;
    }
    li {
      padding-inline: 10px;
    }
    #css {
      padding: 13px;
    }

    img:hover {
      -ms-transform: scale(1.5);
      -webkit-transform: scale(1.5);
      transform: scale(1.5);
    }
  }
}
@media only screen and (min-width: 992px) {
  #project {
    ul {
      img {
        width: 80px;
        flex-wrap: nowrap;
      }
    }
  }
}
</style>
