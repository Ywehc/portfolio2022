<template>
    <div class="container">
        <div class="row">
            <div class="front col-6">
                <div class="content-container">
                    <a href="https://www.cryptohawk.ca" target="_blank">
                    <div class="portfolio-card">
                        <div class="card-heading">
                            <h5 class="card-title">Cryptohawk (2021)</h5>
                            <i class="fas fa-coins"></i>
                        </div>
                        <p class="card-text">A cryptocurrency information and shopping app, built with the Vue.js ecosystem and Nomics API.</p>
                    </div>
                </a>
                <a href="https://propertrust.chriskieran.com" target="_blank">
                    <div class="portfolio-card">
                        <div class="card-heading">
                            <h5 class="card-title">Propertrust (2020)</h5>
                            <i class="fas fa-file-signature"></i>
                        </div>
                        <p class="card-text">A Vue.js app that uses two-way data binding to enable the user to generate a Real Estate Sales agreement.</p>
                    </div>
                </a>
                <a href="https://codepen.io/Ywehc/full/BMQEQW" target="_blank">
                    <div class="portfolio-card">
                        <div class="card-heading">
                            <h5 class="card-title">Hockey Quotes (2019)</h5>
                            <i class="fas fa-comment-dots"></i>
                        </div>
                        <p class="card-text">A fun React app built on Codepen which allows the user to generate a famous NHL hockey quote and Tweet it.</p>
                    </div>
                </a>
                <a class="btn btn-primary" href="https://github.com/Ywehc" role="button" target="_blank">
                    <strong>Github  </strong><i class="fab fa-github"></i>
                </a>
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
a {
    color: white;
    text-decoration: none;
}
.container {
    padding: $containerPadding;
    padding-top: $pagePaddingTop;
    position: relative;
}
.front {
    z-index: $pageZIndex;
    position: relative; 
    padding-left: 15em;
    padding-top: 8em;
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
    bottom: 228px;
    right: 10px;
    width: 100%;
}
.portfolio-card {
    width: 350px;
    border: 1px solid grey;
    border-radius: 5px;
    margin-bottom: 10px;
    padding: 10px;
    h5 {
        font-size: 20px;
        margin-bottom: 4px;
    }
    p {
        font-size: 14px;
    }
    i {
    font-size: 20px;
    }
}
.portfolio-card:hover {
    border: 1px solid white;
    background: white;
    color: black;
    cursor: pointer;
}
.card-heading {
    display: flex;
    justify-content: space-between;
}
.btn-primary {
    color: black;
    background: white;
    border: 1px solid grey;
}
.btn-primary:hover {
    background: black;
    color: white;
    border-color: white;
}
</style>