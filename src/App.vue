<script>
import AddServer from './components/AddServer.vue';
import AddServerStatic from './components/AddServerStatic.vue';
import IniLogo from './components/IniLogo.vue';
import ScrollDown from './components/ScrollDown.vue';
import RollHints from './components/RollHints.vue';
import IniHints from './components/IniHints.vue';

export default {
  name: "App",
  components: { IniLogo, AddServer, AddServerStatic, ScrollDown, RollHints, IniHints }
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
    <article>
      <div id="content">
        <div class="destaque">
          <h1 class="title">
            Tenha <span>mais agilidade</span> durante seus <span>combates!</span>
          </h1>
          <p>
            Deixe seus combates mais dinâmicos e organizados!
          </p>
          <div class="add-button">
            <AddServerStatic />
          </div>
        </div>
      </div>
      <div class="scroll-icon-container">
        <ScrollDown />
      </div>
    </article>
  </section>

  <section>
    <RollHints />
  </section>

  <section>
    <IniHints />
  </section>
</template>

<style scoped>
span {
  color: #eb220e;
}

#top-bar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: fixed;
  z-index: 1000;
  background-color: #191C27;
  box-shadow: 0 0 15px 5px #191C27;
  top: 0;
  width: 100%;
}

.logo-container {
  padding: 20px 10px;
}

.logo {
  width: 5rem;
}

#content {
  padding: 10px;
  color: white;
  font-family: 'Roboto';
  padding-top: 12rem;
}

.title {
  font-size: 2.5rem;
  text-align: center;
}

.destaque p {
  text-align: center;
  padding: 2rem 0;
  color: #EEEEEE99;
}

.add-button {
  display: flex;
  justify-content: center;
}

.scroll-icon-container{
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 4rem;
}
</style>
