<template>
    <div class="container page-container">
        <div class="row">
            <div class="col-12 col-xl-5 right order-xl-last">
                <div class="title-container">
                    <h1 class="page-h1 d-none d-xl-block">Skills</h1>
                    <div class="img-skills img-page-heading"></div>
                </div>
            </div>
            <div class="front col-12 col-xl-7 order-xl-first">
                <div class="content-container">
                        <div class="skill">
                            <div class="icon-container"><i class="fab fa-js"></i></div>
                            JavaScript / Vue.js / React.js
                        </div>
                        <div class="skill">
                            <div class="icon-container"><i class="fab fa-css3-alt"></i></div>
                            CSS & many CSS frameworks
                        </div>
                        <div class="skill">
                            <div class="icon-container"><i class="fas fa-code"></i></div>
                            REST API's
                        </div>
                        <div class="skill">
                            <div class="icon-container"><i class="fab fa-python"></i></div>
                            Python
                        </div>
                        <div class="skill">
                            <div class="icon-container"><i class="fab fa-git"></i></div>
                            Version Control
                        </div>
                        <div class="skill">
                            <div class="icon-container"><i class="fas fa-server"></i></div>
                            Web Administration
                        </div>  
                        <div class="skill">
                            <div class="icon-container"><i class="fab fa-wordpress"></i></div>
                            Content Management Systems
                        </div> 
                        <div class="skill">
                            <div class="icon-container"><i class="fas fa-envelope-open-text"></i></div>
                            HTML Email Development
                        </div> 
                        <div class="skill">
                            <div class="icon-container"><i class="fas fa-book"></i></div>
                            Documentation
                        </div>           
                        <div class="skill">
                            <div class="icon-container"><i class="fas fa-mobile-alt"></i></div>
                            UX
                        </div>
                        <div class="skill">
                            <div class="icon-container"><i class="fas fa-universal-access"></i></div>
                            Accessibility
                        </div> 
                        <div class="skill">
                            <div class="icon-container"><i class="fas fa-search"></i></div>
                            SEO
                        </div>
                        <!-- <div class="skill">
                            <div class="icon-container"><i class="fas fa-tachometer-alt"></i></div>
                            Testing
                        </div> -->
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import '~/assets/scss/_global.scss';

i {
    margin: 8px 8px 8px 0;
}
.row {
    height: 100%;
}
.img-skills {
    background-image: url('~/assets/images/skills.png');
    background-position-x: 80px;
    background-position-y: 40%;
}
.title-container {
    bottom: 228px;
}
.skill {
    font-size: $paragraphFontSize;
    display: flex;
}
.icon-container {
    width: 40px;
}

@media screen and (max-width: 1200px) {
    .front {
        padding: 0;
        min-height: 0;
    }
    .title-container {
        bottom: 0;
    }
    .img-skills {
        margin: 0;
        background-size: cover;
        background-position-x: center;
    }
    .content-container {
        padding: 1em 2em;
        margin-left: 15px;
        background: linear-gradient(to bottom right, #2a2454 0%, black 100%) 100% no-repeat;
        font-size: $mobileParagraphFontSize;
    }
}
</style>