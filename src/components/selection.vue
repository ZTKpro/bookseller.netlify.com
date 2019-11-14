<template>
  <div>
    <div class="search_selection">
      <div  v-bind:id="item.id" :key="item.id"  v-for="item in books" class="selection_bookbox">
        <img v-on:click="checkBook" class="bookbox_img" v-bind:src="item.url" alt="">
        <p v-on:click="checkBook" class="bookbox_tittle">{{item.tittle}}</p>
      </div>
    </div>
    <div class="search_customers">
      <div class="customers_tittle">
        <h2>Sprzedający</h2>
      </div>
      <div class="customers_box">
          <ul  class="custom_ul">
            <li v-for="item in books" :key="item.id"  class="custom_li"> {{item.tittle}} </li>
          </ul>
        </div>



        <div  v-for="(items) in person" :key="items.id"  class="box_custom">
            <p>{{items.nick}}</p>
            <ul >
             <li class="custom_li">{{items.book}}</li>
             <li class="custom_li">{{items.book1}}</li>
             <li class="custom_li">{{items.book2}}</li>
             <li class="custom_li">{{items.book3}}</li>
             <li class="custom_li">{{items.book4}}</li>
             <li class="custom_li">{{items.book5}}</li>
             <li class="custom_li">{{items.book6}}</li>
             <li class="custom_li">{{items.book7}}</li>
             <li class="custom_li">{{items.book8}}</li>
            </ul>
        </div>
        <!-- <div
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
          
        </div> -->

       <!--  -->
      </div>
    </div>
</template>
<script>
import bookJson from './bookList.json'
import person1 from './user/userList.json'

export default {
    data() {
      return {
        books: bookJson,
        person: person1,
      }
    },
    methods: {
      checkBook: function(e) {
      const li = [...document.querySelectorAll('.custom_li')]
        const current = e.target.parentElement.textContent
        let result = li;
        console.log(result[1].textContent)

        result = result.filter(li => li.textContent.includes(current));
        
        for (let i = 0; i < result.length; i++) {
          let c = result[i];
          c.style.backgroundColor = "blue";
          let parent = c.parentElement 
          if(parent.parentElement.classList == 'box_custom'){
            parent.parentElement.style.display = 'flex';
          }
        }
        this.addBoxShadow(e)
      },
      addBoxShadow: function(e){
      e.target.parentElement.style.boxShadow = "0px 0px 35px blue";
      },
      deletedCustom: function(){
        const li = [...document.querySelectorAll('.custom_li')]
        let result = li;
        console.log(result)
        for (let i = 0; i < result.length; i++) {
          let c = result[i];
          console.log(c.textContent)
          if(c.textContent == ''){
           c.style.display = "none";
          }
        }
      },
    },
    mounted: function() {
      this.deletedCustom()
    }
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