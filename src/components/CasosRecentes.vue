<template>
  <div class="rec-container">
    <div>
      <p class="txt-rec text-center flex flex-center">Casos Recentes</p>
    </div>
    <q-carousel
      animated
      v-model="slide"
      navigation
      infinite
      padding
      arrows
      control-color="primary"
      transition-prev="slide-right"
      transition-next="slide-left"
      @mouseenter="autoplay = false"
      @mouseleave="autoplay = true"
      swipeable
      height="350px"
      class="rounded-borders"
    >
      <q-carousel-slide :name="1" class="column no-wrap">
        <div class="row fit justify-center items-center q-gutter-xs q-col-gutter no-wrap">
          <q-card class="my-card q-ma-md">
            <q-img class="rounded-borders col-6"
              src="../assets/card1.svg"
              basic
            >
            <div class="absolute-bottom text-h6">
              <q-btn flat>Pedro</q-btn>
            </div>
            </q-img>

          <q-card-section class="no-wrap">Pedro precisa de ajuda para conseguir uma cama. Ele mora com seus pais e mais 5 irmãos na comunidade dos Coelhos.</q-card-section>
          </q-card>

          <q-card class="my-card q-ma-md">
            <q-img class="rounded-borders col-6"
              src="../assets/card1.svg"
              basic
            >
            <div class="absolute-bottom text-h6">
              <q-btn flat>José</q-btn>
            </div>
            </q-img>

          <q-card-section class="no-wrap">Meu nome é José, eu e meus irmãos estamos precisando de alimentos e roupas, perdemos tudo em um incêndio.</q-card-section>
          </q-card>

        </div>
      </q-carousel-slide>
      <q-carousel-slide :name="2" class="column no-wrap">
        <div class="row fit justify-center items-center q-gutter-xs q-col-gutter no-wrap">
          <q-card class="my-card q-ma-md">
            <q-img class="rounded-borders col-6"
              src="../assets/card1.svg"
              basic
            >
            <div class="absolute-bottom text-h6 col-6">Pedro</div>
            </q-img>

          <q-card-section class="no-wrap">Pedro precisa de ajuda para conseguir uma cama. Ele mora com seus pais e mais 5 irmãos na comunidade dos Coelhos.</q-card-section>
          </q-card>

          <q-card class="my-card q-ma-md">
            <q-img class="rounded-borders col-6"
              src="../assets/card1.svg"
              basic
            >
            <div class="absolute-bottom text-h6">José</div>
            </q-img>

          <q-card-section class="no-wrap">Meu nome é José, eu e meus irmãos estamos precisando de alimentos e roupas, perdemos tudo em um incêndio.</q-card-section>
          </q-card>
        </div>
      </q-carousel-slide>
      <q-carousel-slide :name="3" class="column no-wrap">
        <div class="row fit justify-start items-center q-gutter-xs q-col-gutter no-wrap">
          <q-img class="rounded-borders col-6 full-height" src="https://cdn.quasar.dev/img/cat.jpg" />
          <q-img class="rounded-borders col-6 full-height" src="https://cdn.quasar.dev/img/linux-avatar.png" />
        </div>
      </q-carousel-slide>
    </q-carousel>
  </div>
</template>

<script>
export default {
  name: 'CasosRecentes',
  data () {
    return {
      slide: 1,
      autoplay: true
    }
  }
}
</script>

<style lang="sass" scoped>
.rec-container
  background: white;
  padding: 5px;

.my-card
  width: 100%
  max-width: 250px
  height: 300px
  padding: 10px

.txt-rec
  color: #5cc6d0;
  font-family: Montserrat;
  font-weight: bold;
  font-size: 36px;
  line-height: auto;
</style>
