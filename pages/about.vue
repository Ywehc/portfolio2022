  
<template>
<div class="container">
    <div class="row">
        <div class="front col-7">
            <p>As a developer I'm drawn to the intersection of creativity and technical proficiency.</p>
            <p>The career path I'm on is really exciting. I love bringing code to life on the frontend with Javascript (mostly Vue.js) and CSS, but have also built foundations in PHP and Python.</p>
            <p>I enjoy nature, dogs, travel, music, astronomy, investing, fantasy sports, entrepreneurship and all sorts of other cool stuff. I'm fortunate to be able to spend lots of time with my amazing wife, son and dog, and they are a motivation boost every day.</p>
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
    bottom: -15px;
    right: 10px;
    width: 100%;
}
</style>