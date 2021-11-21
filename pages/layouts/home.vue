<template>
  <div id="index">
    <Navbar> </Navbar>
     <div v-if="$nuxt.isOffline">
      </div>
      <div v-else>
        <nuxt />
      </div>
    <Footer />
  </div>
</template>