<template>
<v-container class="my-15">
    <v-row justify="center">
        <v-col lg="12" class="text-center">
            <v-subheader class="text-h4 justify-center">Portfolio</v-subheader>
            <p> stubs or pad to avoid software testing issues by ensuring that all
                variables and data fields are occupied.</p>
        </v-col>
        <v-col lg="12">
            <div class="text-center">
                <v-chip class="mx-3" @click="ActivePortfolio ='WebApp'" :color="ActivePortfolio== 'WebApp'? 'success':''">
                    Web App
                </v-chip>
                <v-chip class="mx-3" @click="ActivePortfolio = 'MobileApp'" :color="ActivePortfolio== 'MobileApp'? 'success':''">
                    Mobile App
                </v-chip>
                <v-chip class="mx-3" @click="ActivePortfolio =  'DesktopApp'" :color="ActivePortfolio== 'DesktopApp'? 'success':''">
                    Desktop App
                </v-chip>

            </div>
        </v-col>
        <slot v-if="ActivePortfolio=='WebApp'">
            <v-col  v-for="app in WebApp" :key="app.title">
                <v-card class="mx-auto" max-width="344">
                    <v-img :src="app.image" height="200px"></v-img>

                </v-card>
            </v-col>
        </slot>
         <slot v-if="ActivePortfolio=='MobileApp'">
            <v-col  v-for="app in MobileApp" :key="app.title">
                <v-card class="mx-auto" max-width="344">
                    <v-img :src="app.image" height="200px"></v-img>

                </v-card>
            </v-col>
        </slot>

    </v-row>
</v-container>
</template>

<script>
export default {
    data() {
        return {
            ActivePortfolio: "WebApp",
            WebApp: [
                    {title:'Web App 1',image:'https://res.cloudinary.com/practicaldev/image/fetch/s--gJHvKBc---/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/1srpidiu14okwwtvwkhn.png'},
                    {title:'Web App 2',image:'https://p.kindpng.com/picc/s/127-1272110_web-application-transparent-hd-png-download.png'},
                    {title:'Web App 3',image:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcScWhy9sXTSwakJHgk-sEU3_6lDL56PlGzJYezAF7oAjVYTiKl4nbZSl31p_nzjoYHvJEc&usqp=CAU'},
                    {title:'Web App 4',image:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRvmof4X00_zX5j8B2Km_Taa6nZy-0YdEx8E0TKE38oObAX7qlOLZDVaXBJdmqrqfNBL2o&usqp=CAU'},
                    {title:'Web App 5',image:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcScWhy9sXTSwakJHgk-sEU3_6lDL56PlGzJYezAF7oAjVYTiKl4nbZSl31p_nzjoYHvJEc&usqp=CAU'},
                    {title:'Web App 6',image:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRW9Q_S3C6j2aSyMesVRlrNrPClSyPmeJNnv8624RPn43-YC_4vu9wyuz8dOKQFFSD8q28&usqp=CAU'},
                    {title:'Web App 7',image:'https://p.kindpng.com/picc/s/127-1272110_web-application-transparent-hd-png-download.png'},
            ],
             MobileApp: [
                {title:'Mobile App 1',image:'https://cdn.dribbble.com/users/1464151/screenshots/11469899/media/4bda5be66067d24cd66fd4c761d9ab9b.png?compress=1&resize=400x300'},
                    {title:'Mobile App 2',image:'https://cdn.dribbble.com/users/1464151/screenshots/11469899/media/4bda5be66067d24cd66fd4c761d9ab9b.png?compress=1&resize=400x300'},
                    {title:'Mobile App 3',image:'https://cdn.dribbble.com/users/1464151/screenshots/11469899/media/4bda5be66067d24cd66fd4c761d9ab9b.png?compress=1&resize=400x300'},
                    {title:'Mobile App 4',image:'https://cdn.dribbble.com/users/404195/screenshots/13892505/media/541a6221e947a980b8f001b3837a0ab1.png?compress=1&resize=400x300'},
                    {title:'Mobile App 5',image:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcScWhy9sXTSwakJHgk-sEU3_6lDL56PlGzJYezAF7oAjVYTiKl4nbZSl31p_nzjoYHvJEc&usqp=CAU'},
                    {title:'Mobile App 6',image:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRW9Q_S3C6j2aSyMesVRlrNrPClSyPmeJNnv8624RPn43-YC_4vu9wyuz8dOKQFFSD8q28&usqp=CAU'},
                    {title:'Mobile App 7',image:'https://cdn.dribbble.com/users/404195/screenshots/13892505/media/541a6221e947a980b8f001b3837a0ab1.png?compress=1&resize=400x300'},
            ],
             DesktopApp: [{
                    title: 'Web App 1',
                    'image': "https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                },
                {
                    title: 'Web App 2',
                    'image': "https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                },
                {
                    title: 'Web App 3',
                    'image': "https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                },
            ]
        }
    }
}
</script>
