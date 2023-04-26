<template>
    <section class="flex flex-row Hero-container">
        <div class="basis-1/2 hero-text">
                <h1>Welcome to DREAMLABS</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure possimus molestiae optio dolor itaque.</p>
                <button>Explore More</button>
        </div>
        <div class="basis-1/2">
            <h1>sofujvnkfjvn</h1>
        </div>
        
    </section>
</template>

<script setup>

</script>

<style scoped>
    .Hero-container{
        top: 65px;
        background-image: url("https://images.unsplash.com/photo-1633432695542-b2c8e2b8a26c?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1032&q=80");
        height: 85vh;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        position: relative;
    }

    .hero-text{
        text-align: left;
        font-size: 34px;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: white;
        margin-top: 10px;
    }

    .hero-text h1{
        text-align: left;
        font-size: 34px;
        font-weight: 800;
    }

    .hero-text p {
        text-align: left;
        font-size: 30px;
        font-weight: 500;
        padding-top: 15px;
        padding-bottom: 39px;
        font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    }

    .hero-text button{
        border: white;
        border-radius: 15px;
        display: inline-block;
        padding: 12px 17px;
        color: white;
        background: black;
        opacity: 80%;
    }

    @media(max-width:1280px){
        .hero-text button{
            display: inline-block;
            padding: 12px 17px;
        }
    }

    @media(max-width: 1090px){
        .hero-text button{
            
            font-size: 18px;
            display: inline-block;
            padding: 12px 17px;
        }
    }

    @media(max-width: 748px){

        .hero-text p {
            font-size: 22px;
            font-weight: 400;
            padding-top: 15px;
            padding-bottom: 32px;
        }
        .hero-text button{
            align-items: flex-start;
            margin-top: 15px;
            font-size: 15px;
            display: inline-block;
            padding: 8px 13px;
        }
    }


</style>