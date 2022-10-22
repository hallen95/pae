<template>
  <div class="">
    <img
      class="mew__image"
      alt="Mew Image"
      :src="`https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/official-artwork/${src}.png`"
    />
  </div>
</template>

<script>
export default {
  name: "Image",
  props: {
    src: {
      type: String,
    },
  },
};
</script>

<style>
.mew__image {
  height: 180px;
  width: 180px;
  transform: rotateY(560deg);
  animation: turn 3.5s ease-out forwards 1s;
}

@keyframes turn {
  100% {
    transform: rotateY(0deg);
  }
}
</style>
