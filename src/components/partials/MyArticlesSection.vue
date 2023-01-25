<template>
    <article class="container-fluid ">
      <!-- Top articles section -->
      
        <div class="row d-none d-lg-block">
          <section class="jumbo-img col-12 px-0">
            <img src="http://i.cdn-vita.it/blobs/variants/4/6/2/0/4620b827-814a-4700-a7f2-05fb61b292e5_xl.jpg?_637932931424474332" alt="Roccella Jonica, la Lampedusa che l'Italia ignora">
            <div>
              <div class="img-content">
                <div class="banner">
                  <span>
                    <strong>MIGRANTI</strong>
                  </span>
                </div>
                <h2 class="title-img">
                  Roccella Jonica, la Lampedusa che l'Italia ignora
                </h2>
                <div class="autor-information">
                  <img class="autor-img" src="../../assets/img/alessandro-puglia.jpg" alt="">
                  <div class="name-autor">
                    <div>
                      Di Alessandro Puglia
                    </div>
                    <div class="data-article">
                      29 Giugno 2022
                    </div>

                  </div>
                </div> 
              </div>
            </div>
          </section>
        </div>
      <!-- Bottom article Section -->

      <!-- Articles on the left section
      *
      *
      *First article -->
       <section class="article-section-bottom  pt-1 row d-none d-lg-block">
       
          <div class="jumbo-img float-left col-8 px-0">
            <img class="float-img" src="https://www.zai.net/articoli_files/thumbnails/800/600/2c3263c1ca793825b6bffa96f5291d55.jpeg" alt="collasso dei ghiaccia">
            <div class="overlay"></div>
          
              <div class="img-content">
                <div class="banner">
                  <span>
                    <strong>ALLARMI</strong>
                  </span>
                </div>
                <h2 class="title-img">
                  Il collasso dei ghiaccia negli scatti del fotografo ambientale Fabiano Ventura
                </h2>
                <div class="autor-information">
                  <img class="autor-img" src="../../assets/img/alessandro-puglia.jpg" alt="">
                  <div class="name-autor">
                    <div>
                      Di Ugo Lombi
                    </div>
                    <div class="data-article">
                      14 Luglio 2022
                    </div>

                  </div>
                </div>
                <div class="arrow-link">
                  <a href="#"><i class="fa-solid fa-arrow-right"></i></a>
                </div> 
              </div>
          </div>

          <!-- Articles on the right section
          *
          *Second article -->
          <div class=" float-right col-4 ps-1 px-0 ">
            <div  class="article-section jumbo-img ">
            <img class="w-100" src="https://i.cdn-vita.it/blobs/variants/0/0/8/3/00839a64-e373-4676-8e8f-29723582e09f_large.jpg?_637916005237652666" alt="gli startupper">
            <div class="overlay"></div>

              <div class="img-content">
                <div class="banner col-12 d-inline-block">
                  <span>
                    <strong>ESPERIMENTI</strong>
                  </span>
                </div>
                <div class="col-12">
                  <img class="audio" src="../../assets/img/audio.jpg" alt="audio">
                </div>
                <h2 class="title-img col-12">
                  Gli startupper? Li trovi al bistrot. Così il DumBo incuba relazioni
                </h2>
                <div class="autor-information col-12">
                  <img class="autor-img" src="https://i.cdn-vita.it/blobs/author/0/53.jpg?_635870708080865332" alt="">
                  <div class="name-autor">
                    <div>
                      Di Diletta Grella
                    </div>
                    <div class="data-article">
                      14 Luglio 2022
                    </div>

                  </div>
                </div>
                <div class="arrow-link col-12">
                  <a href="#"><i class="fa-solid fa-arrow-right"></i></a>
                </div> 
              </div>

            </div>
          
       

            <!-- Articles on the right section
            *
            *Third article -->
            
            <div class="jumbo-img mt-1">
              <img src="https://torange.biz/photo/51/HD/ukrainian-flag-flags-cloth-51266.jpg" alt="collasso dei ghiaccia">
              <div class="overlay"></div>

                <div class="img-content">
                  <div class="banner col-12">
                    <span>
                      <strong>UCRAINA</strong>
                    </span>
                  </div>
                  <h2 class="title-img col-12">
                    Nella città italiane tutti in piazza per e con Kiev
                  </h2>
                  <div class="autor-information col-12">
                    <img class="autor-img" src="https://i.cdn-vita.it/blobs/author/0/10.jpg?_635634793293794669" alt="ucraina">
                    <div class="name-autor">
                      <div>
                        Di Anna Spena
                      </div>
                      <div class="data-article">
                        14 Luglio 2022
                      </div>
                    
                    </div>
                  </div> 
                  <div class="arrow-link col-12">
                      <a href="#"><i class="fa-solid fa-arrow-right"></i></a>
                    </div>
                </div>
            </div>

          </div>
       
      </section>  

    <MyArticlesSectionSm class="d-lg-none"/>
      <div class="row py-5 support-section">
        <div class="col-10 col-lg-10">
          <h3 class="fs-1 fw-bolder">Il tuo supporto è fondamentale</h3>
        </div>
        <div class="col-12 col-lg-2">
          <span class="fs-3 fw-bolder">Dai il tuo contributo <i class="fa-solid fa-arrow-right"></i></span>
        </div>
      </div>
     
  </article>
</template>

<script>


import MyArticlesSectionSm from './MyArticlesSectionSm.vue';
export default {
 name:'MyArticlesSection',
 components: {
    MyArticlesSectionSm
  },
}
</script>


<style scoped lang="scss">

.support-section{
  background-color: #f4f1de;
}
 .overlay{
      background-color: rgba(0, 0, 0, 0.3);
      height: 100%;
      width: 100%;
      position: absolute;
      top: 0;
      left: 0;
      object-fit: contain;
    }

.arrow-link{
  a{
    text-decoration: none;
    color: #fff;
    font-size: 20px;
  }
}




  .jumbo-img{
    position: relative;
    display: grid;
    
    img{
      height: 560px;
      width: 100%;
      object-fit: cover;
      
    }
    .title-img{
      font-size: 40px;
    }
    .autor-img{
      width: 50px;
      height: 50px;
      object-fit: cover;
      border-radius: 50%;
    }
    .img-content{
      position: absolute;
      bottom:50px;
      left: 30px;
      vertical-align: middle;
      color: #fff;

      .banner{
        span{
          background-color: #fff;
          color: #000;
          padding: 2px 8px;
          font-size: 10px;
          border-radius: 10px;
        }
      }

      .autor-information{
      position: relative;
      margin-top: 10px;
      .name-autor{
        position:absolute;
        left: 60px;
        bottom: 10px;
      }
      .data-article{
        font-size: 12px;
        margin-top: 10px;
      }
    }
    }
    
  }
  .float-left{
    display: grid;
    float: left;
    width: 60%;
    position: relative;
    img{
      height: 800px;
      object-fit: cover;
    }
   
  }
  .float-right{
    display: grid;
    width: 40%;
    position: relative;
    img{
      height: 400px;
      object-fit: cover;
    }
    
   
   
    .audio{
      height: 40px;
      margin-top: 10px;
      width: 60%;
      border-radius: 10px;
    }
  }
</style>