<template>
  <div class="alert alert-primary">
    <h2>{{ title }}</h2>
    <p>{{ message }}</p>
    <hr>
    <div class="alert alert-light">
      <h3>Inneer Slot</h3>
      <ol class="list-group test-left">
        <slot />
      </ol>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      title: 'Slot',
      message: 'This is message.'
    }
  }
}
</script>
