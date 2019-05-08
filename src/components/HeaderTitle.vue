<template>
    <div class="HeaderTitle">
        <div id="paulicelli">
            <h1>paulicelli</h1>
        </div>
        <div id="menu">
            <button @click="$emit('hide-nav')">
                <h2>iii</h2>
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

h2 {
    font-size: 12vw;
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
    background-color: AntiqueWhite;
    display: inline-block;
    width: 80vw;
}

#menu {
    background-color: AntiqueWhite;
    display: inline-flex;
    width: 20vw;
    writing-mode: vertical-rl;

    align-items: center;
    justify-content: center;
}

#sabino {
    background-color: AntiqueWhite;
    color: var(--accent-color);
    text-align: end;
    writing-mode: vertical-rl;

    width: 20vw;
    padding-top: 1em;
    float: right;
}
</style>
