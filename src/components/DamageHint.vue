<script>
export default {
    name: 'DamageHint'
}
</script>

<template>
    <article class="article">
        <div class="title-box">
            <h1>
                <span>#</span> Controle de dano:
            </h1>
            <p class="extra">
                Para controle de dano é usado o simbolo <code>$</code> entre as informações da ordem de combate e o dano causado.
            </p>
        </div>

        <div class="tutorial-content">
            <div>
                <h2>
                    <i class="fa-solid fa-dice-d20"></i> Causando dano:
                </h2>
                <p>
                    &emsp;Para causar dano a um PdJ na batalha deve ser inserido primeiro a posição dele. Ex: <code>1$5</code>.
                </p>
                <div>
                    <img src="../assets/imgs-dmg/dano.png" alt="">
                </div>
            </div>
            <div>
                <h2>
                    <i class="fa-solid fa-dice-d20"></i> Recebendo cura:
                </h2>
                <p>
                    &emsp;De forma semelhante para cura, devendo apenas adicionar o valor negativo. Ex: <code>1$-2</code>.
                </p>
                <div>
                    <img src="../assets/imgs-dmg/cura.png" alt="">
                </div>
            </div>
            <div>
                <h2>
                    <i class="fa-solid fa-dice-d20"></i> Um PdJ caiu:
                </h2>
                <p>
                    &emsp;Para declarar um participante como incapacitado na batalha basta enviar o mesmo comando de dano apenas substituindo o dano por: <code>ko</code>. Ex: <code>4$ko</code>.
                </p>
                <div>
                    <img src="../assets/imgs-dmg/ko.png" alt="">
                </div>
                <p class="extra">
                    <strong>Extra:</strong> Quando um participante é incapacitado, uma frase ou brincadeira é enviada enfatizando o ocorrido.
                </p>
            </div>
            <div>
                <h2>
                    <i class="fa-solid fa-dice-d20"></i> Herois <strong>nunca</strong> morrem:
                </h2>
                <p>
                    &emsp;Mas a morte nem sempre é o fim, você sempre pode contar com aquele Clérigo ou Paladino gente boa (ou não) que vai te prestar socorro ou te trazer você de volta a vida em casos mais extremos... ou não!<br>Nessa ocasião basta substituir o dano/cura por <code>revive</code>. Ex: <code>4$revive</code>.
                </p>
                <div>
                    <img src="../assets/imgs-dmg/revive.png" alt="">
                </div>
                <p class="extra">
                    <strong>Extra:</strong> Quando um participante é revivido, uma frase ou brincadeira tambem é enviada enfatizando o ocorrido.
                </p>
            </div>
            <div>
                <h2>
                    <i class="fa-solid fa-dice-d20"></i> Dano/Cura em massa:
                </h2>
                <p>
                    &emsp;Os comando citados acima podem ser usados em mais de um participante por vez. Basta utilizar uma virgula para separar suas colocações.<br>Ex: O goblin e o kobold acabaram de receber uma bola de fogo na cabeça e foram conhecer seus respectivos criadores, envie <code>1,6$ko</code>.
                </p>
                <div>
                    <img src="../assets/imgs-dmg/cura-em-massa.png" alt="">
                </div>
            </div>
            <div class="box-commands expand-box">
                <h2>
                    <i class="fa-solid fa-dice-d20"></i> Da mesma forma os outros comandos:
                </h2>
                <div class="img-dmg-box">
                    <div>
                        <img src="../assets/imgs-dmg/dano-em-massa.png" alt="">
                    </div>
                    <div>
                        <img src="../assets/imgs-dmg/cura-em-massa.png" alt="">
                    </div>
                    <div>
                        <img src="../assets/imgs-dmg/revive-em-massa.png" alt="">
                    </div>
                </div>
            </div>
        </div>
    </article>
</template>

<style>
article {
    padding: 0 1rem;
}

span {
  color: #eb220e;
}

@media only screen and (min-width: 900px) {
    .img-dmg-box {
        display: flex;
    }

    .img-dmg-box div {
        padding: 0 1rem;
    }
}
</style>