<!-- Copyright (C) 2012-2024 Zammad Foundation, https://zammad-foundation.org/ -->

<script setup lang="ts">
import CommonAlert from '#shared/components/CommonAlert/CommonAlert.vue'
import CommonButton from '#desktop/components/CommonButton/CommonButton.vue'
</script>

<template>
  <div class="w-1/2 ltr:ml-2 rtl:mr-2">
    <h2>Buttons</h2>

    <h3>Text only</h3>
    <div class="space-x-3 py-2 flex">
      <CommonButton variant="primary" />
      <CommonButton variant="secondary" />
      <CommonButton variant="tertiary" />
      <CommonButton variant="submit" />
      <CommonButton variant="danger" />
    </div>
    <div class="space-x-3 py-2 flex">
      <CommonButton variant="primary" size="medium" />
      <CommonButton variant="secondary" size="medium" />
      <CommonButton variant="tertiary" size="medium" />
      <CommonButton variant="submit" size="medium" />
      <CommonButton variant="danger" size="medium" />
    </div>
    <div class="space-x-3 py-2 flex">
      <CommonButton variant="primary" size="large" />
      <CommonButton variant="secondary" size="large" />
      <CommonButton variant="tertiary" size="large" />
      <CommonButton variant="submit" size="large" />
      <CommonButton variant="danger" size="large" />
    </div>

    <h3>With icon</h3>
    <div class="space-x-3 py-2 flex">
      <CommonButton variant="primary" prefix-icon="logo-flat" />
      <CommonButton variant="secondary" prefix-icon="logo-flat" />
      <CommonButton variant="tertiary" prefix-icon="logo-flat" />
      <CommonButton variant="submit" prefix-icon="logo-flat" />
      <CommonButton variant="danger" prefix-icon="logo-flat" />
    </div>
    <div class="space-x-3 py-2 flex">
      <CommonButton variant="primary" suffix-icon="logo-flat" />
      <CommonButton variant="secondary" suffix-icon="logo-flat" />
      <CommonButton variant="tertiary" suffix-icon="logo-flat" />
      <CommonButton variant="submit" suffix-icon="logo-flat" />
      <CommonButton variant="danger" suffix-icon="logo-flat" />
    </div>

    <h3>Icon only</h3>
    <div class="space-x-3 py-2 flex items-center">
      <CommonButton variant="primary" icon="logo-flat" />
      <CommonButton variant="secondary" icon="logo-flat" />
      <CommonButton variant="tertiary" icon="logo-flat" />
      <CommonButton variant="submit" icon="logo-flat" />
      <CommonButton variant="danger" icon="logo-flat" />
      <CommonButton variant="primary" icon="logo-flat" size="medium" />
      <CommonButton variant="secondary" icon="logo-flat" size="medium" />
      <CommonButton variant="tertiary" icon="logo-flat" size="medium" />
      <CommonButton variant="submit" icon="logo-flat" size="medium" />
      <CommonButton variant="danger" icon="logo-flat" size="medium" />
      <CommonButton variant="primary" icon="logo-flat" size="large" />
      <CommonButton variant="secondary" icon="logo-flat" size="large" />
      <CommonButton variant="tertiary" icon="logo-flat" size="large" />
      <CommonButton variant="submit" icon="logo-flat" size="large" />
      <CommonButton variant="danger" icon="logo-flat" size="large" />
    </div>

    <h3>Misc</h3>
    <div class="space-y-2 py-2 flex-wrap">
      <CommonButton variant="submit" block>Block button</CommonButton>
      <CommonButton variant="danger" disabled>Disabled button</CommonButton>
    </div>
  </div>

  <div class="w-1/2 ltr:ml-2 rtl:mr-2">
    <h2>Alerts</h2>

    <CommonAlert
      variant="info"
      dismissible
      link="https://youtu.be/U6n2NcJ7rLc"
      link-text="Party 🎉"
      class="mb-2.5"
      >It's Friday!</CommonAlert
    >
    <CommonAlert variant="success" class="mb-2.5"
      >Hooray! Ticket got updated.</CommonAlert
    >
    <CommonAlert variant="warning" class="mb-2.5"
      >Heee! You're typing too fast.</CommonAlert
    >
    <CommonAlert variant="danger" class="mb-2.5"
      >Ooops! You broke it.</CommonAlert
    >
  </div>

  <div class="ltr:ml-2 rtl:mr-2">
    <h2>Labels</h2>
    <CommonLabel size="small" prefix-icon="logo" suffix-icon="logo-flat"
      >Small</CommonLabel
    >

    <br />

    <CommonLabel size="medium" prefix-icon="logo" suffix-icon="logo-flat"
      >Medium</CommonLabel
    >

    <br />

    <CommonLabel size="large" prefix-icon="logo" suffix-icon="logo-flat"
      >Large</CommonLabel
    >

    <br />

    <CommonLabel size="xl" prefix-icon="logo" suffix-icon="logo-flat"
      >Extra large</CommonLabel
    >
  </div>
</template>
