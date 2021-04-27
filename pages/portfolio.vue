<template>
    <div class="container">
        <h1>PORTFOLIO</h1>
        <div class="row">
            <div class="col-4">
                <div class="card">
                <img src="~/assets/images/cryptohawk.png" class="card-img-top" alt="...">
                <div class="card-body">
                    <h5 class="card-title">Cryptohawk</h5>
                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                </div>
            </div>
            </div>
            <div class="col-4">
                <div class="card">
                <img src="~/assets/images/propertrust.png" class="card-img-top" alt="...">
                <div class="card-body">
                    <h5 class="card-title">Propertrust</h5>
                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                </div>
            </div>
            </div>
            <div class="col-4">
                <div class="card">
                <img src="~/assets/images/hockeyquotes.png" class="card-img-top" alt="...">
                <div class="card-body">
                    <h5 class="card-title">Hockey Quotes</h5>
                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                </div>
            </div>
            </div>  
        </div>
    </div>   
</template>

<style lang="scss" scoped>
@import '~/assets/scss/_global.scss';

// .container {
//     margin: $containerMargin;
// }
h1 {
    text-align: center;
}
.card {
    width: 18rem;
    margin: auto;
    img {
        max-height: 220px;
    }
}
</style>