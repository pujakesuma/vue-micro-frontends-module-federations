<template>
  <div>
      <header class="header">
        <h2> App Header</h2>
          <p>items: {{cartCount}}</p>
      </header>
  </div>
</template>

<script>
export default {
    computed: {
        cartCount() {
            return this.$store.state.cartItems
        }
    },
}
</script>

<style>
.header {
  background-color: darkcyan;
  color: #fff;
  width: 100%;
  text-align: center;
  font-size: 24px;
  font-weight: 700;
  padding: 1rem 0;
}
</style>