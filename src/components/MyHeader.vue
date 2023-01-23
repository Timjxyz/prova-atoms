<template>
  <header>
    <div class="position-fixed">
      <div class="container">
          <!-- Header top -->
          <div class="header-top">
            <!-- Left section header top -->
            <div class="left-heder-top">
                <ul>
                  <li><a href="#">Contribusci</a></li>
                  <li><a href="#">Abbonati</a></li>
                </ul>
            </div>
            <!-- Right section header top -->
            <div  class="right-heder-top">
              <div><i class="fa-solid fa-user"></i> Accedi</div>
            </div>
          </div>
        </div>
        <hr>
        <!-- Section search -->
        <div class="container">
          <div class="search-menu">
            <div class="menu-hidden">
              <i class="fa-solid fa-bars"></i>
            </div>

            <div class="search-icon">
              <i class="fa-solid fa-magnifying-glass"></i>
            </div>
          </div>
        
        </div>
      <hr>
        <!-- Section link pages -->
        <div class="container">
          <nav>

            <ul>
              <li v-for="(link, index) in links_nav" :key="index" >
                <a :class="link.current?'active':''" :href="link.url"> {{link.text}}</a>
              </li>
              
            </ul>
            <div class="nav-icon">
              Aa<i class="fa-solid fa-image"></i>
            </div>
            
          </nav>

        </div>
      <hr>

    </div>
    <div class="container">
      <div class="header-bottom">
        <div class="title">
          <h2>Tutti i temi</h2>
        </div>
        <ul>
          <li v-for="(link, index) in links_button" :key="index" >
            <button v-bind:style="{ 'background-color':link.color}"> {{link.text}}</button>
          </li>
            
        </ul>
        
      </div>

    </div>
   <hr>
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
                color:"#9afda4",
              },
              {
                text: "ECONOMIA",
                color:"#fff",
              },
              {
                text: "MONDO",
                color:"#fd9aac",
              },
              {
                text: "NON PROFIT",
                color:"#fff",
              },
              {
                text: "POLITICA",
                color:"#f5fd9a",
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

//General rules page
.position-fixed{
  position: fixed;
  top: 0px;
  width: 100%;
  background-color: #fff;
}
hr{
  border: 1px solid #000;
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
//End general rules page
.container{
 
  width: 90%;
  .header-top{
   
    height: 50px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .search-menu{
    height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .fa-solid{
      color: #f90202;
      font-size: 40px;
    }
    .menu-hidden{
      height: 100%;
      width: 100px;
      display: flex;
      border-right: 3px solid #000;
      align-items: center;
      justify-content: center;
      
    }
    .search-icon{
      height: 100%;
      width: 100px;
      display: flex;
      border-left: 3px solid #000;
      align-items: center;
      justify-content: center;
     
    }
  }
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
        padding: 20px;
        font-size: 24px;
        color: #000;
        font-weight: 700;
        padding-bottom: 20px;
  
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
  margin-top: 250px;
  height: 200px;
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
        margin: 0px 10px;
        border-radius: 5px;
        color: #000;
        font-weight: 600;
        box-shadow: -2px 2px 1px 0px;
      }
    }
  }
}

</style>
