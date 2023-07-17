<template>
    <div>
        <footer>

<!-- Footer Start-->
<div class="footer-main">
 <div class="footer-area footer-padding">
     <div class="container">
         <div class="row  justify-content-between">
             <div class="col-lg-3 col-md-4 col-sm-8">
                  <div class="single-footer-caption mb-30">
                       <!-- logo -->
                      <div class="footer-logo">
                          <a href="index.html"><img src="../../public/img/logo/logo2_footer.png" alt=""></a>
                      </div>
                      <div class="footer-tittle">
                          <div class="footer-pera">
                              <p class="info1">Lorem ipsum dolor sit amet, consectetur adipisicing elit sed do eiusmod tempor incididunt ut labore.</p>
                         </div>
                      </div>
                  </div>
             </div>
             <div class="col-lg-2 col-md-4 col-sm-5">
                 <div class="single-footer-caption mb-50">
                     <div class="footer-tittle">
                         <h4>Quick Links</h4>
                         <ul>
                             <li><a href="#">About</a></li>
                             <li><a href="#">Features</a></li>
                             <li><a href="#">Pricing</a></li>
                             <li><a href="#">Download</a></li>
                             <li><a href="#">Reviews</a></li>
                         </ul>
                     </div>
                 </div>
             </div>
             <div class="col-lg-2 col-md-4 col-sm-7">
                 <div class="single-footer-caption mb-50">
                     <div class="footer-tittle">
                         <h4>Support</h4>
                         <ul>
                             <li><a href="#">Report a bug</a></li>
                             <li><a href="#">Privacy Policy</a></li>
                             <li><a href="#">Terms & Conditions</a></li>
                             <li><a href="#">Sitemap</a></li>
                             <li><a href="#">FAQs</a></li>
                         </ul>
                     </div>
                 </div>
             </div>
             <div class="col-lg-3 col-md-6 col-sm-8">
                 <div class="single-footer-caption mb-50">
                     <div class="footer-tittle">
                         <h4>Newsletter</h4>
                         <div class="footer-pera footer-pera2">
                          <p>Heaven fruitful doesn't over lesser in days. Appear </p>
                      </div>
                      <!-- Form -->
                      <div class="footer-form">
                          <div id="mc_embed_signup">
                              <form target="_blank" action="https://spondonit.us12.list-manage.com/subscribe/post?u=1462626880ade1ac87bd9c93a&amp;id=92a4423d01" method="get" class="subscribe_form relative mail_part" novalidate="true">
                                  <input type="email" name="EMAIL" id="newsletter-form-email" placeholder=" Email Address " class="placeholder hide-on-focus" onfocus="this.placeholder = ''" onblur="this.placeholder = ' Email Address '">
                                  <div class="form-icon">
                                      <button type="submit" name="submit" id="newsletter-submit" class="email_icon newsletter-submit button-contactForm"><img src="../../public/img/shape/form_icon.png" alt=""></button>
                                  </div>
                                  <div class="mt-10 info"></div>
                              </form>
                          </div>
                      </div>
                     </div>
                 </div>
             </div>
         </div>
         <!-- Copy-Right -->
         <div class="row align-items-center">
             <div class="col-xl-12 ">
                 <div class="footer-copy-right">
                    <p><!-- Link back to Colorlib can't be removed. Template is licensed under CC BY 3.0. -->
Copyright &copy;{{ new Date().getFullYear() }} All rights reserved | This template is made with <i class="ti-heart" aria-hidden="true"></i> by <a href="https://colorlib.com" target="_blank">Colorlib</a>
<!-- Link back to Colorlib can't be removed. Template is licensed under CC BY 3.0. --></p>
                 </div>
             </div>
         </div>
     </div>
 </div>
</div>
<!-- Footer End-->

</footer>
    </div>
</template>
<script setup>

</script>
<style scoped>
    .footer-area .footer-logo {
    margin-bottom: 30px;
}
.footer-area .footer-pera .info1 {
    margin-bottom: 10px;
    line-height: 1.8;
}
.footer-area .footer-pera .info2 {
    margin-bottom: 50px;
    line-height: 1.8;
}
.footer-area .footer-pera.footer-pera2 p {
    padding: 0;
}
.footer-area .footer-tittle h4 {
    color: #000;
    font-size: 18px;
    margin-bottom: 48px;
    font-weight: 700;
}
.footer-area .footer-tittle ul li {
    color: #012f5f;
    margin-bottom: 15px;
}
.footer-area .footer-tittle ul li a {
    color: #868c98;
    font-weight: 300;
    text-decoration: none;
}
.footer-area .footer-tittle ul li a:hover {
    color: #8f1bdc;
    padding-left: 5px;
}
.footer-area .footer-form {
    margin-top: 40px;
}
.footer-area .footer-form form {
    position: relative;
}
.footer-area .footer-form form input {
    width: 100%;
    height: 43px;
    padding: 10px 20px;
    border: 1px solid #fff;
    background: #f9f9fe;
}
.footer-area .footer-form form .form-icon button {
    position: absolute;
    top: 1px;
    right: 0;
    background: none;
    border: 0;
    cursor: pointer;
    padding: 11px 22px;
    background: #8f1bdc;
    line-height: 1;
}
.footer-area .info.error {
    color: #8f1bdc;
}
.footer-area .footer-social a {
    width: 40px;
    height: 40px;
    font-size: 14px;
    border: 1px solid #fafafa;
    background: #fafafa;
    display: inline-block;
    line-height: 40px;
    text-align: center;
    color: #949eb2;
    margin-right: 5px;
    -webkit-transition: .4s;
    -moz-transition: .4s;
    -o-transition: .4s;
    transition: .4s;
}
.footer-area .footer-copy-right {
    padding-top: 20px;
}
@media (max-width: 767px) {
    .footer-area .footer-copy-right {
    padding-top: 0px;
}
}.footer-area .footer-copy-right p {
    color: #888888;
    font-weight: 300;
    font-size: 16px;
    line-height: 2;
    margin-bottom: 12px;
}
.footer-area .footer-copy-right p i {
    color: #f9218d;
}
.footer-area .footer-copy-right p a {
    color: #f9218d;
    text-decoration: none;
}
.footer-area .footer-copy-right p a:hover {
    color: #8f1bdc;
}
.footer-social a:hover {
    background: #8f1bdc;
}
.footer-social a:hover i {
    color: #fff;
    -webkit-transition: .4s;
    -moz-transition: .4s;
    -o-transition: .4s;
    transition: .4s;
}
</style>