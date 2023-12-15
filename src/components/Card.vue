<script>
export default {
  props: {
    data: {
      type: Object,
      required: true,
    },
  },
  data() {
    return {
      cardType: "image",
      content: this.data,
    };
  },
  methods: {
    toggleContent() {
      if (this.cardType === "image") {
        this.changeToVideo();
      } else {
        this.changeToImage();
      }
    },
    changeToVideo() {
      this.cardType = "video";
    },
    changeToImage() {
      this.cardType = "image";
    },
  },
};
</script>

<template>
  <div class="col-lg-5 col-md-10 mb-3 me-3">
    <div class="card" @click="toggleContent">
      <img
        v-if="cardType === 'image'"
        :src="content.image.path"
        :alt="content.image.alt"
        class="card-img-top"
      />
      <video
        v-else-if="cardType === 'video'"
        :src="content.video.path"
        controls
        class="card-img-top"
      ></video>

      <div class="card-body d-flex align-items-center justify-content-between">
        <div class="icons">
          <font-awesome-icon
            class="icon_custom me-2"
            icon="fa-solid fa-image"
            @click.stop="changeToImage"
          />
          <font-awesome-icon
            class="icon_custom"
            icon="fa-solid fa-video"
            @click.stop="changeToVideo"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  max-width: 100%;
}

.card-img-top {
  width: 100%;
  height: auto;
}

.icon_custom {
  cursor: pointer;
  color: rgb(30, 28, 28);
  transition: color 0.3s ease-in-out;

  &:hover {
    color: red;
  }
}
</style>
