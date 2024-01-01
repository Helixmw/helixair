<template>
    <div class="welcome">
        <div class="greeting">
            <div class="logo">
                HelixAir
            </div>
            <div class="slogan">

                Affordable Flights Going Across The World
            </div>
            <div class="buttons">
                <div class="link-button">Booking</div>
                <div class="link-button different">Register</div>
            </div>
        </div>
    </div>
</template>
<style scoped>

.buttons{
    display:flex;
}

.link-button{
    font-family:var(--primary-font);
    margin:0rem 0.5rem;
    background:var(--faint-white-two);
    font-size:1.5rem;
    color:var(--primary);
    padding:0.4rem 1.5rem;
}

.different{
    background:var(--faint-black);
    color:white;
    border:1px solid white;
}
.welcome{
    background:url('../assets/images/bg3.jpg');
    background-size: cover;
    background-repeat:no-repeat;
    height:67vh;
    display: flex;
    justify-content: center;
    align-items: center;
    
}

.logo, .slogan{
    margin-bottom:1.2rem;
    color:white;
}

.logo{
    margin-top:4rem;
    font-family:var(--logo-font);
    font-style:italic;
    font-size:2.6rem;
    font-weight: bold;
}

.slogan{
    font-family:var(--secondary-font);
    font-style:italic;
    font-size:1.4rem;
}

.greeting{
    display:flex;
    flex-direction: column;
    align-items: center;   
}

@media screen and (max-width:768px){
    .slogan{
        font-size:1rem;
    }

    .logo, .slogan{
    margin-bottom:1rem;
   
}

.buttons{
    margin-top:1rem;
}
.link-button{
    padding:0.4rem 1.5rem;
    font-size:1.3rem;
}
}
</style>