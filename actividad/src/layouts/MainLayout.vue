<template>
 <q-layout view="lHh Lpr lff" >
      <q-header elevated class="bg-warning">
        
        <q-toolbar>
          <q-toolbar-title>DISEÑO DE SISTEMAS 1</q-toolbar-title>
          <q-btn flat @click="drawer = !drawer" round dense icon="menu" />
        </q-toolbar>
      </q-header>

      <q-drawer
        v-model="drawer"
        show-if-above
        :width="200"
        :breakpoint="400"
      >
        <q-scroll-area style="height: calc(100% - 150px); margin-top: 150px; border-right: 1px solid #ddd">
          <q-list padding>
            <q-item clickable v-ripple to="/" active-class="my-menu-link" exact>
              <q-item-section avatar>
                <q-icon name="style" />
              </q-item-section>

              <q-item-section>
                Mi Proyecto
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple to="/conocimientos" active-class="my-menu-link">
              <q-item-section avatar>
                <q-icon name="today" />
              </q-item-section>

              <q-item-section>
                Mis Conocimientos
              </q-item-section>
            </q-item>

          </q-list>
        </q-scroll-area>

        <q-img class="absolute-top" src="https://images.unsplash.com/photo-1563118130-00d965c3a559?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1yZWxhdGVkfDEzfHx8ZW58MHx8fHw%3D&w=1000&q=80" style="height: 150px">
          <div class="absolute-bottom bg-transparent">
            <q-avatar size="56px" class="q-mb-sm">
              <img src="https://png.pngtree.com/png-vector/20190321/ourlarge/pngtree-vector-users-icon-png-image_856952.jpg">
            </q-avatar>
            <div class="text-weight-bold">Oscar Alexander Escalante Rajo</div>
            <div>er20001@ues.edu.sv</div>
          </div>
        </q-img>
      </q-drawer>

      <q-page-container>
        <router-view></router-view>
      </q-page-container>
    </q-layout>

    <q-layout view="hHh lpR lFf">

<q-page-container>
  <router-view />
</q-page-container>

<q-footer reveal elevated class="bg-warning text-black text-center">
  <q-toolbar>
    <q-toolbar-title>
      <div>PREGUNTAS FRECUENTES</div>
      <div>CONTACTANOS</div>
      <div>ER20001@UES.EDU.SV</div>
    </q-toolbar-title>
  </q-toolbar>
</q-footer>

</q-layout>


</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    const drawer = ref(false)

    return {
      drawer
    }
  }
}
</script>

<style lang="scss">
.my-menu-link{
  color: white;
  background: #F2C037;
}
</style>

<style lang="scss">
.footer{
  color: white;
  background: #F2C037;
  text-align: center;
}
</style>