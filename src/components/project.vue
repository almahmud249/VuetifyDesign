<template>
<v-container class="">
    <v-row>
        <v-col lg="12" class="text-center">
            <v-subheader class="text-h4 justify-center">Project</v-subheader>
            <p>
                stubs or pad to avoid software testing issues by ensuring that all
                variables and data fields are occupied.
            </p>
        </v-col>
        <v-col v-for="project in 3" :key="project">
            <v-card class="mx-auto" max-width="344">
                <v-img src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" height="200px"></v-img>

                <v-card-title> Top western road trips </v-card-title>

                <v-card-subtitle> 1,000 miles of wonder </v-card-subtitle>
                <v-divider class="mx-4"></v-divider>
                <v-card-actions>
                    <v-btn color="success">View Details</v-btn>
                    <v-spacer></v-spacer>
                    <v-rating background-color="red" color="amber" size="14" half-increments dense :value="4.5"></v-rating>
                </v-card-actions>
            </v-card>
        </v-col>
    </v-row>
</v-container>
</template>
<script>
export default {
    name:'project'
}
</script>
