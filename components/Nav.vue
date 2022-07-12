<template>
    <div class="container">
        <div v-if="navOpen" class="row">
            <div class="col-0 col-xl-1 curve-container">
                <div class="curve d-none d-xl-block"></div>
            </div>
            <div class="col-12 col-xl-11 nav-container d-none d-xl-flex">
                <div class="nav-toggle d-xl-none">
                    <i class="far fa-caret-square-down" @click="navOpen = false"></i>
                </div>
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
            <div class="col-12 col-xl-11 nav-container d-xl-none">
                <div class="nav-toggle">
                    <i class="far fa-caret-square-down" @click="navOpen = false"></i>
                </div>
                <div class="row mobile-menu mx-auto">
                    <div class="col-6">
                        <div class="nav-pane">
                            <NuxtLink class="link" to="/about">about</NuxtLink>
                        </div>
                        <div class="nav-pane">
                            <NuxtLink class="link" to="/portfolio">portfolio</NuxtLink>
                        </div>
                    </div>
                    <div class="col-6">
                        <div class="nav-pane">
                            <NuxtLink class="link" to="/skills">skills</NuxtLink>
                        </div>
                        
                        <div class="nav-pane">
                            <NuxtLink class="link" to="/contact">contact</NuxtLink>
                        </div>
                    </div>
                </div>
                <div class="row mx-auto">
                    <div class="nav-pane">
                        <NuxtLink class="link" to="/">home</NuxtLink>
                    </div>
                </div>
            </div>
        </div>
        <div v-else>
            <div class="nav-toggle closed" @click="navOpen = true">
                <i class="far fa-caret-square-up"></i>
                <p class="text-center">menu</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            navOpen: true
        }
    },
}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/_global.scss';
@import '@/assets/scss/_nav.scss';

</style>