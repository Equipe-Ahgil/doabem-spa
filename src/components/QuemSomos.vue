<template>
  <div class="s-2">

    <div class="descricao-sobre">
      <div class="text-sobre">
        <p>Quem somos</p>
      </div>
    </div>

    <div class="text-descricao-sobre">
      <p>{{ lorem }}</p>
    </div>

  </div>
</template>

<script>
export default {
  name: 'QuemSomos',
  data () {
    return {
      lorem: 'Uma plataforma online, administrada pela Áhgil, empresa de multi plataformas digitais, atuante no mercado de tecnologia de web developer e mobile app. Nós vamos revolucionar o seu modo de captar doações, de maneira que você possa financiar a sua visão, o seu sonho. Faça a diferença em sua comunidade e ajude a melhorar a vida de pessoas em todo o mundo. Não estamos apenas vendendo uma plataforma de doações, queremos atender as suas necessidades, tornando real os seus planos de ajudar ao próximo. Temos as soluções perfeitas para você.'
    }
  }
}
</script>

<style lang="stylus" scoped>
@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');

.text-sobre p {
  color: $azulescuro;
  font-family: Lato;
  font-style: normal;
  font-weight: bold;
  font-size: 36px;
  line-height: 29px;
  }

.text-descricao-sobre p {
  font-family: Lato;
  font-size: 17px;
  font-style: normal;
  text-align: justify;
  }

.s-2{
  margin: auto;
  width: 70vw;
  padding: 30px;
}

.s-2 p {
  padding-bottom: 40px;
  margin: 0 0 0;
}

@media screen and (max-width: 768px) {
  .s-2{
    margin: auto;
    width: 90vw;
    padding: 30px;
  }
}

</style>
