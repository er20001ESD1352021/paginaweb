<template>
   <div class="text-h5 text-center">Mis Conocimientos</div>
        <div class="q-pa-md row items-start q-gutter-md">
      <q-card class="my-card text-center">
        <img src="https://dev.java/assets/images/java-logo-vert-blk.png">
  
        <q-card-section>
          <div class="text-h6">JAVA</div>
        </q-card-section>
      </q-card>

      <q-card class="my-card text-center">
        <img src="data:image/jpeg;base64,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">
  
        <q-card-section>
          <div class="text-h6">PHP</div>
        </q-card-section>
      </q-card>

      <q-card class="my-card text-center">
        <img src="https://tublitzed.com/img/portfolio/node/browser/full/1.jpg">
  
        <q-card-section>
          <div class="text-h6">NODE</div>
        </q-card-section>
      </q-card>

      <q-card class="my-card text-center">
        <img src="https://www.logolynx.com/images/logolynx/db/db9a81493e7931d9a006990890b70057.jpeg">
  
        <q-card-section>
          <div class="text-h6">VUE</div>
        </q-card-section>
      </q-card>

        <q-card class="my-card text-center">
        <img src="https://play-lh.googleusercontent.com/RslBy1o2NEBYUdRjQtUqLbN-ZM2hpks1mHPMiHMrpAuLqxeBPcFSAjo65nQHbTA53YYn">
  
        <q-card-section>
          <div class="text-h6">HTML</div>
        </q-card-section>
      </q-card>

    </div>
</template>
  
  <script>
  import { defineComponent } from 'vue'
  
  export default defineComponent({
    name: 'IndexPage'
  })
  </script>

<style lang="scss" scoped>
.my-card{

    max-width: 210px;
}
</style>