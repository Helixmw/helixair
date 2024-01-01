<template>
    <div class="footer-mobile">
        <div class="copyright">
            {{ year }} &copy; HelixAir. All rights reserved.
        </div>
        <div class="footer-links">
            <div class="footer-link">
                <img src="../assets/icons/instagram.svg" class="social">
                
            </div>
            <div class="footer-link">
                <img src="../assets/icons/facebook.svg" class="social">
                
            </div>
            <div class="footer-link">
                <img src="../assets/icons/whatsapp.svg" class="social">
                
            </div>
        </div>
    </div>
    <div class="footer">
        <div class="copyright">
            {{ year }} &copy; HelixAir. All rights reserved.
        </div>
        <div class="footer-links">
            <div class="footer-link">
                <img src="../assets/icons/instagram.svg" class="social">
                
            </div>
            <div class="footer-link">
                <img src="../assets/icons/facebook.svg" class="social">
                
            </div>
            <div class="footer-link">
                <img src="../assets/icons/whatsapp.svg" class="social">
                
            </div>
        </div>
        <div class="footer-logo">
            HelixAir
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
            year: 0
        }
    },
    mounted(){
        let currDate = new Date();
        this.year = currDate.getFullYear();
    }
}
</script>
<style scoped>

.copyright{
    color:white;
    font-family:var(--primary-font);
    font-size:0.9rem;
    
}

.footer-logo{
    color:white;
    font-family:var(--logo-font);
    font-weight:bold;
    font-style:italic;
    font-size:2rem;
}


.footer-links{
    display:flex;
    margin-right:3rem;
}
.footer-link{
    margin:0rem 1rem;
}
.footer{
    background:var(--primary);
    /* max-width:100vw; */
    padding:1.3rem 2.5rem;
    display:flex;
    justify-content: space-between;
    
}

.social{
    height:2.5rem;
}

.footer-mobile{
    display:none;
}

@media screen and (max-width: 768px){

.footer-mobile{
    display:flex;
    flex-direction: column;
    align-items: center;
    background:var(--primary);
    margin-left:1rem;
    
}
.footer-logo{
    display:none;
}

.footer-links{
   
    margin-right:2rem;
}
.footer{
    display:none;
    max-width:100%;
    padding:0rem 0rem;
    flex-direction: column;

    
}
}
</style>