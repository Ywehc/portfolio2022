<template>
    <div class="container">
        <div class="row">
            <div class="front col-6">
                <div class="content-container">
                    <div class="row">
                    <form   class="contact-form" 
                            action="https://formspree.io/chriskierandevelopment@gmail.com" 
                            target="_blank" 
                            method="POST"
                    >   
                    <div class="form-top">
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
                    <div class="form-group col-12">
                        <label for="message"></label>
                        <textarea  
                                class="form-input form-control" 
                                rows="7"
                                type="text" 
                                name="message" 
                                id="message"
                                placeholder="How can I help you?" 
                                required
                        ></textarea>
                        <div>
                            <button class="btn btn-outline-light button-submit" type="submit" value="Send">
                                Send
                            </button> 
                            
                            <p class="linkedin">Or <a  href="https://www.linkedin.com/in/chris-kieran" target="_blank">message me on <span class="underline">LinkedIn </span></a></p>
                            
                        </div>
                    </div>    
                    </form>
                </div>
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
form {
    width: 350px;
}
.content-container {
    padding-top: 0;
    padding-left: 40px;
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
}
.img-contact {
    background-image: url('~/assets/images/keyboard.png');
    background-size: cover;
    height: $imgHeight;
    background-position-x: 140px;
}
.title-container {
    text-align: right;
    position: $imgContainerPosition;
    bottom: 228px;
    right: 10px;
    width: 100%;
}
.form-group {
    margin-bottom: 0;
    padding: 0;
}
.btn-outline-light {
    margin-top: 20px;
}
.linkedin {
    margin-top: 20px;
}
.linkedin a {
    text-decoration: none;
    color: white;
}
.underline {
    text-decoration: underline;
}
</style>