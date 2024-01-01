<template>
    <div class="nav">     
        <div class="left">
            <div class="logo">HelixAir</div>
            <div class="links">
                <div class="link">Flights</div>
                <div class="link">Car Hire</div>
                <div class="link">Hotels</div>
                <div class="link">Contact Us</div>
                            
            </div>
        </div>
        <div class="right" v-on:click="ToggleMenu">
            <img src="../assets/icons/menu.svg" style="height:1.8rem;">
        </div>
        <div class="side-menu" v-show="toggled">
            <div class="heading">Menu</div>
            <div class="side-links">
                <div class="side-link">
                    Flights
                </div>
                <div class="side-link">
                    Car Hire
                </div>
                <div class="side-link">
                    Hotels
                </div>
                <div class="side-link">
                Contact Us
                </div>
            </div>
        </div>
    </div>
    
</template>
<script>
export default {
    data(){
        return{
            toggled: false
        }
    },
    methods:{
        ToggleMenu(){
            if(this.toggled == true){
                this.toggled = false;
            }else{
                this.toggled = true;
            }
        }
    }
}
</script>
<style scoped>


.heading{
    color:white;
    font-family:var(--logo-font);
    font-size:1.4rem;
    padding-bottom:0.5rem;
    border-bottom:1px solid white;
    margin-bottom:0.9rem;
    width:16rem;
    
}
.side-menu{
    background:var(--faint-primary);
    padding-left:3rem;
    padding-top:1rem;
    height:20rem;
    position:absolute;
    top:0;
    left:0;
    right:0;
    margin-top:3.6rem;
    display:none;

}

.side-link{
    margin-bottom:1.5rem;
    color:white;
    font-family:var(--primary-font);
    font-size:1.2rem;
}

.nav{
    /* background: BLUE; */
    background:var(--faint-white);
    backdrop-filter:blur(3px);
    position:fixed;
    top:0;
    left:0;
    right:0;
    width:100vw;
    min-height:3rem;
    display:flex;
    justify-content: space-between;
    align-items: center;
    padding:0.5rem 2.8rem;
}

.logo{
    margin-right:2rem;
    font-family:Montserrat;
    font-size:1.7rem;
    font-weight:Bold;
    font-style:italic;
    color:var(--primary);

}

.letter{
    /* color:rgb(136, 108, 108); */
}

.grad{
    
    background: -webkit-linear-gradient(60deg,var(--primary),var(--secondary), rgb(255, 255, 255));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.link{
    margin:0rem 1.6rem;
    font-family:Roboto;
}

.links{
    display:flex;
    color:var(--primary);
}

.left{
    display:flex;
    align-items: center;
}

@media screen and (max-width: 768px){

    .nav{
        min-height:2.6rem;
        padding:0.5rem 1rem;
    }  
    .left{ 
        justify-content: space-between!important;  
    }

    .right{
        margin-right:2rem;
    }
    .link{
        display:none;
    }

    .side-menu{
        display:block;
    }
}
</style>