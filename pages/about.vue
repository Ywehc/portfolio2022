  
<template>
<div class="container page-container">
    <div class="row">
        <div class="front col-7">
            <div class="content-container">
                <p>What draws me to web development and especially frontend development is the intersection of creativity and technical ability.</p>
                <p>The career path I'm on is really exciting. I love bringing code to life on the frontend with Javascript (mostly Vue.js) and CSS, but have also built foundations in PHP and Python.</p>
                <p style="width: 90%">The best thing about being a developer is collaboratively building awesome software as part of a team of talented people while still being able to spend lots of time with my wife, son and dog.</p>
                <p style="width: 80%">Outside of web development I'm in to nature, dogs, travel, music, astronomy, hockey and fantasy hockey, snowboarding, spicy foods and more.</p>
            </div>
        </div>
        <div class="col-5 right">
            <div class="title-container">
                <h1 class="page-h1">About Me</h1>
                <div class="img-about img-page-heading"></div>
            </div>
        </div>
    </div>
</div>
    
</template>

<style lang="scss" scoped>
@import '~/assets/scss/_global.scss';

.front {
    .narrow {
        width: 80%;
    }
    p {
        font-size: $paragraphFontSize;
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
</style>