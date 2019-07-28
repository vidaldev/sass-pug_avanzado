<template lang="pug">
  #app
    .columns
        .column
            .is-full.header_bar
              header_bar
            .columns.content_body
                .column.sidebar_size
                    sidebar
                .column
                    movie_cards
</template>

<script>
import header_bar from'./components/header/Header.vue'
import sidebar from'./components/sidebar/Sidebar.vue'
import movie_cards from'./components/movie_cards/Movie_cards.vue'
export default {
  name: 'app',
  components: {
    header_bar,
    sidebar,
    movie_cards
  }
}
</script>

<style lang="scss">
@import '../node_modules/bulma/bulma.sass';
@import url('https://fonts.googleapis.com/css?family=Lato:700&display=swap');
body {
  margin:0;
  padding: 0;
}
.header_bar {
  position: fixed;
  z-index: 3;
  width: 100%;
  height: 72px;
}
.sidebar_size {
  flex:none;
  width: 89px;
}
.content_body{
  margin-top:49px;
}
</style>
