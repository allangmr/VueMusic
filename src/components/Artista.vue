<template>
  <li :class="artist">
    <h2>
      <a :href="artist.url" target="_blank">{{artist.name}}</a>
    </h2>
    <img :src="artist.image[2]['#text']" />
  </li>
</template>

<script>
export default {
  name: "artista",
  props: ["artist"]
};
</script>


<style lang="stylus" scope>
li.artist {
  display: block;
  margin: 0 10px;
}
</style>

