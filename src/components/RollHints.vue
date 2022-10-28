<script>
export default {
    name: 'RollHints'
}
</script>

<template>
    <article class="article">
        <div>
            <h1>
                <span>#</span> Rolagem de dados
            </h1>
        </div>
        <div class="important-container">
            <h2 class="important">Pontos Importantes:</h2>
            <ul>
                <li>
                    &emsp;Por padrão as rolagens de dados estão desativadas devido aos usuários preferirem outros bots
                    de rolagem.
                </li><br>
                <li>
                    &emsp;Caso queira usar a rolagem do nosso bot basta enviar no canal em que deseja usa-lo o comando
                    <code>.rolagem</code>
                </li><br>
                <li>
                    &emsp;Para desativar as rolagens em um canal basta enviar <code>.desativa-rolagem</code>
                </li><br>
                <li>
                    &emsp;Para consultar o status atual dessa opção envie <code>.status-rolagem</code>
                </li>
            </ul>
        </div>
        <div class="roll-list">
            <ul>
                <li>Rolagem normal -> <code>1d20</code></li>
                <li>Rolagem com modificadores -> <code>1d20+5</code></li>
                <li>Rolagem com vantagem -> <code>1d20+5*</code></li>
                <li>Rolagem com desvantagem -> <code>1d20+5/</code></li>
                <li>Rolagem múltipla -> <code>2#d20+5</code></li>
            </ul>
        </div>
        <div class="important-container">
            <h2 class="important">Importante:</h2>
            <p>
                &emsp;O número máximo de dados e faces permitidas é <code>100</code>, acima disso o Bot ira considerar
                como <code>1</code>.
            </p>
        </div>
    </article>
</template>

<style scoped>
article {
    padding: 0 1rem;
}

ul {
    list-style: disc;
}

.important-container {
    background-color: #262A3B;
    padding: .6rem;
    border-radius: 10px;
    margin: 1rem .5rem;
}

.important-container ul {
    padding: 0 1.5rem;
}

.important {
    color: yellow;
    font-size: 1.3rem;
    text-transform: uppercase;
}

.roll-list {
    padding: 0 1rem;
}
</style>