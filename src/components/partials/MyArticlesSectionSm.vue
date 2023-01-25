<template>
 <article class="container-fluid d-lg-none">
<div class="row">
          <section class="jumbo-img col-12 px-0">
            <img class="img" src="http://i.cdn-vita.it/blobs/variants/4/6/2/0/4620b827-814a-4700-a7f2-05fb61b292e5_xl.jpg?_637932931424474332" alt="Roccella Jonica, la Lampedusa che l'Italia ignora">
            <div>
              <div class="img-content">
                <div class="banner">
                  <span>
                    <strong>MIGRANTI</strong>
                  </span>
                </div>
                <h2 class="title-img">
                  <strong>Roccella Jonica, la Lampedusa che l'Italia ignora</strong> 
                </h2>
                <div class="autor-information">
                  <img class="autor-img" src="../../assets/img/alessandro-puglia.jpg" alt="Alessandro Puglia">
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
       <section class="article-section-bottom  pt-1 row">
       
        <div class="jumbo-img mt-3 col-12  border-bottom border-dark ">
            <img class="img"  src="https://www.zai.net/articoli_files/thumbnails/800/600/2c3263c1ca793825b6bffa96f5291d55.jpeg" alt="collasso dei ghiaccia">
              <div class="img-content-sm">
                <div class="banner my-3">
                  <span style="background-color:#cbffd0e2">
                    <strong>ALLARMI</strong>
                  </span>
                </div>
                <h2 class="title-img mb-4">
                 <strong>Il collasso dei ghiaccia negli scatti del fotografo ambientale Fabiano Ventura</strong>
                </h2>
                <div class="autor-information">
                  <img class="autor-img" src="../../assets/img/alessandro-puglia.jpg" alt="Ugo Lombi">
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
       
        <div class="jumbo-img mt-3 col-12  border-bottom border-dark ">
            <div class="banner my-3">
                <span  style="background-color:#d5e0f9">
                    <strong>ESPERIMENTI</strong>
                </span>
            </div>
            <img class="w-100" src="../../assets/img/audio.jpg" alt="audio">
            <div class="img-content-sm">
                <div class="title-img mb-4 fs-3 fw-bolder">
                    Gli startupper? Li trovi al bistrot. Così il DumBo incuba relazioni
                </div>
                <div class="autor-information">
                  <img class="autor-img" src="https://i.cdn-vita.it/blobs/author/0/53.jpg?_635870708080865332" alt="Diletta Grella">
                  <div class="name-autor">
                    <div>
                      Di Diletta Grella
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
        *
        *Third article -->
        <div class="jumbo-img mt-3 col-12  border-bottom border-dark ">
            <div class="banner my-3">
                <span style="background-color:#fdc5c5">
                    <strong>UCRAINA</strong>
                </span>
            </div>
            <div class="img-content-sm">
                <div class="title-img mb-4 fs-3 fw-bolder">
                   Nella città italiane tutti in piazza per e con Kiev
                </div>
                <div class="autor-information">
                  <img class="autor-img" src="https://i.cdn-vita.it/blobs/author/0/10.jpg?_635634793293794669" alt="Anna Spena">
                  <div class="name-autor">
                    <div>
                      Di Anna Spena
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
       
      </section> 
      
 </article>
</template>

<script>



export default {
 name:'MyArticlesSectionSm',
 
}
</script>


<style scoped lang="scss">
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
    
    .img{
      height: 350px;
      width: 100%;
      object-fit: cover;
      
    }
    .title-img{
      font-size: 30px;
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


    }
        .banner{
            span{
            background-color: #fff;
           
            padding: 4px 10px;
            font-size: 14px;
           
            text-align: center;
           
            border-radius: 5px;
            color: #000;
            font-weight: 600;
            box-shadow: -4px 4px 1px 0px;
            }
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
  
</style>