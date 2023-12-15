<script>
export default {
  name: "HomePage",
};
</script>

<template>
  <div id="home" class="mp-4">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <div class="m-5 py-5">
            <h1 class="main-heading">
              Hi I'm <br />
              Alessandro Iacovella
            </h1>
            <h3 class="sub-heading">Jr. Full Stack Web Developer</h3>
            <div class="py-5">
              <a href="#about" class="btn btn-outline-success btn-lg"
                >About me</a
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#home {
  min-height: 100vh;
  background-color: whitesmoke;

  .main-heading {
    font-weight: 700;
    font-size: 4vw; // Utilizzo di vw per il dimensionamento del testo
  }

  .sub-heading {
    font-weight: 700;
    font-size: 2.5rem;
  }

  @media only screen and (min-width: 576px) {
    .main-heading {
      font-size: 3rem;
    }
  }

  @media only screen and (min-width: 768px) {
    .main-heading {
      font-size: 4rem;
    }
  }

  @media only screen and (min-width: 992px) {
    .main-heading {
      font-size: 5rem;
    }
  }

  @media only screen and (min-width: 1200px) {
    .main-heading {
      font-size: 6rem;
    }
  }
}
</style>
