<template>
  <div>
    <h1>TEXT:{{...this.book}}</h1>
    <div class="search_selection">
      <div class="selection_bookbox">
        <img class="bookbox_img" v-bind:src="this.book.urlimg" alt="">
      </div>
    </div>
    <div class="search_customers">
      <div class="customers_tittle">
        <h2>Sprzedający</h2>
      </div>
      <div class="customers_box">
          <ul class="custom_ul">
            <li
            
              class="custom_li"
            >Krok w przedsiębiorczość Podręcznik</li>
            <li  class="custom_li">To jest chemia</li>
            <li
            
              class="custom_li"
            >Fizyka - ODKRYĆ FIZYKĘ - Nowa Era - podstawowy</li>
            <li class="custom_li">Oblicza geografii</li>
            <li  class="custom_li">Biologia na czasie</li>
            <li
             
              class="custom_li"
            >Spotkania z kulturą podręcznik Liceum i technikum</li>
            <li
              
              class="custom_li"
            >Ponad słowami podręcznik klasa 1 CZ. 1 NOWA ERA</li>
            <li
              
              class="custom_li"
            >Informatyka Europejczyka Podręcznik z płytą CD</li>
            <li class="custom_li">W centrum uwagi</li>
            <li
             
              class="custom_li"
            >Świat fizyki Podręcznik. Zakres podstawowy</li>
            <li
              class="custom_li"
            >Wiedza o kulturze SPOTKANIA Z KULTURĄ Podręcznik</li>
            <li
             
              class="custom_li"
            >Język polski Świat do przeczytania cz.1</li>
            <li  class="custom_li">PONAD SŁOWAMI 1.2 NOWA ERA</li>
            <li
             
              class="custom_li"
            >Matematyka 1. Zakres podstawowy i rozszerzony</li>
            <li
              
              class="custom_li"
            >Informatyka Europejczyka Zakres podstawowy Podr.</li>
            <li
             
              class="custom_li"
            >MATEMATYKA W OTACZAJĄCYM NAS ŚWIECIE 1 PODSTAWA</li>
            <li
             
              class="custom_li"
            >Czas na geografię Podręcznik Zakres podstawowy</li>
            <li
              
              class="custom_li"
            >POZNAĆ PRZESZŁOŚĆ WIEK XX PODRĘCZNIK NOWA ERA</li>

          
          </ul>
        </div>
        <div
          class="box_custom"
        >
          <p>Klaudia Arcikiewicz</p>
          <ul class="custom_ul">
            <li
             
              class="custom_li"
            >POZNAĆ PRZESZŁOŚĆ WIEK XX PODRĘCZNIK NOWA ERA</li>
            <li
      
              class="custom_li"
            >Krok w przedsiębiorczość Podręcznik</li>
            <li  class="custom_li">Oblicza geografii</li>
            <li class="custom_li">To jest chemia</li>
            <li class="custom_li">Biologia na czasie</li>
            <li  class="custom_li">W centrum uwagi</li>
            <li
            
              class="custom_li"
            >Spotkania z kulturą podręcznik Liceum i technikum</li>
            <li  class="custom_li">PONAD SŁOWAMI 1.2 NOWA ERA</li>
            <li
              
              class="custom_li"
            >Świat fizyki Podręcznik. Zakres podstawowy</li>
          </ul>
          <p>9</p>
        </div>

        <div
          class="box_custom"
        >
          <p>Radosław rakowski</p>
          <ul class="custom_ul">
            <li
              class="custom_li"
            >Krok w przedsiębiorczość Podręcznik</li>
            <li class="custom_li">Oblicza geografii</li>
            <li  class="custom_li">To jest chemia</li>
            <li  class="custom_li">Biologia na czasie</li>
            <li  class="custom_li">W centrum uwagi</li>
            <li
              
              class="custom_li"
            >Spotkania z kulturą podręcznik Liceum i technikum</li>
            <li class="custom_li">PONAD SŁOWAMI 1.2 NOWA ERA</li>
          </ul>
          <p>7</p>
        </div>

        <div
      
          class="box_custom"
        >
          <p>Sylwia szyszko</p>
          <ul class="custom_ul">
            <li  class="custom_li">Oblicza geografii</li>
            <li  class="custom_li">Biologia na czasie</li>
            <li  class="custom_li">To jest chemia</li>
            <li  class="custom_li">W centrum uwagi</li>
            <li
             
              class="custom_li"
            >POZNAĆ PRZESZŁOŚĆ WIEK XX PODRĘCZNIK NOWA ERA</li>
            <li
           
              class="custom_li"
            >Fizyka - ODKRYĆ FIZYKĘ - Nowa Era - podstawowy</li>
          </ul>
          <p>6</p>
        </div>


        <div
         
          class="box_custom"
        >
          <p>Piotrek Dąbrowski</p>
          <ul class="custom_ul">
            <li
             
              class="custom_li"
            >Krok w przedsiębiorczość Podręcznik</li>
            <li
             
              class="custom_li"
            >Świat fizyki Podręcznik. Zakres podstawowy</li>
            <li  class="custom_li">Biologia na czasie</li>
            <li  class="custom_li">W centrum uwagi</li>
            <li
           
              class="custom_li"
            >Spotkania z kulturą podręcznik Liceum i technikum</li>
            <li
       
              class="custom_li"
            >POZNAĆ PRZESZŁOŚĆ WIEK XX PODRĘCZNIK NOWA ERA</li>
          </ul>
          <p>6</p>
        </div>

        <div
        
          class="box_custom"
        >
          <p>zuzanna jedrzejewska</p>
          <ul class="custom_ul">
            <li
           
              class="custom_li"
            >POZNAĆ PRZESZŁOŚĆ WIEK XX PODRĘCZNIK NOWA ERA</li>
            <li class="custom_li">Oblicza geografii</li>
            <li class="custom_li">To jest chemia</li>
            <li  class="custom_li">Biologia na czasie</li>
            <li
             
              class="custom_li"
            >Fizyka - ODKRYĆ FIZYKĘ - Nowa Era - podstawowy</li>
            <li
              
              class="custom_li"
            >Świat fizyki Podręcznik. Zakres podstawowy</li>
          </ul>
          <p>6</p>
        </div>

        <div
         
          class="box_custom"
        >
          <p>Piotrek Dąbrowski</p>
          <ul class="custom_ul">
            <li
              
              class="custom_li"
            >Krok w przedsiębiorczość Podręcznik</li>
            <li  class="custom_li">Biologia na czasie</li>
            <li  class="custom_li">W centrum uwagi</li>
            <li
              
              class="custom_li"
            >Spotkania z kulturą podręcznik Liceum i technikum</li>
            <li
              
              class="custom_li"
            >Język polski Świat do przeczytania cz.1</li>
            <li class="custom_li">To jest chemia</li>
          </ul>
          <p>6</p>
        </div>

        <div
    
          class="box_custom"
        >
          <p>Klaudia Karłowska</p>
          <ul class="custom_ul">
            <li  class="custom_li">Oblicza geografii</li>
            <li  class="custom_li">Biologia na czasie</li>
            <li  class="custom_li">To jest chemia</li>
            <li  class="custom_li">Czas na geografię</li>
            <li
              
              class="custom_li"
            >POZNAĆ PRZESZŁOŚĆ WIEK XX PODRĘCZNIK NOWA ERA</li>
          </ul>
          <p>5</p>
        </div>

        <div

          class="box_custom"
        >
          <p>Magda magdalena Kamińska</p>
          <ul class="custom_ul">
            <li
             
              class="custom_li"
            >Krok w przedsiębiorczość Podręcznik</li>
            <li  class="custom_li">To jest chemia</li>
            <li  class="custom_li">W centrum uwagi</li>
          </ul>
          <p>2</p>
        </div>

        <!-- tutaj dodajesz nowych sprzedawców -->
        <!-- tutaj dodajesz nowych sprzedawców -->
        <!-- tutaj dodajesz nowych sprzedawców -->
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
  return {
    book: [

     {urlimg:'https://a.allegroimg.com/s360/03381c/226a37c7453cb051fc1cb466397b',
     tittle:'Krok w przedsiębiorczość Podręcznik'},
        
     {urlimg:   'https://a.allegroimg.com/s360/03c64b/0e1ff22f4c8aadd1496f585c6c6f',
     tittle:'To jest chemia Podręcznik + CD Zakres podstawowy' },
        
     {urlimg:  'https://e.allegroimg.com/s360/031e42/e57bbf3c418bb2253e3d4c02bf9e',
     tittle:' Fizyka - ODKRYĆ FIZYKĘ - Nowa Era - podstawowy' },
          
     {urlimg:   'https://4.allegroimg.com/s360/03b874/dd67a6254d81afcf3026e859b634',
     tittle:'Oblicza geografii'},
        
     {urlimg:  'https://7.allegroimg.com/s360/03fabd/d16f3ff247328422989b421c46f7'
    ,tittle:'Biologia na czasie'},
        
     {urlimg:'https://a.allegroimg.com/s360/03d23a/da5f8a8241919fde5b2b31a2f01d'
    ,tittle:'Spotkania z kulturą podręcznik Liceum i technikum'},
        
     {urlimg:  'https://c.allegroimg.com/s360/03385f/696aeb78425b9e9cf19d2dc0d96c '
    ,tittle:'W centrum uwagi'},
        
     {urlimg:  'https://6.allegroimg.com/s360/03057a/16b389f241f9b556416f607c8306 '
     ,tittle:'Ponad słowami podręcznik klasa 1 CZ. 1 NOWA ERA'},
        
     {urlimg:  'https://a.allegroimg.com/s360/0385bd/90d9dae842e38c2afde514766cfa '
     ,tittle:'Informatyka Europejczyka Podręcznik z płytą CD'},
        
     {urlimg:  'https://a.allegroimg.com/s360/03cb39/784c6d604149a34f395a3c14b1e9 '
     ,tittle:'Świat fizyki Podręcznik. Zakres podstawowy'},

     {urlimg: 'https://8.allegroimg.com/s360/031bf4/4b7fe93c447bb3b24a160be81cb8 '
    ,tittle:'Wiedza o kulturze SPOTKANIA Z KULTURĄ Podręcznik'},

     {urlimg:  'https://a.allegroimg.com/s360/034836/84528bff420dbaf631ddfaa60793 '
    ,tittle:'Język polski Świat do przeczytania cz.1'},
        
     {urlimg:  'https://a.allegroimg.com/s360/03743d/bb43213045a7b7be819c312a2d12 '
     ,tittle:'PONAD SŁOWAMI 1.2 NOWA ERA'},

    {urlimg:  'https://a.allegroimg.com/s360/03a902/f42a3f3d497c9a36c9228ed3a2a7 '
    ,tittle:'Matematyka 1. Zakres podstawowy i rozszerzony'},
        
     {urlimg:  'https://a.allegroimg.com/s360/038caf/3d01e4334207a0d4abab32f05576 '
     ,tittle:'Informatyka Europejczyka Zakres podstawowy Podr.'},
        
     {urlimg:  'https://e.allegroimg.com/s360/03adbb/a8f0d92142e585e3e9ce1449c41e '
     ,tittle:'MATEMATYKA W OTACZAJĄCYM NAS ŚWIECIE 1 PODSTAWA'},
     {urlimg:  'https://a.allegroimg.com/s360/03ccae/e3f6bd3147b98247f8bddb3ab1bb '
     ,tittle:'Czas na geografię Podręcznik Zakres podstawowy'},
        
     {urlimg:  'https://5.allegroimg.com/s360/03b1e2/3c474d744d908b543e20515bce25 '
     ,tittle:'Poznać przeszłość Wiek XX Podręcznik'},
     ]
    }
  },
};
</script>
<style>
.search_selection {
  height: 100%;
  width: 100vw;
  background-color: #eceff1;
  padding: 15px 100px;
   display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
.selection_bookbox{
  height: 180px;
  width: 180px;
  background-color: rgb(221, 221, 221);
}
.bookbox_img{
  height: 180px;
  width: 180px;
}
/* customers */
/* customers */
/* customers */

.search_customers {
  background-color: #eceff1;
}

.customers_tittle {
  padding: 10px;
  width: 99vw;
  height: 75px;
  background-color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  border: 1px solid rgb(221, 221, 221);
}
.customers_box {
  padding: 20px 100px 100px 100px;
}
.box_custom {
  display: none;
  justify-content: space-between;
  align-items: center;
  background-color: white;
  padding: 15px;
  border: 1px solid rgb(221, 221, 221);
  margin-bottom: 5px;
  cursor: pointer;
}
.box_custom:first-of-type {
  display: flex;
}
.custom_ul {
  display: flex;
  flex-wrap: wrap;
  max-width: 67vw;
}
.custom_li {
  list-style: none;
  margin: 5px;
  border: 1px solid rgb(221, 221, 221);
  padding: 5px;
}

  /* active class */
  /* active class */
  /* active class */


.active_li {
  border: 1px solid #16cae6;
  background-color: #16cae659;
}
.box_bookactive {
  background-color: yellow;
  border: none;
}

/* change this */
/* change this */
/* change this */

.box_customactive0 {
  display: flex;
}
.box_customactive1 {
  display: flex;
}
.box_customactive2 {
  display: flex;
}
.box_customactive3 {
  display: flex;
}
.box_customactive4 {
  display: flex;
}
.box_customactive5 {
  display: flex;
}
.box_customactive6 {
  display: flex;
}
.box_customactive7 {
  display: flex;
}
.box_customactive8 {
  display: flex;
}
.box_customactive9 {
  display: flex;
}
.box_customactive10 {
  display: flex;
}
</style>