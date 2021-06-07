  
<template>
<div class="container page-container">
    <div class="row">
        <div class="col-12 col-xl-5 right order-xl-last">
            <div class="title-container">
                <h1 class="page-h1 d-none d-xl-block">About Me</h1>
                <div class="img-about img-page-heading"></div>
            </div>
        </div>
        <div class="front col-12 col-xl-7 order-xl-first">
            <div class="content-container">
                <p>What draws me to web development and especially frontend development is the intersection of creativity and technical ability.</p>
                <p>The career path I'm on is really exciting. I love bringing code to life on the frontend with Javascript (mostly Vue.js) and CSS, but have also built backend foundations in PHP, Python, and Node.js.</p>
                <p class="p3">The best thing about being a developer is collaboratively building awesome software as part of a team of talented people while still being able to spend lots of time with my wife, son and dog.</p>
                <p class="p4">Outside of web development I'm in to nature, dogs, travel, music, astronomy, hockey and fantasy hockey, snowboarding, spicy foods and more.</p>
            </div>
        </div>
    </div>
</div>
    
</template>

<style lang="scss" scoped>
@import '~/assets/scss/_global.scss';

.front {
    p {
        font-size: $paragraphFontSize;
    }
    .p3 {
        width: 90%;
    }
    .p4 {
        width: 80%;
    }
}
.row {
    height: 100%;
}
.img-about {
    background-image: url('~/assets/images/forest-wide.png');
    background-position-y: 95%;
    margin: $paneMargin;
}
.title-container {
    bottom: 225px;
}
@media screen and (max-width: 1200px) {
    .front {
        padding: 0;
    }
    .title-container {
        bottom: 0;
    }
    .img-about {
        margin: 0;
    }
    .p3, .p4 {
        width: 100%!important;
    }
}
</style>