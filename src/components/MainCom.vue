<template>
<v-container class="pt-15">
    <v-row>
        <v-col lg="6">
            <h2 class="into_text">Welcome to our  vuetify design</h2>
            <p class="descrip" >
                In Informatics, dummy data is benign information that does not contain
                any useful data, but serves to reserve space where real data is
                nominally present. ... For testing, dummy data can also be used as
                stubs or pad to avoid software testing issues by ensuring that all
                variables and data fields are occupied.
            </p>
            <v-btn color="success" class="white--text" rounded >Get Started</v-btn>
            <v-btn class="white--text ml-5" rounded color="indigo">
                <v-icon >
                   mdi-play-circle
                </v-icon>
                watch vide
            </v-btn>
        </v-col>
        <v-col lg="6" > 
            <img src="./../assets/hero-img.png" height="600px" alt="">
        </v-col>
    </v-row>
</v-container>
</template>
<style scoped>
h2.into_text {
    font-family: cursive;
    font-size: 60px;
    font-weight: bold;
    line-height: initial;
    color: #444;
}
p.descrip {
    font-size: 19px;
    margin: 32PX 0PX;
    font-family: cursive;
    color: #444;
}
</style>