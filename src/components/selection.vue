<template>
  <div>
    <div class="search_selection">
      <div  v-bind:id="item.id" :key="item.id"  v-for="(item) in book" class="selection_bookbox">
        <img v-on:click="checkBook" class="bookbox_img" v-bind:src="item.url" alt="">
        <p v-on:click="checkBook" class="bookbox_tittle">{{item.tittle}}</p>
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
      </div>
    </div>
</template>
<script>
export default {
  data() {
  return {
    // books
    // books
    // books
    book: [
     {id:'kwk',
     url:'https://a.allegroimg.com/s360/03381c/226a37c7453cb051fc1cb466397b',
     tittle:'Krok w przedsiębiorczość Podręcznik'},
        
     {id:'tj',url:   'https://a.allegroimg.com/s360/03c64b/0e1ff22f4c8aadd1496f585c6c6f',
     tittle:'To jest chemia Podręcznik + CD Zakres podstawowy' },
        
     {id:'fof',url:  'https://e.allegroimg.com/s360/031e42/e57bbf3c418bb2253e3d4c02bf9e',
     tittle:' Fizyka - ODKRYĆ FIZYKĘ - Nowa Era - podstawowy' },
          
     {id:'og',url:   'https://4.allegroimg.com/s360/03b874/dd67a6254d81afcf3026e859b634',
     tittle:'Oblicza geografii'},
        
     {id:'bnc',url:  'https://7.allegroimg.com/s360/03fabd/d16f3ff247328422989b421c46f7'
    ,tittle:'Biologia na czasie'},
        
     {id:'szk',url:'https://a.allegroimg.com/s360/03d23a/da5f8a8241919fde5b2b31a2f01d'
    ,tittle:'Spotkania z kulturą podręcznik Liceum i technikum'},
        
     {id:'wcu',url:  'https://c.allegroimg.com/s360/03385f/696aeb78425b9e9cf19d2dc0d96c '
    ,tittle:'W centrum uwagi'},
        
     {id:'pns',url:  'https://6.allegroimg.com/s360/03057a/16b389f241f9b556416f607c8306 '
     ,tittle:'Ponad słowami podręcznik klasa 1 CZ. 1 NOWA ERA'},
        
     {id:'ie',url:  'https://a.allegroimg.com/s360/0385bd/90d9dae842e38c2afde514766cfa '
     ,tittle:'Informatyka Europejczyka Podręcznik z płytą CD'},
        
     {id:'sf',url:  'https://a.allegroimg.com/s360/03cb39/784c6d604149a34f395a3c14b1e9 '
     ,tittle:'Świat fizyki Podręcznik. Zakres podstawowy'},

     {id:'wok',url: 'https://8.allegroimg.com/s360/031bf4/4b7fe93c447bb3b24a160be81cb8 '
    ,tittle:'Wiedza o kulturze SPOTKANIA Z KULTURĄ Podręcznik'},

     {id:'jps',url:  'https://a.allegroimg.com/s360/034836/84528bff420dbaf631ddfaa60793 '
    ,tittle:'Język polski Świat do przeczytania cz.1'},
        
     {id:'pn',url:  'https://a.allegroimg.com/s360/03743d/bb43213045a7b7be819c312a2d12 '
     ,tittle:'PONAD SŁOWAMI 1.2 NOWA ERA'},

    {id:'m1',url:  'https://a.allegroimg.com/s360/03a902/f42a3f3d497c9a36c9228ed3a2a7 '
    ,tittle:'Matematyka 1. Zakres podstawowy i rozszerzony'},
        
     {id:'iez',url: 'https://a.allegroimg.com/s360/038caf/3d01e4334207a0d4abab32f05576 '
     ,tittle:'Informatyka Europejczyka Zakres podstawowy Podr.'},
        
     {id:'mot' ,url:  'https://e.allegroimg.com/s360/03adbb/a8f0d92142e585e3e9ce1449c41e '
     ,tittle:'MATEMATYKA W OTACZAJĄCYM NAS ŚWIECIE 1 PODSTAWA'},
     {id:'cng',url:  'https://a.allegroimg.com/s360/03ccae/e3f6bd3147b98247f8bddb3ab1bb '
     ,tittle:'Czas na geografię Podręcznik Zakres podstawowy'},
        
     {id:' pp',url:  'https://5.allegroimg.com/s360/03b1e2/3c474d744d908b543e20515bce25 '
     ,tittle:'Poznać przeszłość Wiek XX Podręcznik'},
     ],



    user:[
      {name:'Klaudia Arcikiewicz', 
      book:'',
      }
     ]

  }
    },
    methods: {
      checkBook: function(e) {
      e.target.parentElement.style.boxShadow = "0px 0px 35px blue";
      const current = e.target.parentElement.textContent
      console.log('current:  ' +current)
      const li = [...document.querySelectorAll('.custom_li')]
       let result = li;
       result = result.filter(li => li.textContent.includes(current));
       console.log(result)
           for (let i = 0; i < result.length; i++) {
        var c = result[i];
        c.style.backgroundColor = "blue";
       let parent = c.parentElement 
       if(parent.parentElement.classList == 'box_custom'){
         parent.parentElement.style.display = 'flex';
       }
        console.log( parent.parentElement.classList )
      }
    },
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
  background-color: rgb(199, 199, 199);
  margin-top: 25px;
  margin-bottom: 25px;
  cursor: pointer;
}
.bookbox_img{
  width: auto;
  padding: 0px 40px;
  height:120px;
}
.bookbox_tittle{
  display:flex;
  justify-content: center;
  align-items: center;
  height: 60px;
  width: 180px;
  background-color: white;
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
  border: 1px solid rgb(180, 119, 119);
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

</style>