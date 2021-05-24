<template>
    <div class="container page-container">
        <div class="row">
            <div class="front col-7">
                <div class="content-container">
                        <div class="skill">
                            <div class="icon-container"><i class="fab fa-js"></i></div>
                            JavaScript
                        </div>
                        <div class="skill">
                            <div class="icon-container"><i class="fab fa-css3-alt"></i></div>
                            CSS/SASS/Bootstrap
                        </div>
                        <div class="skill">
                            <div class="icon-container"><i class="fab fa-vuejs"></i></div>
                            Vue.js/Nuxt.js
                        </div>
                        <div class="skill">
                            <div class="icon-container"><i class="fab fa-react"></i></div>
                            React.js
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
                            CMS - WordPress/Shopify/HubSpot/Salesforce
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
                        <div class="skill">
                            <div class="icon-container"><i class="fab fa-adobe"></i></div>
                            Photoshop
                        </div>
                </div>
            </div>
            <div class="col-5 right">
                <div class="title-container">
                    <h1 class="page-h1">Skills</h1>
                    <div class="img-skills img-page-heading"></div>
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
    font-size: 17px;
    display: flex;
}
.icon-container {
    width: 40px;
}
</style>