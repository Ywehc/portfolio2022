<template>
    <div class="container">
        <div class="icon-container">
            <a href="https://github.com/Ywehc" role="button" target="_blank">
                <i class="fab fa-github-square"></i>
            </a>
        </div>
        <div class="icon-container">
            <a href="https://www.linkedin.com/in/chris-kieran" role="button" target="_blank">
                <i class="fab fa-linkedin"></i>
            </a>
        </div>
        <div class="icon-container">
            <NuxtLink class="link" to="/contact"><i class="fas fa-envelope"></i></NuxtLink>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.container {
    margin-top: 4em;
    padding-left: 35em;
    display: flex;
    .icon-container {
        margin: 10px;
        width: 50px;
        height: 50px;
    }
    a {
        color: black;
    }
    i {
        font-size: 24px;
    }
    i:hover {
        font-size: 34px;
    }
}
</style>