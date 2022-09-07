<template>
    <div>
          <nav class="navbar navbar-expand-lg navbar-dark bg-dark padding">
  <NuxtLink class="navbar-brand" to="/">BookiFy</NuxtLink>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse ml-auto" id="navbarSupportedContent">
    <ul class="navbar-nav ml-auto">
      <li class="nav-item active">
        <NuxtLink class="nav-link" to="/products">Products <span class="sr-only">(current)</span></NuxtLink>
      </li>
      <li class="nav-item">
        <NuxtLink class="nav-link" to="/my-items">MyItems</NuxtLink>
      </li>
    </ul>
  </div>
</nav>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
 .padding {
        padding: 0.6rem;
        background-color: black
    }
    .nav-left {
        margin-left: auto;
    }
</style>