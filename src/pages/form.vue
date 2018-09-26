<template>
  <f7-page>
    <f7-navbar title="Üyelik Formu" back-link="Geri"></f7-navbar>
    <f7-block-title>Üyelik Formu</f7-block-title>
    <f7-list form>
      <f7-list-item>
        <f7-label>İsim</f7-label>
        <f7-input type="text" placeholder="İsim"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>E-mail</f7-label>
        <f7-input type="email" placeholder="E-mail"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>URL</f7-label>
        <f7-input type="url" placeholder="URL"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Passaport</f7-label>
        <f7-input type="password" placeholder="Pasaport"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Telefon</f7-label>
        <f7-input type="tel" placeholder="Telefon"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Cinsiyet</f7-label>
        <f7-input type="select">
          <option selected>Erkek</option>
          <option>kadın</option>
        </f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Doğum Günü</f7-label>
        <f7-input type="date" placeholder="Birth date" value="2014-04-30"></f7-input>
      </f7-list-item>
      <f7-list-item title="Bildirimler">
        <f7-toggle slot="after"></f7-toggle>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Slider</f7-label>
        <f7-input>
          <f7-range min="0" max="10" value="50" step="1" :label="true"></f7-range>
        </f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Biyografi</f7-label>
        <f7-input type="Kısa biyografiniz." placeholder="Bio"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Üyelik şartları</f7-label>
        <f7-input type="Üyelik Şartları" placeholder="Bio" resizable></f7-input>
      </f7-list-item>
    </f7-list>


    <f7-block-title>Üyelik</f7-block-title>
    <f7-block strong>
      <f7-row tag="p">
        <f7-button class="col" round fill>Şimdi Üyel Ol </f7-button>
      </f7-row>
    </f7-block>
  </f7-page>
</template>

<script>
export default {}
</script>
