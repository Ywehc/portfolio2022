  
<template>
<div class="container">
    <div class="row">
        <div class="front col-7">
            <div class="content-container">
                <p>What draws me to web development and especially frontend development is the intersection of creativity and technical ability.</p>

                <p>The career path I'm on is really exciting. I love bringing code to life on the frontend with Javascript (mostly Vue.js) and CSS, but have also built foundations in PHP and Python.</p>
                <p style="width: 90%">The best thing about life as a developer is collaboratively building awesome software as part of a cross-functional team of talented people while still being able to spend lots of time with my wife, son and dog.</p>
                <p style="width: 80%">Outside of web development I'm in to nature, dogs, travel, music, astronomy, hockey and fantasy hockey, snowboarding, spicy foods and more.</p>
            </div>
        </div>
        <div class="col-5 right">
            <div class="title-container">
                <h1>About Me</h1>
                <div class="img-about"></div>
            </div>
        </div>
    </div>
</div>
    
</template>

<style lang="scss" scoped>
@import '~/assets/scss/_global.scss';

h1 {
    font-size: $headingFontSize;
    margin-bottom: $headingMarginBottom;
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
.right {
    position: relative;
}
.img-about {
    background-image: url('~/assets/images/forest-wide.png');
    background-size: 100%;
    background-position-y: 95%;
    height: $imgHeight;
    margin: $paneMargin;
}
.title-container {
    text-align: right;
    position: $imgContainerPosition;
    bottom: 225px;
    right: 10px;
    width: 100%;
}
</style>