<template>
    <div class="search">
    <form action="" class="form">
        <div class="form-control">
            <div class="label">From</div>
            <input type="text" placeholder="Departure" class="input">
        </div>
        <div class="form-control">
            <div class="label">To</div>
            <input type="text" placeholder="Destination" class="input">
        </div>
        <div class="form-control">
            <div class="label">Travel Date</div>
            <input type="date" class="input date">
        </div>
        <div class="btn">
            Search Flight
        </div>

    </form>
    </div>
</template>
<style scoped>
.search{
    margin-bottom:5rem;
}
.form{
    margin:1.3rem 20rem;
    display:flex;
    align-items: center;
}


input{
    width:12rem;
    margin-right:2rem;
    font-family:var(--primary-font);
    border:0px;
    border-bottom:1px solid var(--primary);
    font-size:1.5rem;
}

.date{
    color:var(--primary);
}

input:focus{
    outline:none;
}
.btn{
    font-family:var(--primary-font);
    background:var(--primary);
    padding:1.1rem 1.5rem;
    color:white;
    font-size:1.2rem;
    cursor:pointer;
}

.btn:hover{
    font-family:var(--primary-font);
    background:var(--light-grey);
    padding:1.1rem 1.5rem;
    color:var(--primary);
    font-size:1.2rem;
    cursor:pointer;
}
.label{
    font-family:var(--primary-font);
    font-size:0.9rem;
    color:var(--primary);
    margin-bottom:0.6rem;
}

@media screen and (max-width: 768px){
    .form{
        margin:1.3rem 0.6rem;
        flex-direction:column;
        align-items: flex-start;
    }

    .form-control{
        margin-bottom:2rem;
    }

    .label{
        font-weight:bold;
    }

    input{
        width:100%;
    }

    .btn{
    font-family:var(--primary-font);
    border:2px solid var(--primary);
    padding:0.9rem 1.5rem;
    color:white;
    font-size:1.2rem;
    cursor:pointer;
    
}

    

}


</style>