<template>
  <div class="col-md-4 d-flex justify-content overflow-hidden">
    <div class="row">
      <img class="rounded" :src="img(image)" style="height: 70%; width: 100%;" />
      <div class="d-flex justify-content-center card_count">
        <h1 style="color: red">{{this.qtyVotes}}&thinsp;</h1>
        <h1>votos</h1>
      </div>
      <div class="d-flex justify-content-center">
        <h2>Digite "/{{ name }}" para votar</h2>
      </div>
    </div>
  </div>
</template>

<style>
.card_count {
  margin-top: 10px;
}
</style>

<script>
export default {
  props: {
    image: {
      type: String,
      required: true,
      // default: '../../images/bolsonaro.png'
    },
    name: {
      type: String,
      required: true,
    },
    qtyVotes: {
      type: Number,
      required: true,
    },
  },
  mounted() {
  },
};
</script>
