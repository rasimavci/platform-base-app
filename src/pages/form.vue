<template>
  <f7-page>
    <f7-navbar title="Üyelik Formu" back-link="back"></f7-navbar>
    <f7-block-title>Üye Ol</f7-block-title>
    <f7-list form>
      <f7-list-item>
        <f7-label>Name</f7-label>
        <f7-input type="text" placeholder="Name"></f7-input>
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
        <f7-label>Password</f7-label>
        <f7-input type="password" placeholder="Password"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Phone</f7-label>
        <f7-input type="tel" placeholder="Phone"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Gender</f7-label>
        <f7-input type="select">
          <option selected>Male</option>
          <option>Female</option>
        </f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Birtday</f7-label>
        <f7-input type="date" placeholder="Birth date" value="2014-04-30"></f7-input>
      </f7-list-item>
      <f7-list-item title="Feeback">
        <f7-toggle slot="after"></f7-toggle>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Slider</f7-label>
        <f7-input>
          <f7-range min="0" max="10" value="50" step="1" :label="true"></f7-range>
        </f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Biography</f7-label>
        <f7-input type="Kısa biyografiniz." placeholder="Bio"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Üyelik şartları</f7-label>
        <f7-input type="Üyelik Şartları" placeholder="Bio" resizable></f7-input>
      </f7-list-item>
    </f7-list>


    <f7-block-title>Registration</f7-block-title>
    <f7-block strong>
      <f7-row tag="p">
        <f7-button class="col" round fill>Register Now</f7-button>
      </f7-row>
    </f7-block>
  </f7-page>
</template>

<script>
export default {}
</script>
