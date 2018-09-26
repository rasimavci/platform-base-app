<template>
  <f7-page>
    <f7-navbar title="Sol menü"></f7-navbar>
    <f7-block strong>
      <p>Sol menü içeriği</p>
    </f7-block>
    <f7-block-title>Load page in panel</f7-block-title>
    <f7-list>
      <f7-list-item link="/about/" title="Hakkımızda"></f7-list-item>
      <f7-list-item link="/form/" title="Başvuru"></f7-list-item>
    </f7-list>
    <f7-block-title>Load page in main view</f7-block-title>
    <f7-list>
      <f7-list-item link="/about/" title="Hakkımızda" view="#main-view" panel-close></f7-list-item>
      <f7-list-item link="/form/" title="Başvuru" view="#main-view" panel-close></f7-list-item>
    </f7-list>
  </f7-page>
</template>
<script>
export default {}
</script>
