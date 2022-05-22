<template>
  <client-only>
    <header class="header">
      <div class="container p-0">
        <nav class="header-nav">
          <!-- HAMBURGER BUTTON START -->
          <div class="hamburger">
            <button class="btn-hamburger" type="button" data-bs-toggle="offcanvas" data-bs-target="#mobileMenu" aria-controls="mobileMenu">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M4 18H20M4 6H20H4ZM4 12H12H4Z" stroke="#A0AEC0" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </button>

            <MobileMenu/>
          </div>
          <!--- HAMBURGER BUTTON END --->

          <!-- SITE-LOGO START -->
          <div class="sitelogo">
            <nuxt-link to="/" class="logo">
              <img src="~/static/assets/images/logo/logo.png" alt="logo">
            </nuxt-link>
          </div>
          <!-- SITE-LOGO END -->

          <!-- DESKTOP-SEARCH START -->
          <div class="desktopsearch">
            <input type="search" class="searchfield" placeholder="What are you looking for?">
            <button type="submit" class="btn-search">
              <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-search" viewBox="0 0 16 16">
                <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"/>
              </svg>
            </button>

            <!-- DESKTOP-SEARCH SUGGESTIONS START -->
            <div class="desktopsearch-result">

            </div>
            <!-- DESKTOP-SEARCH SUGGESTIONS END ---->
          </div>
          <!-- DESKTOP-SEARCH END -->

          <!-- DESKTOP-LIST START -->
          <ul class="desktoplist">
            <li class="desktoplist-item">
              <nuxt-link to="/blog" class="desktoplist-link">Blog</nuxt-link>
            </li>

            <li class="desktoplist-item">
              <nuxt-link to="/contact" class="desktoplist-link">Contact</nuxt-link>
            </li>

            <li class="desktoplist-item">
              <nuxt-link to="/doctors" class="desktoplist-link">Doctors</nuxt-link>
            </li>
          </ul>
          <!-- DESKTOP-LIST END -->

          <!-- MOBILE-SEARCH START -->
          <div class="mobilesearch">
            <button class="btn-mobsearch">
              <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-search" viewBox="0 0 16 16">
                <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"/>
              </svg>
            </button>
          </div>
          <!--- MOBILE-SEARCH END --->
        </nav>
      </div>
    </header>
  </client-only>
</template>

<script>
import gsap from 'gsap';
import { ScrollTrigger } from 'gsap/dist/ScrollTrigger';
import MobileMenu from '~/components/MobileMenu/MobileMenu';

// REGISTER SCROLL-TRIGGER
gsap.registerPlugin(ScrollTrigger);

export default {
  name: 'HeaderComponent',
  components: {
    MobileMenu
  },
  mounted() {
    this.$nextTick(() => {
      this.headerScroll();
    });
  },
  methods: {
    headerScroll() {
      const showAnim = gsap.from('.header', {
        yPercent: -100,
        paused: true,
        duration: 0.2
      }).progress(1);

      ScrollTrigger.create({
        start: "top top",
        end: 99999,
        onUpdate: (self) => {
          self.direction === -1 ? showAnim.play() : showAnim.reverse();
        }
      });
    }
  }
}
</script>