<script>
export default {
    name: 'ScrollDown'
}
</script>

<template>
    <a href="#tutorial">
        <p>Veja mais...</p>
        <div class="scrolldown" style="--color: skyblue">
            <div class="chevrons">
                <div class="chevrondown"></div>
                <div class="chevrondown"></div>
            </div>
        </div>
    </a>
</template>

<style scoped>
a {
    display: flex;
    flex-direction: column;
    align-items: center;
}

p {
    color: white;
    font-family: 'Roboto';
    margin-bottom: .4rem;
}

.scrolldown {
    --color: white;
    --sizeX: 30px;
    --sizeY: 50px;
    position: relative;
    width: var(--sizeX);
    height: var(--sizeY);
    margin-left: var(sizeX / 2);
    border: calc(var(--sizeX) / 10) solid #eb220e;
    border-radius: 50px;
    box-sizing: border-box;
    margin-bottom: 16px;
    cursor: pointer;
}

.scrolldown::before {
    content: "";
    position: absolute;
    bottom: 30px;
    left: 50%;
    width: 6px;
    height: 6px;
    margin-left: -3px;
    background-color: #eb220e;
    border-radius: 100%;
    animation: scrolldown-anim 2s infinite;
    box-sizing: border-box;
    box-shadow: 0px -5px 3px 1px #eb220e60;
}

@keyframes scrolldown-anim {
    0% {
        opacity: 0;
        height: 6px;
    }

    40% {
        opacity: 1;
        height: 10px;
    }

    80% {
        transform: translate(0, 20px);
        height: 10px;
        opacity: 0;
    }

    100% {
        height: 3px;
        opacity: 0;
    }
}

.chevrons {
    padding: 6px 0 0 0;
    margin-left: -3px;
    margin-top: 48px;
    width: 30px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.chevrondown {
    margin-top: -6px;
    position: relative;
    border: solid #eb220e;
    border-width: 0 3px 3px 0;
    display: inline-block;
    width: 10px;
    height: 10px;
    transform: rotate(45deg);
}

.chevrondown:nth-child(odd) {
    animation: pulse54012 500ms ease infinite alternate;
}

.chevrondown:nth-child(even) {
    animation: pulse54012 500ms ease infinite alternate 250ms;
}

@keyframes pulse54012 {
    from {
        opacity: 0;
    }

    to {
        opacity: 0.5;
    }
}
</style>