<template>
  <footer class="footer">
    <div class="footer-content">
      <div class="footerupper">
        <div class="container p-0">
          <div class="row g-4">
            <div class="col-md-3 col-12">
              <div class="footerlogo">
                <img src="~/static/assets/images/logo/logo.png" alt="footer-logo">
              </div>
            </div>

            <div class="col-md-3 col-12">
              <div class="footerinfo footeraboutinfo">
                <div class="footerinfo-header">
                  <h4 class="footerinfo-title">About</h4>
                </div>

                <div class="footerinfo-body">
                  <ul class="footerlist">
                      <li class="footerlist-item">
                        <nuxt-link to="/doctors" class="footerlist-link">Doctors</nuxt-link>
                      </li>

                      <li class="footerlist-item">
                        <nuxt-link to="/hospital" class="footerlist-link">Hospital</nuxt-link>
                      </li>

                      <li class="footerlist-item">
                        <nuxt-link to="/blog" class="footerlist-link">Blog</nuxt-link>
                      </li>
                  </ul>
                </div>
              </div>
            </div>

            <div class="col-md-3 col-12">
              <div class="footerinfo footeraboutinfo">
                <div class="footerinfo-header">
                  <h4 class="footerinfo-title">Links</h4>
                </div>

                <div class="footerinfo-body">
                  <ul class="footerlist">
                      <li class="footerlist-item">
                        <nuxt-link to="/termsofuse" class="footerlist-link">Terms of use</nuxt-link>
                      </li>

                      <li class="footerlist-item">
                        <nuxt-link to="/privacypolicy" class="footerlist-link">Privacy Policy</nuxt-link>
                      </li>

                      <li class="footerlist-item">
                        <nuxt-link to="/contact" class="footerlist-link">Contact</nuxt-link>
                      </li>
                  </ul>
                </div>
              </div>
            </div>

            <div class="col-md-3 col-12">
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
                      <VueCustomTooltip label="Follow us on Instagram">
                        <a href="#" target="_blank" class="social-list-link">
                          <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 40 40" fill="none">
                            <circle cx="20" cy="20" r="20" fill="white"/>
                            <path d="M30.9339 15.4648C30.8803 14.2939 30.6944 13.4943 30.4224 12.7947C30.1463 12.0607 29.7133 11.3958 29.1537 10.8463C28.6043 10.2867 27.9393 9.8535 27.2053 9.57722C26.5056 9.30548 25.7061 9.11967 24.5352 9.06647C23.3621 9.01276 22.9873 9 20 9C17.0127 9 16.6379 9.01276 15.4648 9.06613C14.2939 9.11967 13.4944 9.30565 12.7947 9.57756C12.0607 9.85367 11.3958 10.2867 10.8463 10.8463C10.2867 11.3957 9.8535 12.0605 9.57722 12.7945C9.30548 13.4943 9.11967 14.2939 9.06647 15.4646C9.01276 16.6379 9 17.0125 9 19.9998C9 22.9873 9.01276 23.3621 9.06647 24.5352C9.11984 25.7059 9.30582 26.5056 9.57773 27.2053C9.85384 27.9391 10.2869 28.6042 10.8465 29.1535C11.3958 29.7131 12.0609 30.1462 12.7948 30.4223C13.4944 30.6944 14.2941 30.8802 15.465 30.9337C16.6382 30.9872 17.0128 30.9998 20.0002 30.9998C22.9875 30.9998 23.3623 30.9872 24.5354 30.9337C25.7063 30.8802 26.5057 30.6944 27.2055 30.4223C28.683 29.8509 29.8511 28.6829 30.4224 27.2053C30.6945 26.5056 30.8803 25.7059 30.9339 24.5352C30.9872 23.362 31 22.9873 31 20C31 17.0125 30.9872 16.6379 30.9339 15.4648V15.4648ZM28.9538 24.4451C28.9049 25.5176 28.7257 26.1001 28.5751 26.4876C28.205 27.447 27.4469 28.2052 26.4874 28.5753C26.0999 28.7258 25.5175 28.9051 24.4449 28.9539C23.2853 29.007 22.9373 29.0181 20 29.0181C17.0625 29.0181 16.7147 29.007 15.5549 28.9539C14.4825 28.9051 13.9001 28.7258 13.5124 28.5753C13.0347 28.3989 12.6025 28.1177 12.2477 27.7523C11.8823 27.3975 11.6011 26.9655 11.4247 26.4876C11.2742 26.1001 11.0949 25.5176 11.0461 24.4451C10.9932 23.2853 10.9819 22.9373 10.9819 20.0002C10.9819 17.0629 10.9932 16.7151 11.0461 15.5551C11.0951 14.4825 11.2742 13.9001 11.4247 13.5126C11.6011 13.0347 11.8824 12.6025 12.2477 12.2477C12.6025 11.8823 13.0347 11.6011 13.5126 11.4249C13.9001 11.2742 14.4825 11.0951 15.5551 11.0461C16.7149 10.9932 17.0629 10.9819 20 10.9819H19.9998C22.937 10.9819 23.2849 10.9932 24.4449 11.0462C25.5175 11.0951 26.0997 11.2743 26.4874 11.4249C26.9651 11.6013 27.3973 11.8824 27.7522 12.2477C28.1176 12.6025 28.3987 13.0347 28.575 13.5126C28.7257 13.9001 28.9049 14.4825 28.9538 15.5551C29.0067 16.7149 29.0179 17.0629 29.0179 20C29.0179 22.9373 29.0068 23.2851 28.9538 24.4451Z" fill="url(#instaicon-1)"/>
                            <path d="M20.0001 14.3511C16.8805 14.3511 14.3516 16.8802 14.3516 19.9998C14.3516 23.1194 16.8805 25.6483 20.0001 25.6483C23.1199 25.6483 25.6488 23.1194 25.6488 19.9998C25.6488 16.8802 23.1199 14.3511 20.0001 14.3511V14.3511ZM20.0001 23.6664C17.9752 23.6662 16.3335 22.0247 16.3337 19.9996C16.3337 17.9747 17.9752 16.333 20.0003 16.333C22.0253 16.3332 23.6669 17.9747 23.6669 19.9996C23.6669 22.0247 22.0252 23.6664 20.0001 23.6664V23.6664Z" fill="url(#instaicon-2)"/>
                            <path d="M27.1918 14.1282C27.1918 14.8572 26.6008 15.4482 25.8719 15.4482C25.1427 15.4482 24.5518 14.8572 24.5518 14.1282C24.5518 13.3991 25.1427 12.8081 25.8719 12.8081C26.6008 12.8081 27.1918 13.3991 27.1918 14.1282V14.1282Z" fill="url(#instaicon-3)"/>
                            <defs>
                              <linearGradient id="instaicon-1" x1="10.8462" y1="29.1536" x2="29.1538" y2="10.846" gradientUnits="userSpaceOnUse">
                                <stop stop-color="#FFD600"/>
                                <stop offset="0.5" stop-color="#FF0100"/>
                                <stop offset="1" stop-color="#D800B9"/>
                              </linearGradient>
                              <linearGradient id="instaicon-2" x1="16.006" y1="23.9939" x2="23.9944" y2="16.0055" gradientUnits="userSpaceOnUse">
                                <stop stop-color="#FF6400"/>
                                <stop offset="0.5" stop-color="#FF0100"/>
                                <stop offset="1" stop-color="#FD0056"/>
                              </linearGradient>
                              <linearGradient id="instaicon-3" x1="24.9385" y1="15.0615" x2="26.8052" y2="13.1948" gradientUnits="userSpaceOnUse">
                                <stop stop-color="#F30072"/>
                                <stop offset="1" stop-color="#E50097"/>
                              </linearGradient>
                            </defs>
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
      </div>

      <div class="footerlower">
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
    </div>
  </footer>
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