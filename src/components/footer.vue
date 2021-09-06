<template>
<v-footer padless dark>
    <v-col lg="12">
        <v-row justify="center">
            <v-col lg="4" class="text-center">
                <v-toolbar-title class="toolbar_title">Vuetify App</v-toolbar-title>
                <v-card-text>
                    <v-btn v-for="icon in icons" :key="icon" class="mx-4 white--text" icon>
                        <v-icon size="24px">
                            {{ icon }}
                        </v-icon>
                    </v-btn>
                </v-card-text>
                <v-subheader>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate
                    eligendi minus officia ratione maxime, obcaecati ad doloremque rerum
                    inventore placeat!</v-subheader>
            </v-col>
        </v-row>
    </v-col>

 

    <v-divider></v-divider>

    <v-card-text class="white--text">
        {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
    </v-card-text>
</v-footer>
</template>

<script>
export default {
    data: () => ({
        icons: ["mdi-facebook", "mdi-twitter", "mdi-linkedin", "mdi-instagram"],
    }),
};
</script>
