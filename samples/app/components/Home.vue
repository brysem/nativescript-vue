<template>
  <Page>
    <ActionBar class="action-bar" title="Home Page">
    </ActionBar>
    <StackLayout>
      <Button text="Open page" @tap="openPage" />
      <Label class="text-center">Click the button above to go to the next page.</Label>
    </StackLayout>
  </Page>
</template>

<script>
import Details from './Details'

export default {
  components: [
    Details,
  ],
  methods: {
    openPage() {
      this.$navigateTo(Details)
    }
  }
}
</script>

<style>
  Button {
    background-color: #222;
    color: #FFF;
  }

  .text-center {
    text-align: center;
    color: #FF0000;
  }
</style>
