<template>
    <div class="container page-container">
        <div class="row">
            <div class="col-12 col-xl-6 right order-xl-last">
                <div class="title-container">
                    <h1 class="page-h1 d-none d-xl-block">Portfolio</h1>
                    <div class="img-portfolio img-page-heading"></div>
                </div>
            </div>
            <div class="front col-12 col-xl-6 order-xl-first">
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
                <p class="d-none d-xl-block">This application was built with Nuxt.js.</p>
                <a class="btn btn-primary" href="https://github.com/Ywehc" role="button" target="_blank">
                    <strong>Github  </strong><i class="fab fa-github"></i>
                </a>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import '~/assets/scss/_global.scss';

a {
    color: white;
    text-decoration: none;
}
.img-portfolio {
    background-image: url('~/assets/images/portfolio.png');
}
.row {
    height: 100%;
}
.title-container {
    bottom: 228px;
}
.portfolio-card {
    background-color: white;
    color: black;
    width: 350px;
    border: 1px solid grey;
    border-radius: 5px;
    margin-bottom: 20px;
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
    background: black;
    color: white;
    border-color: white;
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
@media screen and (max-width: 1200px) {
    .front {
        padding: 0;
        min-height: 0;
    }
    .title-container {
        bottom: 0;
    }
    .img-portfolio {
        margin: 0;
    }
    .portfolio-card {
        text-align: left;
        margin-bottom: 10px;
        h5 {
            font-size: 18px;
        }
        p {
            font-size: 14px;
        }
        width: auto;
    }
    .content-container {
        padding-right: 15px;
        padding-top: 15px;
        background: linear-gradient(to bottom right, #542624 0%, black 100%) 100% no-repeat;
    }
}
</style>