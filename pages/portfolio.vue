<template>
    <div class="container">
        <div class="row">
            <div class="front col-6">
                <h1>Portfolio</h1>
                <div class="row">
                    <div class="col-4">
                        <div class="card">
                            <img src="~/assets/images/cryptohawk.png" class="card-img-top" alt="...">
                            <div class="card-body">
                                <h5 class="card-title">Cryptohawk (2021)</h5>
                                <p class="card-text">A cryptocurrency information and shopping app, built with the Vue.js ecosystem and Nomics API.</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-4">
                        <div class="card">
                            <img src="~/assets/images/propertrust.png" class="card-img-top" alt="...">
                            <div class="card-body">
                                <h5 class="card-title">Propertrust (2020)</h5>
                                <p class="card-text">A Vue.js app that leans on Vuex state management to enable the user to generate a Sales agreement.</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-4">
                        <div class="card">
                            <img src="~/assets/images/hockeyquotes.png" class="card-img-top" alt="...">
                            <div class="card-body">
                                <h5 class="card-title">Hockey Quotes (2019)</h5>
                                <p class="card-text">A fun React app built on Codepen which allows the user to generate a Hockey quote and Tweet it.</p>
                            </div>
                        </div>
                    </div>  
                </div>
            </div>
            <div class="col-6 right">
                <div class="title-container">
                    <h1>Portfolio</h1>
                    <div class="img-portfolio"></div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import '~/assets/scss/_global.scss';

h1 {
    margin-bottom: $headingMarginBottom;
    font-size: $headingFontSize;
}
.card {
    width: 18rem;
    margin: auto;
    img {
        max-height: 220px;
    }
}
.card-text {
    font-size: 14px;
}
.container {
    padding: $containerPadding;
    padding-top: $pagePaddingTop;
    position: relative;
}
.front {
    z-index: $pageZIndex;
    position: relative; 
}
.img-portfolio {
    background-image: url('~/assets/images/portfolio.png');
    background-size: cover;
    height: $imgHeight;
}
.row {
    height: 100%;
}
.right {
    position: relative;
}
.title-container {
    text-align: right;
    position: $imgContainerPosition;
    bottom: -15px;
    right: 10px;
    width: 100%;
}
</style>