<script>
export default {
    name: 'FooterBox'
}
</script>

<template>
    <article class="articles">
        <div class="extra">
            <p>Este bot tem o intuito de deixar sua sessão a distância um pouco mais simples e no momento conta com
                apenas essas funções.</p>
            <p>Caso você tenha uma ideia de melhoria e gostaria que adicionassemos, por favor, nos envie sua ideia pelo
                nosso canal do <a class="discord" href="https://discord.com/invite/XuNnEwYbx4"><i class="fa-brands fa-discord"></i>
                    Discord</a> e vamos considerar e implementar assim que possivel.</p>
        </div>

        <div>
            <p>
                Copyright &copy; 2022 | <a href="http://nivelzero.com.br/" target="_blank">Nível Zero</a>
            </p>
        </div>
    </article>
</template>

<style scoped>
.discord {
    color: #5865F2;
    font-weight: 700;
}

.discord:hover {
    text-decoration: underline;
}

.articles {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.articles div:nth-child(2) {
    margin: .8rem 0;
}

.articles div:nth-child(2) a {
    color: white;
    text-decoration: underline;
}
</style>