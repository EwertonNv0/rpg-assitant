<script>
export default {
    name: 'AddServerStatic'
}
</script>

<template>
    <a href="https://www.google.com/" target="_blank">
        <button>
            <img src="../assets/bad-cat.png" alt="bad cat" id="bad-cat">
            Adicione ao seu Servidor.
        </button>
    </a>
</template>

<style scoped>
button {
    background: linear-gradient(-45deg, #be302c, #370e0c, #22060a, #eb220e);
    box-shadow: 0 0 10px 1px #eb220e70;
    background-size: 800% 400%;
    padding: .8em 2em;
    display: inline-flex;
    border: none;
    border-radius: 10px;
    font-family: 'Roboto';
    font-size: 1.1rem;
    color: white;
    transition: all .5s ease-in-out;
    cursor: pointer;
    align-items: center;
}

button:hover {
    transform: scale(1.04);
}

button:active {
    transform: scale(.95);
}

#bad-cat{
    width: 1.5rem;
    margin-right: .2rem;
}
</style>