<template>
  <v-app :style="{background: $vuetify.theme.themes.light.backogruns} ">
    <v-container>
      <v-row>
        <v-col cols="12" md="4">
          <v-text-field label="Buscar items" prepend-icon="search" color="red" error></v-text-field>
        </v-col>
        <v-spacer></v-spacer>
        <span class="red--text mt-9"> 19 Items</span>
        <v-btn text class="mt-7">
          <v-icon color="red" class="mr-n10">menu</v-icon>
        </v-btn>
        <v-btn text class="mt-7">
          <v-icon color="red" class="mr-n10">dashboard</v-icon>
        </v-btn>
      </v-row>

      <v-row>

        <v-col cols="12" md="3" class="mb-4">
          <v-hover v-slot:default="{ hover }">
            <v-card max-width="250" max-height="250" align="center">
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn icon><v-icon>edit</v-icon></v-btn>
              </v-card-actions>
              <v-img src="1.png" width="150" height="150"></v-img>
              <v-card-text class="red--text">Air Max Hyper Agressor</v-card-text>
              <v-expand-transition>
                <div v-if="hover" class="d-flex transition-fast-in-fast-out red v-card--reveal display-3 white--text" style="height:100%">
                  <v-btn outlined="" color="white">Detalles</v-btn>
                </div>
              </v-expand-transition>
              <v-btn absolute="" color="red" class="white--text" fab large left top>
                <h1>1</h1>
              </v-btn>
            </v-card>
          </v-hover>
        </v-col>


        <v-col cols="12" md="3" class="mb-4">
          <v-hover v-slot:default="{ hover }">
            <v-card max-width="250" max-height="250" align="center">
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn icon><v-icon>edit</v-icon></v-btn>
              </v-card-actions>
              <v-img src="4.png" width="150" height="150"></v-img>
              <v-card-text class="red--text">Air Max Hyper Agressor</v-card-text>
              <v-expand-transition>
                <div v-if="hover" class="d-flex transition-fast-in-fast-out red v-card--reveal display-3 white--text" style="height:100%">
                  <v-btn outlined="" color="white">Detalles</v-btn>
                </div>
              </v-expand-transition>
              <v-btn absolute="" color="red" class="white--text" fab large left top>
                <h1>1</h1>
              </v-btn>
            </v-card>
          </v-hover>
        </v-col>

        <v-col cols="12" md="3" class="mb-4">
          <v-hover v-slot:default="{ hover }">
            <v-card max-width="250" max-height="250" align="center">
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn icon><v-icon>edit</v-icon></v-btn>
              </v-card-actions>
              <v-img src="3.png" width="150" height="150"></v-img>
              <v-card-text class="red--text">Air Max Hyper Agressor</v-card-text>
              <v-expand-transition>
                <div v-if="hover" class="d-flex transition-fast-in-fast-out red v-card--reveal display-3 white--text" style="height:100%">
                  <v-btn outlined="" color="white">Detalles</v-btn>
                </div>
              </v-expand-transition>
              <v-btn absolute="" color="red" class="white--text" fab large left top>
                <h1>3</h1>
              </v-btn>
            </v-card>
          </v-hover>
        </v-col>

        <v-col cols="12" md="3" class="mb-4">
          <v-hover v-slot:default="{ hover }">
            <v-card max-width="250" max-height="250" align="center">
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn icon><v-icon>edit</v-icon></v-btn>
              </v-card-actions>
              <v-img src="2.png" width="150" height="150"></v-img>
              <v-card-text class="red--text">Air Max Hyper Agressor</v-card-text>
              <v-expand-transition>
                <div v-if="hover" class="d-flex transition-fast-in-fast-out red v-card--reveal display-3 white--text" style="height:100%">
                  <v-btn outlined="" color="white">Detalles</v-btn>
                </div>
              </v-expand-transition>
              <v-btn absolute="" color="red" class="white--text" fab large left top>
                <h1>4</h1>
              </v-btn>
            </v-card>
          </v-hover>
        </v-col>

      </v-row>
    </v-container>
  </v-app>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
    
  },
  computed:{
    theme() {
      return (this.$vuetify.theme.dark) ? 'dark' : 'light'
    }
  }
  
}
</script>
<style>
  .v-card--reveal{
    align-items: center;
    bottom: 0;
    justify-content: center;
    opacity: .5;
    position: absolute;
    width: 100%;
  }
</style>