<template>
    <div class="container">
        <div class="row">
            <div class="col-1 curve-container">
                <div class="curve"></div>
            </div>
            <div class="col-11 nav-container">
                <div class="nav-pane pane-5">
                    <NuxtLink class="link" to="/">home</NuxtLink>
                </div>
                <div class="nav-pane pane-4">
                    <NuxtLink class="link" to="/about">about</NuxtLink>
                </div>
                <div class="nav-pane pane-3">
                    <NuxtLink class="link" to="/skills">skills</NuxtLink>
                </div>
                <div class="nav-pane pane-2">
                    <NuxtLink class="link" to="/portfolio">portfolio</NuxtLink>
                </div>
                <div class="nav-pane pane-1">
                    <NuxtLink class="link" to="/contact">contact</NuxtLink>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import '@/assets/scss/_global.scss';
@import '@/assets/scss/_nav.scss';

</style>