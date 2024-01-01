<template>
    <div class="description">
        <div class="sections">
            <div class="box small">
                <div class="icon">
                    <img src="../assets/icons/airplane.svg" class="ic"/>
                </div>
                <div class="info">
                    A dense network of global connections across the major continents to ensure that we take you to your destination. 
                </div>
            </div>
            <div class="box small">
                <div class="icon">
                    <img src="../assets/icons/taxi.svg" class="ic"/>
                </div>
                <div class="info">
                    Transportation services like Taxi, Family Van and Luxury Cars for first class passengers from your residence and at your remote destination.
                </div>
            </div>
            <div class="box small">
                <div class="icon">
                    <img src="../assets/icons/hotel.svg" class="ic"/>
                </div>
                <div class="info">
                    A special Hotel Booking service so you can have your accommodation sorted before you reach your destination. Seamless travel experience.
                   
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>

.ic{
    height:3.6rem;
}

.icon{
    display:flex;
    justify-content: center;
}
.description{
    margin-top:0.5rem;
}

.sections{
    display:flex;
}

.box{
    margin:1.4rem 4rem;
}

.info{
    font-family:var(--primary-font);
    line-height:1.8rem;
    font-size:1.2rem;
    text-align: center;
}

.icon{
    margin-bottom:2rem;
}

@media screen and (max-width: 768px){
    .sections{
        flex-direction:column;
    }

    .info{
    line-height:1.6rem;
    font-size:1rem;
}

.ic{
    height:3rem;
}

.icon{
    margin-bottom:1rem;
}

.small{
    margin-bottom:2.5rem!important;
}

.box{
    margin:0rem 0.8rem;
}

.description{
    margin-top:1rem;
}
}
</style>