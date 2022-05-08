<template>
  <client-only>
    <header class="header">
      <div class="container p-0">
        <nav class="header-nav">
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
              <nuxt-link to="/" class="desktoplist-link">Home</nuxt-link>
            </li>

            <li class="desktoplist-item">
              <nuxt-link to="/doctors" class="desktoplist-link">Doctors</nuxt-link>
            </li>

            <li class="desktoplist-item">
              <nuxt-link to="/hospital" class="desktoplist-link">Hospital</nuxt-link>
            </li>

            <li class="desktoplist-item">
              <nuxt-link to="/blog" class="desktoplist-link">Blog</nuxt-link>
            </li>
          </ul>
          <!-- DESKTOP-LIST END -->
        </nav>
      </div>
    </header>
  </client-only>
</template>

<script>
export default {
  name: 'HeaderComponent'
}
</script>