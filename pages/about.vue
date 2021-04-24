  
<template>
<div class="container">
    <div class="row">
        <div class="col">
            <h1>About Me</h1>
    <p>As a developer I'm drawn to the intersection of creativity and technical proficiency.</p>
    <p>The career path I'm on is really exciting. I love bringing code to life on the frontend with Javascript (mostly Vue.js) and CSS, but have also built foundations in PHP and Python. These fundamentals are allowing me to get my feet wet with technologies like Deep Learning.</p>
    <p>I enjoy nature, dogs, travel, music, astronomy, investing, fantasy sports, entrepreneurship and all sorts of other cool stuff. I'm fortunate to be able to spend lots of time with my amazing wife, son and dog, and they are a motivation boost every day.</p>
        </div>
        <div class="col img-container">
                <img src="~/assets/images/forest-wide.png" alt="Chris and son walking in forest">
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
p {
    font-size: $paragraphFontSize;
}
.img-container {
    display: flex;
    align-items: flex-end;
    flex-direction: column;
    img {
    width: 100%;
    align-self: flex-end;
    }
}
.container {
    padding: $containerPadding;
}
</style>