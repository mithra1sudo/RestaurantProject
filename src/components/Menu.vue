<template>
    <v-container>
        <v-card color="blue" >
            <v-card-title>
                <div class="text-h3">Our Menu</div>
            </v-card-title>
        </v-card>
    </v-container>
    <v-container><!--Outer Container-->
        <v-card class="mx-auto" elevation="24">
            <v-container>
            <v-row>
                <v-col cols="12" md="4" v-for="item in menuItems" :key="item"><!--This creates a loop-->
                    <v-card>
                        <v-container>
                        <v-card color="#0D47A1">
                            <v-card-item>
                                <v-card-title>{{item.name}}</v-card-title>

                                <v-card-subtitle>{{item.description}}</v-card-subtitle>
                            </v-card-item>
                            <v-img height="200px" src="pexels-brett-sayles-1374552.jpg" cover ></v-img>

                            <v-card-text>
                            {{ item.price }}
                            </v-card-text>
                        </v-card>
                        </v-container>
                    </v-card>
                </v-col>
            </v-row>
        </v-container>
        </v-card>    
                    
 </v-container>
</template>

<script setup>
const menuItems = [
    {
        name: "Chips",
        price: 200,
        description: "Best chips in town",
        size: "Large",
        offers: "None",
        image: "/pexels-dzeninalukac-1583891.jpg"
    },
    {
        name: "Sausage",
        price: 50,
        description: "Best sausages in town",
        size: "None",
        offers: "None",
        image: "/pexels-amanda-lim-5074906-8508108"
    },
    {
        name: "Soda",
        price: 100,
        description: "Best soda in town",
        size: "Large",
        offers: "None",
        image: "/pexels-aj4xo-29336185.jpg"
    },
    {
        name: "Chapati",
        price: 50,
        description: "Best chapati in town",
        size: "None",
        offers: "None",
        image: "/pexels-zia-uddin-shah-392997573-18657574.jpg"
    },
    {
        name: "Tea",
        price: 80,
        description: "Best tea in town",
        size: "Large",
        offers: "None",
        image: "/pexels-valeriya-842544.jpg"
    },
    {
        name: "Sushi",
        price: 5000,
        description: "Best sushi in town",
        size: "None",
        offers: "None",
        image: "/pexels-valeriya-1052189.jpg"
    },
    {
        name: "Rice",
        price: 200,
        description: "Best chips in town",
        size: "Large",
        offers: "None",
        image: "/pexels-dzeninalukac-1583891.jpg"
    },
    {
        name: "Sausage",
        price: 50,
        description: "Best sausages in town",
        size: "None",
        offers: "None",
        image: "/pexels-amanda-lim-5074906-8508108"
    },
    {
        name: "Soda",
        price: 100,
        description: "Best soda in town",
        size: "Large",
        offers: "None",
        image: "/pexels-aj4xo-29336185.jpg"
    },
    {
        name: "Chapati",
        price: 50,
        description: "Best chapati in town",
        size: "None",
        offers: "None",
        image: "/pexels-zia-uddin-shah-392997573-18657574.jpg"
    },
    {
        name: "Tea",
        price: 80,
        description: "Best tea in town",
        size: "Large",
        offers: "None",
        image: "/pexels-valeriya-842544.jpg"
    },
    {
        name: "Wine",
        price: 5000,
        description: "Best wine in town",
        size: "None",
        offers: "None",
        image: "/pexels-hkn-clk-2148641156-30767623.jpg"
    }
]
</script>