<template>
    <div class="container">
        <div class="row">
            <div class="front col-6">
                <div class="skill-grid row">
                    <div class="col-12 col-sm-3 skill-column">
                        <div class="skill"><i class="fab fa-js"></i>JavaScript</div>
                        <div class="skill"><i class="fab fa-css3-alt"></i>CSS/CSS preprocessors</div>
                        <div class="skill"><i class="fab fa-vuejs"></i>Vue.js</div>
                        <div class="skill"><i class="fab fa-react"></i>React.js</div>
                        <div class="skill"><i class="fas fa-code"></i>Bootstrap</div>
                    </div>  
                    <div class="col-12 col-sm-3 skill-column">
                        <div class="skill"><i class="fab fa-python"></i>Python</div>
                        <div class="skill"><i class="fab fa-git"></i>Version Control</div>
                        <div class="skill"><i class="fas fa-server"></i>Hosting</div>  
                        <div class="skill"><i class="fab fa-aws"></i>AWS</div> 
                        <div class="skill"><i class="fab fa-wordpress"></i>WordPress/Shopify/HubSpot</div>                        
                    </div>            
                    <div class="col-12 col-sm-3 skill-column">
                        <div class="skill"><i class="fas fa-envelope-open-text"></i>Foundation/HTML Emails</div> 
                        <div class="skill"><i class="fas fa-book"></i>Documentation</div>           
                        <div class="skill"><i class="fas fa-mobile-alt"></i>Responsive Design</div>
                        <div class="skill"><i class="fas fa-universal-access"></i>Accessibility</div>
                    </div>
                    <div class="col-12 col-sm-3 skill-column">
                        <div class="skill"><i class="fas fa-search"></i>SEO</div>
                        <div class="skill"><i class="fas fa-chart-pie"></i>Salesforce</div>
                        <div class="skill"><i class="fab fa-adobe"></i>Photoshop</div>
                        <div class="skill"><i class="fas fa-tachometer-alt"></i>Testing</div>
                    </div>
                </div>
            </div>
            <div class="col-6 right">
                <div class="title-container">
                    <h1>Skills</h1>
                    <div class="img-skills"></div>
                </div>
            </div>
            <!-- <div class="img-container img-skills col-6"></div> -->
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
}
.row {
    height: 100%;
}
.right {
    position: relative;
}
.img-skills {
    background-image: url('~/assets/images/skills.png');
    background-size: cover;
    height: $imgHeight;
}
.title-container {
    text-align: right;
    position: $imgContainerPosition;
    bottom: -15px;
    right: 10px;
    width: 100%;
}
</style>