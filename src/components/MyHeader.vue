<template>
  <header>
    <div class="fixed-top bg-light">
      <div class="container-fluid my-position-relative">
          <span class="  border-end border-secondary border-start border-secondary d-block d-sm-none my-h-100"></span>
        <div class="row border-bottom pt-3 border-secondary">
            <!-- Header top -->
            <div class="header-top row d-flex d-flex justify-content-between ">
              <!-- Left section header top -->
              <div class="left-heder-top col-12 col-sm-2 ">
                  <ul class="d-flex justify-content-around ms-5">
                    <li class="col-xs-6"><a href="#">Contribusci</a></li>
                    
                    <li class="col-xs-6"><a href="#">Abbonati</a></li>
                  </ul>
              </div>

              <!-- <div class="col-10 col-sm-auto"></div> -->

              <!-- Right section header top -->
              <div  class="right-heder-top col-1 col-sm-2 text-end d-none d-sm-inline-block me-5">
                <div><i class="fa-solid fa-user "></i> Accedi</div>
              </div>
            </div>
          </div>
          </div>
          <!-- Section search -->

            <div class="container-fluid border-bottom border-secondary ">

                <div class=" row d-flex d-flex justify-content-between ">

                  <div class="menu-hidden col-2 col-sm-1 col-xs-2 text-center">
                    <a href="#"><i class="fa-solid fa-bars fs-1 text-danger  pt-4 pb-4"></i></a>
                  </div>
                  <div class=" col-sm-10 col-8 border-start border-secondary border-end border-secondary pt-4 pb-4"></div>
                  
                  <div class="search-icon col-2 col-sm-1 col-xs-2  text-center ">
                    <a href="#">
                      <i class="fa-solid fa-magnifying-glass text-danger fs-1 pt-4 pb-4"></i>
                    </a>
                  </div>
                </div>

            </div>


          <!-- Section link pages -->
          <div class="container-fluid border-bottom border-secondary d-none d-lg-inline-block">
            <nav class="row justify-content-around">

              <ul class="col-11">
                <li v-for="(link, index) in links_nav" :key="index" >
                  <a :class="link.current?'active':''" :href="link.url"> {{link.text}}</a>
                </li>

              </ul>
              <div class="nav-icon col-1 text-end ">
                Aa<i class="fa-solid fa-image"></i>
              </div>

            </nav>

          </div> 

    </div>

    <!-- Section button  -->
    <div class="container-fluid my-mt-10 mb-4">
      <div class="header-bottom row">
        <div class="title col-12 col-lg-4 ps-5">
          <h2>Tutti i temi <i class="fa-solid fa-chevron-down fs-1 d-inline-block d-lg-none"></i></h2>
        </div>
        <ul class=" col-12 col-lg-8 d-flex flex-wrap ">
          <li class="mx-3 my-3" v-for="(link, index) in links_button" :key="index" >
            <button :style="{ 'background-color':link.color}"> {{link.text}}</button>
          </li>

        </ul>

      </div>

    </div>
  </header>
</template>

<script>
export default {
  name: 'MyHeader',
  data() {
    return {
      links_nav: [
              {
                  text: "Tutti i temi",
                  url: "#",
                  current: true,
              },
              {
                  text: "Ambiente",
                  url: "#",
                  current: false,
              },
              {
                  text: "Economia",
                  url: "#",
                  current: false,
              },
              {
                  text: "Mondo",
                  url: "#",
                  current: false,
              },
              {
                  text: "Non Profit",
                  url: "#",
                  current: false,
              },
              {
                  text: "Politica",
                  url: "#",
                  current: false,
              },
              {
                  text: "Società",
                  url: "#",
                  current: false,
              },
              {
                  text: "Welfare",
                  url: "#",
                  current: false,
              },
      ],

      links_button: [
              {
                text: "AMBIENTE",
                color:"#cbffd0e2",
              },
              {
                text: "ECONOMIA",
                color:"#fff",
              },
              {
                text: "MONDO",
                color:"#fdc5c5",
              },
              {
                text: "NON PROFIT",
                color:"#fff",
              },
              {
                text: "POLITICA",
                color:"#f5fab9",
              },
              {
                text: "SOCIETÀ",
                color:"#fff",
              },
              {
                text: "WELFARE",
                color:"#fff",
              },
      ],
    }

  }
}
</script>


<style scoped lang="scss">
.my-mt-10{
  margin-top: 250px;
}
.my-position-relative{
  position: relative;
}
.my-h-100{
  height: 100%;
 position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
 ul{
   display: flex;
   li{
     list-style: none;
   }
 }

 a{
   text-decoration: none;
   padding: 10px;
   font-size: 14px;
   color: #000;
   font-weight: 500;
   padding-bottom: 36px;
 }

//Nav section
 nav{
   height: 89px;
   display: flex;
   justify-content: space-between;
   align-items: center;

   ul{
     li{
       a{
         height: 100%;
         text-decoration: none;
         font-size: 24px;
         color: #000;
         font-weight: 700;
         padding-bottom: 30px;

         &.active, &:hover{
           border-bottom: 8px solid #f90202;

         }
       }
     }
   }
   .nav-icon{
     font-size: 30px;
     .fa-image{

       border: 1px solid #000;
       padding: 5px;
       border-radius: 5px;
       margin-left: 10px;
       box-shadow: -2px 2px 1px 0px;
     }
   }
}

//Header bottom section
.header-bottom{


  display: flex;
  justify-content: space-between;
  align-items: center;
  h2{
    font-size: 60px;
  }

  ul{
    li{
      button{
        text-align: center;
        padding: 10px;
      
        border-radius: 5px;
        color: #000;
        font-weight: 600;
        box-shadow: -2px 2px 1px 0px;
      }
    }
  }
}

</style>
