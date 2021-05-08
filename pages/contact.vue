<template>
    <div class="container">
        <div class="row">
            <div class="front col-6">
                <h1 class="section-heading">Contact Me</h1>
                <div class="row">
                    <form   class="contact-form" 
                        action="https://formspree.io/chriskierandevelopment@gmail.com" 
                        target="_blank" 
                        method="POST"
                >   
                    <div class="col-12 col-sm-8 form-top">
                        <div class="form-group">
                            <label for="name"></label>
                            <input  class="form-input form-control" 
                                    type="text" 
                                    name="name" 
                                    id="name" 
                                    placeholder="Name" 
                                    required
                            >
                        </div>
                        <div class="form-group">
                            <label for="email"></label>
                            <input  class="form-input form-control" 
                                    type="email" 
                                    name="email" 
                                    id="email" 
                                    placeholder="Email" 
                                    required
                            >
                        </div>
                        <div class="form-group">
                            <label for="phone"></label>
                            <input  class="form-input form-control" 
                                    type="tel" 
                                    name="phone" 
                                    id="phone" 
                                    placeholder="Phone"
                            >
                        </div> 
                    </div>
                    <div class="col-7 col-sm-4">
                        <a href="https://www.linkedin.com/in/chris-kieran" target="_blank">
                            <div class="linkedin-container">
                                <p class="linkedin">Connect with me on LinkedIn</p>
                                <i class="fab fa-linkedin-in"></i>
                            </div>
                        </a>              
                    </div> 
                        <div class="form-group col-12">
                            <label for="message"></label>
                            <textarea  
                                    class="form-input form-control" 
                                    rows="4"
                                    type="text" 
                                    name="message" 
                                    id="message"
                                    placeholder="How can I help you?" 
                                    required
                            ></textarea>
                            <div>
                                <div>
                                    <button class="btn btn-outline-light button-submit" type="submit" value="Send">
                                        Send
                                    </button> 
                                </div>
                            </div>
                        </div>    
                    </form>
                </div>
            </div>
            <div class="col-6 right">
            <div class="title-container">
                <h1>Contact Me</h1>
                <div class="img-contact"></div>
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
}
.img-contact {
    background-image: url('~/assets/images/contact.png');
    background-size: 110%;
    background-position-y: 45%;
    background-position-x: 30%;
    height: $imgHeight;
}
.title-container {
    text-align: right;
    position: $imgContainerPosition;
    bottom: 174px;
    right: 10px;
    width: 100%;
}
</style>