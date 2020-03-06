<template>
    <div>
        <app-header></app-header>
        <div class="container-fluid about-container-title">
            <div class="mt-5 text-title">
                <p class="h3 font-weight-bold text-center text-monospace">-</p>
                <p class="h2 text-center text-monospace">about</p>
            </div>
        </div>
        <div class="container-fluid about-container">
            <div class="row mt-5 mb-5">
                <div class="col-md-6 d-flex">
                    <div class="justify-content-center align-self-center mx-auto about">                    
                        <img src="static/pictures/team.png" alt="about">
                    </div>
                </div>
                <div class="col-md-6 text text-justify align-self-center">
                    <p class="font-italic font-weight-bold mt-2">
                            歡迎來到iNKPOT!很高興你喜歡我們，我們創立於2019年的一個春天，我們是一群喜歡玩弄鋼筆墨水紙張的小團體。
                        </p>
                    <p class="text-monospace">
                        歡迎來到iNKPOT!很高興你喜歡我們，我們創立於2019年的一個春天，
                        我們是一群喜歡玩弄鋼筆墨水紙張的小團體。歡迎來到iNKPOT!很高興你喜歡我們，我們創立於2019年的一個春天，
                        我們是一群喜歡玩弄鋼筆墨水紙張的小團體。歡迎來到iNKPOT!很高興你喜歡我們，我們創立於2019年的一個春天，
                        我們是一群喜歡玩弄鋼筆墨水紙張的小團體。
                    </p>
                </div>
            </div>
        </div>
        <app-footer></app-footer>
    </div>
</template>
<script>
import header from '../components/home/Header';
import footer from '../components/home/Footer';
export default {
    components:{
        'app-header':header,
        'app-footer':footer,
    }
}
</script>
<style>
@media (min-width: 992px){
    .about-container-title{
        margin-top: 5rem;
    }
    .about-container{
        margin-bottom: 9rem;    
    }
    .about{ 
        animation: waves 1.5s alternate infinite;
    }
   .text{
        padding-right: 9rem;
        padding-left: 1.5rem;
    }
   .about img{
        margin-left: -10%;
    }
}
@media (min-width: 768px) and (max-width: 991px){
    .about-container-title{
        margin-top: 5rem;
    }
    .about-container{
        margin-bottom: 9rem;    
    }
    .about{ 
        animation: waves 1.5s alternate infinite;
    }
    .text{
        padding-right: 6rem;
    }
    .about img{
        width: 150%;
        margin-left: -32%;
    }
}
@media (max-width: 767px){ 
    h1{
        line-height: 0;
    }
    .text{
        padding: 2.5rem;
    }
    .about{
        /* padding: 0 1rem; */
        margin-top: -30px;
        margin-bottom: -10px;   
    }
    .about img{
        width: 100%;
    }
}
.text-title{
    color: #007bff;
    animation: change 2s infinite;
}
@keyframes change{
    from{ color: #007bff; }
    to{ color: #ee8a42; }
}@keyframes waves {
    from {transform: rotate(-20deg);}
    to{
        transform: rotate(20deg);
        transform: translate(5rem, 0);}
}
p{
    margin: auto;
}
/* .text-title{
    color: #323232;
} */
.text{
    color: #495057;
}

</style>