<script>
export default {
    name: 'AddServer'
}
</script>

<template>
    <a href="https://www.google.com/" target="_blank"><button>Adicione ao seu <br/> Servidor.</button></a>
</template>

<style scoped>
button {
    background: linear-gradient(-45deg, #be302c, #370e0c, #22060a, #eb220e);
    background-size: 800% 400%;
    padding: .7em 2em;
    display: inline-block;
    border: none;
    border-radius: 10px;
    font-family: 'Roboto';
    font-size: 1.1rem;
    color: white;
    transition: all .5s ease-in-out;
    animation: gradient 15s infinite cubic-bezier(.62, .28, .23, .99) both;
    margin-right: .7rem;
    cursor: pointer
}

button:hover {
    animation: gradient 3s infinite;
    transform: scale(1.04);
}

button:active {
    animation: gradient 3s infinite;
    transform: scale(.95);
}

@keyframes gradient {
    0% {
        background-position: 0% 50%;
    }

    50% {
        background-position: 100% 50%;
    }

    100% {
        background-position: 0% 50%;
    }
}
</style>