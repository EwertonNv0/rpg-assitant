<script>
import AddServer from './components/AddServer.vue';
import AddServerStatic from './components/AddServerStatic.vue';
import IniLogo from './components/IniLogo.vue';
import ScrollDown from './components/ScrollDown.vue';
import RollHints from './components/RollHints.vue';
import IniHints from './components/IniHints.vue';
import DamageHint from './components/DamageHint.vue';
import GridHints from './components/GridHints.vue';
import FooterBox from './components/FooterBox.vue';

export default {
  name: "App",
  components: { IniLogo, AddServer, AddServerStatic, ScrollDown, RollHints, IniHints, DamageHint, GridHints, FooterBox }
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

  <section id="tutorial">
    <div class="space"></div>
  </section>

  <div id="sections">
    <section class="section roll">
      <RollHints />
    </section>

    <section class="section ini">
      <IniHints />
    </section>

    <section class="section dmg">
      <DamageHint />
    </section>

    <section class="section grid">
      <GridHints />
    </section>
  </div>
  
  <section>
    <div class="space"></div>
  </section>

  <footer id="footer-container">
    <FooterBox />
  </footer>
</template>

<style scoped>
span {
  color: #eb220e;
}

.space {
  margin: 7rem 1rem;
  border: 1px solid #eb220e90;
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
  padding-top: 10rem;
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

.scroll-icon-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 3rem;
}

@media only screen and (min-width: 900px) {
  .tutorial-content {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr;
  }

  #sections section {
    margin: 10rem 1.5rem;
    padding: 0 2rem;
  }

  .title {
    padding: 0 30%;
  }

  .destaque p {
    margin: 2% 0;
  }

  .space {
    border: 1px solid transparent;
  }
}
</style>
