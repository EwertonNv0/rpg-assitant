<script>
import AddServer from './components/AddServer.vue';
import AddServerStatic from './components/AddServerStatic.vue';
import IniLogo from './components/IniLogo.vue';

export default {
  name: "App",
  components: { IniLogo, AddServer, AddServerStatic }
}
</script>

<template>
  <header>
    <div id="top-bar">
      <div class="logo-container">
        <IniLogo />
      </div>
      <div>
        <AddServer />
      </div>
    </div>
  </header>

  <section>
    <div id="content">
      <h1 class="title">
        Tenha <span>mais agilidade</span> durante seus <span>combates!</span>
      </h1>
      <div class="add-button">
        <AddServerStatic />
      </div>
      <div class="explain-container">
        <h1>
          &emsp;Este bot tem o intuito de deixar a jogatina a distância um pouco mais simples, no momento conta com apenas essas funções mas olha só, um spoiler, enquanto você lê isso outras funções estão sendo desenvolvidas, acompanhe nosso Instagram para não perder nenhuma novidade.
        </h1>
        <h2>
          &emsp;Qualquer duvida, sugestão, reporte de bugs ou qualquer outro assunto não exite em entrar em contato em um dos canais mencionados acima.
        </h2>
      </div>
    </div>
  </section>
</template>

<style scoped>
#top-bar{
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.logo-container{
  padding: 20px 10px;
}
.logo {
  width: 5rem;
}
#content{
  padding: 10px;
  color: white;
  font-family: 'Roboto';
}
.title{
  font-size: 2.5rem;
  text-align: center;
}
.add-button{
  display: flex;
  justify-content: center;
  padding-top: 1rem;
}
.explain-container{
  margin-top: 3rem;
}
span{
  color: #eb220e;
}
</style>
