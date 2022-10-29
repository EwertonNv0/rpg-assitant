<script>
export default {
    name: 'IniHints'
}
</script>

<template>
    <article class="article">
        <div class="title-box">
            <h1>
                <span>#</span> Iniciativa
            </h1>
        </div>

        <div class="tutorial-content">
            <div class="inicio">
                <h2><i class="fa-solid fa-dice-d20"></i> Inicio de uma Batalha:</h2>
                <p>
                    &emsp;O mestre deve enviar iniciativa e aparecerá a seguinte resposta:
                </p><br>
                <div>
                    <img src="../assets/imgs-ini/iniciativa.png" alt="">
                </div>
            </div>
            <div>
                <h2><i class="fa-solid fa-dice-d20"></i> Jogadores entrando:</h2>
                <p>
                    &emsp;Em seguida os jogadores enviam <code>ini</code> seguido do seu bônus então receberá o valor da sua
                    iniciativa para aquela batalha.
                </p>
                <div>
                    <img src="../assets/imgs-ini/ini.png" alt="">
                </div>
            </div>
            <div class="npcs">
                <h2><i class="fa-solid fa-dice-d20"></i> NPCs:</h2>
                <p>
                    &emsp;Para adcionar um npc na batalha, basta inserir o nome dele após o ini. Exemplo:
                    <code>ini monstro</code>
                </p>
                <div>
                    <img src="../assets/imgs-ini/monstro.png" alt="">
                </div>
            </div>
            <div class="mods expand-box">
                <h2><i class="fa-solid fa-dice-d20"></i> Modificadores:</h2>
                <p>&emsp;Os detalhes a seguir se aplicam a jogadores e npcs.</p>
                <div class="recuo display-flex">
                    <div>
                        <h3>
                            <i class="fa-solid fa-dice-d6"></i> Modificador positivo:
                        </h3>
                        <p>
                            &emsp;Caso seu personagem possua algum bônus de iniciativa, utilize o bônus após o ini. Ex: <code>ini +5</code>.
                        </p>
                        <div>
                            <img src="../assets/imgs-ini/ini+.png" alt="">
                        </div>
                    </div>
                    <div>
                        <h3>
                            <i class="fa-solid fa-dice-d6"></i> Modificador negativo:
                        </h3>
                        <p>
                            &emsp;Caso seu modificador de iniciativa seja negativo, utilize o sinal de <code>-</code> após o
                            ini. Ex: <code>ini -5</code>.
                        </p>
                        <div>
                            <img src="../assets/imgs-ini/ini-.png" alt="">
                        </div>
                    </div>
                </div>
            </div>
            <div class="set-valor expand-box">
                <h2> <i class="fa-solid fa-dice-d20"></i> Valor pré-definido:</h2>
                <p>
                    &emsp;Para usar um valor pré-definido de iniciativa ao invés de uma rolagem, baste inserir o valor entre
                    <code>()</code>. Ex: <code>ini (15)</code>.
                </p>
                <div class="pre-def-value">
                    <img src="../assets/imgs-ini/ini().png" alt="">
                </div>
                <p>
                    &emsp;Todos os casos acima são validos para NPCS, apenas use um <code>.</code> para separa-los. Ex:
                    <code>ini monstro.+3</code> ou <code>ini monstro.(10)</code>.
                </p>
                <div class="exemples display-flex">
                    <div>
                        <img src="../assets/imgs-ini/ini-monstro+.png" alt="">
                    </div>
                    <div>
                        <img src="../assets/imgs-ini/ini-monstro().png" alt="">
                    </div>
                </div>
            </div>
            <div class="hordas">
                <h2><i class="fa-solid fa-dice-d20"></i> Hordas:</h2>
                <p>
                    &emsp;Para adicionar mais de um npc simultâneo use a quantidade seguida de um <code>#</code> e nome do
                    monstro. Ex: <code>ini 3#orc.+2</code>.
                </p>
                <div>
                    <img src="../assets/imgs-ini/horda.png" alt="">
                </div>
            </div>
            <div class="combate">
                <h2><i class="fa-solid fa-dice-d20"></i> Hora da Batalha:</h2>
                <p>
                    &emsp;Depois de todos participantes rolarem suas iniciativas basta enviar <code>batalha</code> para ver
                    a ordem de combate e o dano sofrido de cada participante.
                </p>
                <div>
                    <img src="../assets/imgs-ini/batalha.png" alt="">
                </div>
            </div>
            <div class="extra expand-box">
                <p>
                    <strong>Extra:</strong> Para ver o valor de Iniciativa dos participantes envie <code>batalha.i</code>
                </p>
                <div>
                    <img src="../assets/imgs-ini/batalha-i.png" alt="">
                </div>
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

ul {
    list-style: disc;
}

.recuo {
    border-left: 2px solid #eb220e;
    margin-left: 1.3rem;
    padding-left: .5rem;
}

@media only screen and (min-width: 900px) {
    .display-flex {
        display: flex;
    }

    .recuo {
        border-left: none;
        margin-left: 0;
        padding-left: 0;
    }

    .recuo div {
        padding: 0 2rem;
    }

    .exemples div {
        padding: 0 1rem;
    }

    .pre-def-value img {
        width: 60%;
    }
}
</style>