<template>
    <div class="blogs">
        <div class="sections">
            <div class="box">
                <div class="image one">
                </div>
                <div class="info">
                    <p>Thank you for choosing <span class="text-logo">HelixAir</span>, the fastest growing airline and the popular name for affordable air travel. We are 4-star rated. And never compromise on quality customer service. Time is a priority and we ensure flights get to where you're going on time.</p>
                <!-- Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus doloremque cumque veniam minima minus ad magni ullam unde quaerat. Voluptatem repellendus sequi reprehenderit iusto facere? Veniam, nam sapiente! Quasi, molestiae. -->
                </div>
            </div>
            <div class="box">
                <div class="image two">
                </div>
                <div class="info">
                    Our flights range from economy, premium economy, business and first class. We make sure that all our passengers get the most of what they pay for to create a memorable traveling experience. 
                
                </div>
            </div>
        </div>
        <div class="heading">
            Let's Find You That Flight
        </div>
        <!-- <SearchForm/> -->
    </div>
</template>
<script>
import SearchForm from './SearchForm.vue'
export default {
    components: {
        SearchForm
    }
}
</script>
<style scoped>

.heading{
    margin:0rem 20rem;
    font-size:2.4rem;
    font-weight:bold;
    font-family:var(--logo-font);
    color:var(--primary);
    font-style:italic;
}
.text-logo{
    font-family:var(--logo-font);
    font-weight:bold;
    font-style:italic;
}
.one{
    background:url('../assets/images/img3.jpg')!important;
}

.two{
    background:url('../assets/images/img.jpg')!important;
}
.blogs{
    margin-top:2rem;
}
.sections{
    display:flex;
    flex-direction: column;
    align-items: center;
    padding:0rem 20rem;
}

.box{
    display:flex;
    /* min-height:20rem; */
    margin-bottom:5rem;
    
}

.image{
    min-height:20rem;
    background:blue;
    /* height:20rem; */
    flex:0.5;
    background-size:cover;
    background-repeat:no-repeat;
}

.info{
    background:var(--tertiary);
    flex:1;
    display: flex;
    align-items: center;
    padding:1rem;
    font-size:1.2rem;
    line-height:2.1rem;
    font-family:var(--primary-font);
    color:var(--primary);
    /* height:20rem; */
    
}
@media screen and (max-width: 768px){
    .box{
       /* flex-direction:column; */
       min-height:8rem;
    }

    .info{
        font-size:1rem;
        line-height:1.5rem;
    }

    .image{
    background:blue;
    background-size:cover;
    background-repeat:no-repeat;
}

    .sections{
    padding:0rem 1rem!important;
}

.heading{
    margin:0rem 1rem;
    text-align: center;
    font-size:1.5rem;
    font-weight:bold;
}

    
}
</style>