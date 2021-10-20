<template>
  <div>
    <!-- Remove this component to get started! -->
    <NuxtWelcome />
  </div>
</template>

<script>
export default {
  setup() {
    onMounted(() => {
      // I want to get process.env here ...
      console.log('I cat get process.env here ...')
      // I can get process.env. But I don't know how to add variables in process.env
      console.log(process.env)
      // Like this
      console.log(process.env.variables)

      /*
       *  But I want to add other variables in process.env
       *  Like process.env.Base_URL or process.env.TIMEOUT etc..
       *  Because I have some sdks require process.env.variables
       *  
       *  If I use process.env with 'const config = useRuntimeConfig() ' , I must edit my sdks code
       *  But I can't
       */

    })
  },
}
</script>
