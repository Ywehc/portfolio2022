<template>
    <div class="container">
        <div class="row mx-auto">
            <div class="col content text-center">
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
        </div>
    </div>
</template>

<style lang="scss" scoped>
.row {
    width: 100%;
}
.content {
    margin-top: 4em;
    display: flex;
    justify-content: center;
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