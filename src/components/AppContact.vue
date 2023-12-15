<script>
export default {
  name: "AppContact",
};
</script>

<template lang="">
  <div id="contact" class="d-flex justify-content-center align-items-center">
    <div class="container text-center">
      <div class="row">
        <div class="col-12">
          <div class="m-2 p-2">
            <h2 class="section">My Contacts</h2>
          </div>
        </div>
        <div
          class="col-12 col-lg-6 d-flex align-items-center justify-content-center"
        >
          <ul class="list-unstyled">
            <li>
              <div class="d-flex py-3">
                <div class="pe-3">
                  <i class="fa-solid fa-envelope fa-xl"></i>
                </div>
                <div>
                  <a
                    href="mailto:alessandroiacovella95@gmail.com ?subject=Oggetto del messaggio"
                    target="_blank"
                    rel="noopener noreferrer"
                  >
                    <font-awesome-icon
                      icon="fa-solid fa-envelope"
                      style="color: #ffffff"
                    />
                    alessandroiacovella95@gmail.com
                  </a>
                </div>
              </div>
            </li>
            <li>
              <div class="d-flex py-3 justify-content-center">
                <div class="pe-3">
                  <i class="fa-solid fa-phone fa-xl"></i>
                </div>
                <div class="phone">
                  <font-awesome-icon icon="fa-solid fa-phone" /> +39 3485229072
                </div>
              </div>
            </li>
          </ul>
        </div>
        <div
          class="col-12 col-lg-6 d-flex align-items-center justify-content-center"
        >
          <ul class="list-unstyled">
            <li>
              <div class="d-flex py-3">
                <div>
                  <a
                    href="https://www.linkedin.com/in/alessandro-iacovella-b543431a2/"
                    ><font-awesome-icon
                      icon="fa-brands fa-linkedin"
                      style="color: #ffffff"
                    />
                    Linkedin</a
                  >
                </div>
              </div>
            </li>
            <li>
              <div class="d-flex py-3">
                <div>
                  <a href="https://github.com/AlessandroIacovella95"
                    ><font-awesome-icon
                      icon="fa-brands fa-github"
                      style="color: #ffffff"
                    />
                    Github</a
                  >
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#contact {
  background-color: rgb(20, 20, 20);
  color: white;
  min-height: 60vh;

  ul {
    font-size: 1.5rem;
  }

  h2 {
    padding-bottom: 50px;
  }

  a {
    text-decoration: none;
    color: white;
    font-size: 1.25rem;
  }

  .phone {
    font-size: 1.25rem;
  }

  @media only screen and (min-width: 600px) {
    ul {
      font-size: 2rem;
    }

    h2 {
      padding-bottom: 100px;
    }
  }
}
</style>
