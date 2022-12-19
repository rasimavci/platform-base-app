<template lang='pug'>
  f7-app(:params="f7params")
    f7-statusbar
    // Left panel with reveal effect when hidden
    .panel.panel-left.panel-reveal
      .view.view-left
        .page
          .navbar
            .navbar-inner.sliding
              .title AnaPlatform
          .page-content
            .block-title Main Screen Settings
            .list.links-list
              ul
                li
                  a.panel-close(href="/about/" data-view=".view-main") Hakkında
                li
                  a.panel-close(href="/form/" data-view=".view-main") Üyel Ol
                li
                  a.back(href="#" data-view=".view-main") Geri
    // Right panel with cover effect
    .panel.panel-right.panel-cover.theme-dark
      .view
        .page
          .navbar
            .navbar-inner
              .title right menu
          .page-content
            .block right menu content
    f7-view(id="main-view" url="/" main)
</template>

<script>
// Import Routes
import routes from './routes.js'

export default {
  data() {
    return {
      // Framework7 parameters here
      f7params: {
        id: 'io.framework7.testapp', // App bundle ID
        name: 'Framework7', // App name
        theme: 'auto', // Automatic theme detection
        // App routes
        routes: routes,
        panel: {
          leftBreakpoint: 768
        },
      }
    }
  }
}
</script>
