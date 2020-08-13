<template>
  <div>
  <v-card color="grey lighten-4" flat height="80px" tile>
    <v-toolbar dense>
      <v-app-bar-nav-icon  @click.stop="drawer = !drawer"></v-app-bar-nav-icon>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>assignment</v-icon>
      </v-btn>

    </v-toolbar>
  </v-card>
   <Entradas></Entradas>
  <v-navigation-drawer class="Navigation"
      v-model="drawer"
      app
    >
      <v-list dense>
        <v-list-item link>
          <v-list-item-action>
            <v-icon>settings</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Ajustes</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link>
          <v-list-item-action>
            <v-icon>mdi-email</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Contacto</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
                <v-list-item link>
          <v-list-item-action>
            <v-icon>credit_card</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Formas de pago</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link>
          <v-list-item-action>
            <v-icon>call</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Telefono</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

      </v-list>
    </v-navigation-drawer>
  <v-footer padless class="footer">
    <v-card class="flex" flat tile>
     <v-bottom-navigation v-model="bottomNav">
      <v-btn value="recent">
        <span>Home</span>
        <v-icon>mdi-home</v-icon>
      </v-btn>
      <v-spacer></v-spacer>
      <v-btn value="favorites">
        <span>Destacados</span>
        <v-icon>local_play</v-icon>
      </v-btn>

      <v-btn value="nearby">
        <span>Buscar</span>
        <v-icon>search</v-icon>
      </v-btn>
     </v-bottom-navigation>
    </v-card>
  </v-footer>
  </div>
</template>
<script>
import Entradas from '@/views/Entradas.vue'
export default {
  data() {
    return {
      bottomNav: 'recent',
      drawer: null,
    }
},
    components: {
      Entradas
    }
}
</script>
<style>
.footer {
  min-height: 100px;
  bottom: 0;
  width: 100%;
  height: 100px;
  position: fixed;
}
.Navigation {
  color: black;
}
</style>
