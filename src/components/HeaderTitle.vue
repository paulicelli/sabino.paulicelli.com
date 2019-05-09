<template>
    <div class="HeaderTitle">
        <div id="paulicelli">
            <h1>paulicelli</h1>
        </div>
        <div id="menu">
            <button @click="$emit('hide-nav')">
                <div></div>
                <div></div>
                <div></div>
            </button>
        </div>
        <div id="sabino">
            <h1>sabino</h1>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HeaderTitle',
}
</script>

<style scoped>
h1 {
    font-size: 15vw;
    text-transform: uppercase;
}

button {
    background-color: transparent;
    border: none;
}

.HeaderTitle {
    position: fixed;
}

#paulicelli {
    background-color: var(--background);
    display: inline-block;
    width: 80vw;
}

#menu {
    background-color: var(--background);
    display: inline-flex;
    width: 20vw;

    align-items: center;
    justify-content: center;
}

#menu > button > div {
    background-color: var(--main-color);

    width: 10vw;
    height: 2vw;
    margin: 0.5em 0;
}

#sabino {
    background-color: var(--background);
    color: var(--accent-color);
    text-align: end;
    writing-mode: vertical-rl;

    width: 20vw;
    padding-top: 2em;
    float: right;
}

#sabino > h1 {
    font-weight: bold !important;
}
</style>
