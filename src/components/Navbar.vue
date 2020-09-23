<template>
    <nav>
        <v-app-bar color="white" dark app class="line">
            <v-toolbar-title class="text-uppercase red--text">
                <span class="font-weight-light">Sors</span>
                <span>Inventario</span>
            </v-toolbar-title>
            <template>
                <v-btn color="red" dark small absolute bottom right fab>
                    <v-icon>mdi-plus</v-icon>
                </v-btn>
            </template>
        </v-app-bar>

        <v-navigation-drawer v-model="darwer" dark app mini-variant class="red">
            <v-list flat>
                <v-list-item class="mb-12">
                       <v-list-item-action>
                           <v-icon>fas fa-cloud-download-alt</v-icon>
                       </v-list-item-action>
                </v-list-item>
                <v-list-item router to="/">
                    <v-list-item-action>
                        <v-icon>fas fa-desktop</v-icon>
                    </v-list-item-action>
                </v-list-item>
                <v-list-item router to="/">
                    <v-list-item-action>
                        <v-badge color="green">
                            <template v-slot:badge>1</template>
                            <v-icon>fas fa-shopping-cart</v-icon>
                        </v-badge>
                    </v-list-item-action>
                </v-list-item>
                <v-list-item router to="/">
                    <v-list-item-action>
                        <v-icon>fas fa-city</v-icon>
                    </v-list-item-action>
                </v-list-item>
                <v-list-item router to="/">
                    <v-list-item-action>
                        <v-icon>fas fa-cog</v-icon>
                    </v-list-item-action>
                </v-list-item>
                 
            </v-list>
            
        </v-navigation-drawer>

    </nav>
</template>
<script>
export default {
    data: () => ({
        darawer: true
    })
}
</script>