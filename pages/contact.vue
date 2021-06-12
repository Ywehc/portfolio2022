<template>
    <div class="container page-container">
        <div class="row">
            <div class="col-12 col-xl-6 right order-xl-last">
                <div class="title-container">
                    <h1 class="page-h1 d-none d-xl-block">Contact Me</h1>
                    <div class="img-contact img-page-heading"></div>
                </div>
            </div>
            <div class="front col-12 col-xl-6 order-xl-first">
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
                            <p class="linkedin">Or 
                                <a  href="https://www.linkedin.com/in/chris-kieran" target="_blank">send me a message on 
                                    <span class="underline">LinkedIn </span>
                                </a>
                            </p>
                        </div>
                    </div>    
                    </form>
                </div>
                </div>
                
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import '~/assets/scss/_global.scss';

form {
    width: 350px;
}
textarea {
    height: 200px;
}
.content-container {
    padding-top: 0;
    padding-left: 40px;
}
.img-contact {
    background-image: url('~/assets/images/keyboard.png');
    background-position-x: 140px;
}
.title-container {
    bottom: 228px;
}
.form-group {
    margin-bottom: 0;
    padding: 0;
}
.btn-outline-light {
    margin-top: 20px;
}
.linkedin {
    margin-top: 14px;
}
.linkedin a {
    text-decoration: none;
    color: white;
}
.underline {
    text-decoration: underline;
}

@media screen and (max-width: 1200px) {
    .front {
        padding: 0;
    }
    .title-container {
        bottom: 0;
    }
    .img-contact {
        margin: 0;
        background-size: cover;
        background-position-x: center;
    }
    textarea {
        height: 100px;
    }
    .btn-outline-light {
        margin-top: 20px;
    }
    .form-group {
        height: 46px;
    }
}
</style>