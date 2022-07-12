  
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
                <p>Hailing from Toronto, Ontario I now live in Calgary, Alberta with my wonderful family.</p>
                <p>What draws me to web development is the breadth and depth of the field and learning something new every day.</p>
                <!-- <p>I think what makes it such a great fit for me is I posess a combination of strong problem solving abilities, technical precision, creative thinking and user empathy.</p> -->
                <p class="p3">The career path I'm on is really exciting! I love bringing code to life and building interactive things with JavaScript and CSS.</p>
                <p class="p4">Outside of software development I enjoy spending time with my wife, son and dog, hiking, snowboarding, travel, listening to music and managing my fantasy hockey team.</p>
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
        width: 100%;
    }
    .p3, .p4 {
        width: 100%!important;
    }
    .content-container {
        padding: 1em 2em 0 2em;
        background: linear-gradient(to bottom right, #422454 0%, black 100%) 100% no-repeat;
        text-align: left;
        font-size: $mobileParagraphFontSize;
        line-height: normal;
    }
}
</style>