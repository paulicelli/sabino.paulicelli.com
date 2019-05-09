<template>
    <div class="HeaderTitle">
        <div id="paulicelli">
            <h1>paulicelli</h1>
        </div>
        <div id="divider"></div>
        <div id="menuButton">
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

#divider {
    display: none;
}

#menuButton {
    background-color: var(--background);
    display: inline-flex;
    width: 20vw;

    align-items: center;
    justify-content: center;
}

#menuButton > button > div {
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
    padding-top: 1em;
    float: right;
}

#sabino > h1 {
    font-weight: bold !important;
}

@media (min-width: 48rem) {
    #menuButton {
        display: none;
    }

    h1 {
    font-size: 4em;
    text-transform: uppercase;
    }

    .HeaderTitle {
        position: initial;
        margin: 2em 10vw;
        width: 80vw;
        height: 8em;
        display: flex;
        transform: rotate(-10deg);
    }

    #paulicelli {
    background-color: var(--background);
    display: inline-block;
    width: inherit;
    align-self: flex-start;
    }

    #paulicelli > h1 {
        text-align:right;
    }

    #divider {
        display: inline-block;
        width: 0;
        height: 100%;
        border-left: solid 4px var(--main-color);
    }

    #sabino {
        writing-mode: horizontal-tb;
        display: inline-block;
        align-self: flex-end;
        width: inherit;
        padding: 0;
        margin-right: 4em;
        float: none;
    }
}
</style>
