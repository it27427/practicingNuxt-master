<template>
  <client-only>
    <footer class="footer">
      <div class="footer-content">
        <div class="container p-0">
          <div class="row">
            <div class="col-md-4 col-12">
              <div class="footerlogo">
                <img src="~/static/assets/images/logo/logo.png" alt="footer-logo">
              </div>
            </div>

            <div class="col-md-4 col-12">
              <div class="footerinfo footeraboutinfo">
                <div class="footerinfo-header">
                  <h4 class="footerinfo-title">About</h4>
                </div>

                <div class="footerinfo-body">
                  <ul class="footerlist">
                      <li class="footerlist-item">
                        <a href="case-study.html" class="footerlist-link">Doctors</a>
                      </li>

                      <li class="footerlist-item">
                        <a href="contact.html" class="footerlist-link">Hospital</a>
                      </li>

                      <li class="footerlist-item">
                        <a href="products.html" class="footerlist-link">Blog</a>
                      </li>
                  </ul>
                </div>
              </div>
            </div>

            <div class="col-md-4 col-12">
              <div class="footerinfo">
                <div class="footerinfo-header">
                  <h4 class="footerinfo-title">Follow us</h4>
                </div>

                <div class="footerinfo-body">
                  <ul class="social-list">
                    <li class="social-list-item">
                      <VueCustomTooltip label="Follow us on Facebook">
                        <a href="#" target="_blank" class="social-list-link">
                          <svg width="40" height="41" viewBox="0 0 40 41" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <circle cx="20" cy="20.8423" r="20" fill="white"/>
                            <path d="M21.7416 30.8422V21.7192H24.8038L25.2623 18.1639H21.7416V15.8939C21.7416 14.8645 22.0275 14.163 23.5037 14.163L25.3864 14.1621V10.9822C25.0606 10.9391 23.9431 10.8423 22.643 10.8423C19.9285 10.8423 18.0701 12.4991 18.0701 15.5419V18.164H15V21.7193H18.07V30.8423L21.7416 30.8422Z" fill="#4267B2"/>
                          </svg>
                        </a>
                      </VueCustomTooltip>
                    </li>

                    <li class="social-list-item">
                      <VueCustomTooltip label="Follow us on Twitter">
                        <a href="#" target="_blank" class="social-list-link">
                          <svg width="40" height="41" viewBox="0 0 40 41" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <rect y="0.842285" width="40" height="40" rx="20" fill="white"/>
                            <path d="M27.9843 16.8999C27.9843 17.0831 27.9843 17.2664 27.9843 17.4234C27.9843 22.8423 23.8482 29.0988 16.3089 29.0988C13.9791 29.0988 11.8325 28.4182 10 27.2664C10.3141 27.2925 10.6545 27.3187 10.9686 27.3187C12.8796 27.3187 14.6597 26.6643 16.0733 25.5648C14.267 25.5386 12.7487 24.3344 12.2513 22.7114C12.5131 22.7638 12.7487 22.7899 13.0366 22.7899C13.4031 22.7899 13.7696 22.7376 14.1099 22.6329C12.2251 22.2664 10.8115 20.6172 10.8115 18.6276C10.8115 18.6014 10.8115 18.6014 10.8115 18.5753C11.3613 18.8894 11.9895 19.0727 12.6702 19.0988C11.5707 18.3658 10.8377 17.1093 10.8377 15.6695C10.8377 14.9103 11.0471 14.2035 11.3874 13.6014C13.4031 16.0884 16.4398 17.7114 19.8429 17.8946C19.7644 17.6067 19.7382 17.2664 19.7382 16.9522C19.7382 14.6747 21.5707 12.8423 23.8482 12.8423C25.0262 12.8423 26.0995 13.3397 26.8325 14.125C27.7749 13.9418 28.6387 13.6014 29.4503 13.1302C29.1361 14.0988 28.4817 14.8842 27.644 15.4077C28.4817 15.303 29.267 15.0936 30 14.7533C29.4764 15.591 28.7958 16.324 27.9843 16.8999Z" fill="#1DA1F2"/>
                          </svg>
                        </a>
                      </VueCustomTooltip>
                    </li>

                    <li class="social-list-item">
                      <VueCustomTooltip label="Follow us on Youtube">
                        <a href="#" target="_blank" class="social-list-link">
                          <svg width="40" height="41" viewBox="0 0 40 41" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <circle cx="20" cy="20.8423" r="20" fill="white"/>
                            <path fill-rule="evenodd" clip-rule="evenodd" d="M28.6078 13.6118C29.5502 13.8655 30.2932 14.6085 30.5469 15.5508C31.018 17.2724 30.9999 20.8605 30.9999 20.8605C30.9999 20.8605 30.9999 24.4305 30.5469 26.1521C30.2932 27.0944 29.5502 27.8374 28.6078 28.0911C26.8862 28.5442 20 28.5442 20 28.5442C20 28.5442 13.1318 28.5442 11.3921 28.073C10.4497 27.8193 9.70675 27.0763 9.45305 26.134C9 24.4305 9 20.8424 9 20.8424C9 20.8424 9 17.2724 9.45305 15.5508C9.70675 14.6085 10.4679 13.8474 11.3921 13.5937C13.1137 13.1406 20 13.1406 20 13.1406C20 13.1406 26.8862 13.1406 28.6078 13.6118ZM23.5338 20.8426L17.8073 24.1408V17.5445L23.5338 20.8426Z" fill="#FF0000"/>
                          </svg>
                        </a>
                      </VueCustomTooltip>
                    </li>

                    <li class="social-list-item">
                      <VueCustomTooltip label="Follow us on Linkedin">
                        <a href="#" target="_blank" class="social-list-link">
                          <svg width="40" height="41" viewBox="0 0 40 41" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <rect y="0.842285" width="40" height="40" rx="20" fill="white"/>
                            <path d="M29.6798 29.3963C28.458 29.3672 27.2652 29.3672 26.0433 29.3963C25.7815 29.3963 25.7233 29.3381 25.7233 29.0763C25.7233 26.9235 25.7233 24.7416 25.7233 22.5888C25.7233 22.0942 25.6942 21.5997 25.5488 21.1342C25.1124 19.6214 23.3669 19.0687 22.1159 20.0869C21.4468 20.6106 21.185 21.3379 21.185 22.2106C21.185 24.247 21.185 26.2835 21.185 28.3199C21.185 28.5817 21.1559 28.8436 21.185 29.1345C21.2141 29.3672 21.0977 29.4254 20.8941 29.3963C19.6431 29.3963 18.4213 29.3963 17.1703 29.3963C16.9376 29.3963 16.8794 29.3381 16.8794 29.1054C16.9085 27.2726 16.9085 25.4398 16.9085 23.5779C16.9085 21.3088 16.9085 19.0396 16.8794 16.7995C16.8794 16.5377 16.9376 16.4795 17.1703 16.4795C18.4213 16.4795 19.6431 16.4795 20.8941 16.4795C21.1268 16.4795 21.185 16.5377 21.185 16.7704C21.185 17.2359 21.185 17.7014 21.185 18.2541C21.2723 18.1668 21.3014 18.1378 21.3304 18.1087C22.465 16.4504 24.0651 15.985 25.9561 16.2759C28.1379 16.625 29.5343 18.1378 29.8835 20.4651C29.9707 21.0178 29.9998 21.5706 29.9998 22.1233C29.9998 24.4507 29.9998 26.7489 29.9998 29.0763C29.9998 29.309 29.9416 29.3963 29.6798 29.3963Z" fill="#0077B5"/>
                            <path d="M14.5524 22.9379C14.5524 24.9743 14.5524 27.0107 14.5524 29.0472C14.5524 29.309 14.4942 29.3963 14.2324 29.3963C13.0105 29.3672 11.7887 29.3963 10.5668 29.3963C10.3341 29.3963 10.2759 29.3381 10.2759 29.1054C10.2759 25.0034 10.2759 20.8724 10.2759 16.7704C10.2759 16.5668 10.3341 16.4795 10.5668 16.4795C11.8177 16.4795 13.0687 16.4795 14.3196 16.4795C14.5815 16.4795 14.6106 16.5668 14.6106 16.7995C14.5524 18.8359 14.5524 20.8724 14.5524 22.9379Z" fill="#0077B5"/>
                            <path d="M14.7559 13.1048C14.465 14.2685 13.2722 14.9376 11.9049 14.7049C10.4503 14.4721 9.6357 13.0466 10.1594 11.6502C10.5085 10.7775 11.3521 10.2538 12.4285 10.2829C14.0577 10.2538 15.1341 11.5629 14.7559 13.1048Z" fill="#0077B5"/>
                          </svg>
                        </a>
                      </VueCustomTooltip>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
        </div>
          
        <div class="divider"></div>

        <div class="container p-0">
          <div class="row g-0 justify-content-center">
            <div class="copyright">
              <p class="copyright-text">
                <span>&copy;</span> 2022 Doctorvaly. All rights reserved.
              </p>
            </div>
          </div>
        </div>
      </div>
    </footer>
  </client-only>
</template>

<script>
import VueCustomTooltip from '@adamdehaven/vue-custom-tooltip';

export default {
  name: 'FooterComponent',
  components: {
    VueCustomTooltip
  }
}
</script>