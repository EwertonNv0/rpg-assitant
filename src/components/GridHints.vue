<script>
export default {
    name: 'GridHints'
}
</script>

<template>
    <article class="article">
        <div>
            <h1><span>#</span> Grid</h1>
            <p class="extra">
                Como forma de suporte o bot também conta com um grid basico para auxilio em batalhas.<br>Aconcelhamos seu uso apenas em pequenos conflitos, onde não haja um número muito grande de inimigos e/ou jogadores.
            </p>
        </div>

        <div>
            <h2>
                <i class="fa-solid fa-dice-d20"></i> Iniciando o Grid
            </h2>
            <p>
                &emsp;Para criar um Grid basta enviar <code>.grid;x,y</code> o tamanho máximo dele é de 20x20.
            </p>
            <p class="extra">
                Com o <code>X</code> representando a largura e o <code>Y</code> a altura.
            </p>
            <p>Exemplo:</p>
            <div>
                <img src="../assets/imgs-grid/grid.png" alt="">
            </div>
            <p class="extra">
                <strong class="attention">Atenção:</strong> Assim como a iniciativa, cada canal tem seu proprio grid, iniciar um grid <strong>apaga imediatamente</strong> o grid anterior.
            </p>
        </div>

        <div>
            <h2>
                <i class="fa-solid fa-dice-d20"></i> Adicionando Participantes:
            </h2>
            <p>
                &emsp;Para adicionar participantes envie a sigla do participante <strong>(máx. 2 caráteres)</strong> seguido por <code>';'</code> e após isto a letra e o número referente as coordenadas.
            </p>
            <p>Exemplo:</p>
            <div>
                <img src="../assets/imgs-grid/add-par.png" alt="">
            </div>
        </div>

        <div>
            <h2>
                <i class="fa-solid fa-dice-d20"></i> Movendo Participantes:
            </h2>
            <p>
                &emsp;Para mudar um participante de lugar basta reenviar o comando acima com as novas coordenadas.
            </p>
            <div>
                <img src="../assets/imgs-grid/move-par.png" alt="">
            </div>
        </div>

        <div>
            <h2>
                <i class="fa-solid fa-dice-d20"></i> Retirando Participantes:
            </h2>
            <p>
                &emsp;Para retirar um participante basta colocar 0 na coordenada.
            </p>
            <div>
                <img src="../assets/imgs-grid/retira-par.png" alt="">
            </div>
        </div>

        <div>
            <h2>
                <i class="fa-solid fa-dice-d20"></i> Exibindo o Grid:
            </h2>
            <p>
                &emsp;Para ver o grid a qualquer momento envie: <code>.exibegrid</code> .
            </p>
            <div>
                <img src="../assets/imgs-grid/exibe.png" alt="">
            </div>
        </div>
    </article>
</template>

<style scoped>
article {
    padding: 0 1rem;
}

span {
  color: #eb220e;
}

.attention {
    color: yellow;
}
</style>