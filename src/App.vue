<script setup>
import StatisticCard from './components/StatisticCard.vue';


const products=[
  

{
    "icon": "https://d12jofbmgge65s.cloudfront.net/wp-content/uploads/2023/01/tech-guide_header-image-twitch.webp",
    "name": "Twitch Posts",
    "new": "500.00",
    "unit": "$",
    "last": "+40.5%",
    "what":"more impressions",
    "info": "0.5% MRR" 
},
{
    "icon": "https://img.freepik.com/premium-vector/new-twitter-logo-x-2023-twitter-x-logo-vector-download_691560-10809.jpg",
    "name": "Twitter Followers",
    "new": "807",
    "unit": "k",
    "last": "+17.62%",
    "what":"Followers growth",
    "info": "5% New trials" 
},
{
    "icon": "https://upload.wikimedia.org/wikipedia/commons/thumb/8/84/Spotify_icon.svg/1982px-Spotify_icon.svg.png",
    "name": "Spotify Listeners",
    "new": "1,073",
    "unit": "k",
    "last": "+10.45%",
    "what":"Less comments than usual",
    "info": "40% Impressions" 
},
{
    "icon": "https://upload.wikimedia.org/wikipedia/commons/0/08/Pinterest-logo.png",
    "name": "Pinterest Posts",
    "new": "97",
    "unit": "k",
    "last": "+26.1%",
    "what":"More posts",
    "info": "10% Spend" 
},
{
    "icon": "https://cdn-icons-png.flaticon.com/512/25/25231.png",
    "name": "Github Contributes",
    "new": "4,109",
    "unit": "k",
    "last": "+32.8%",
    "what":"Less Contributors",
    "info": "40% Dispute" 
},
{
    "icon": "https://img.freepik.com/premium-vector/red-youtube-logo-social-media-logo_197792-1803.jpg",
    "name": "Youtube Subscribers",
    "new": "354",
    "unit": "k",
    "last": "+29.45",
    "what":"Subscribers growth",
    "info": "40% Subscribers" 
}
]

</script>

<template>
<div class="grid grid-cols-3 gap-4 p-5">
  <StatisticCard v-for="product in products" :details="product" :key="product.name" class="col-span-1"/>
</div>

</template>

<style scoped>

</style>
