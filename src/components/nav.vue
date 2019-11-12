<template>
  <nav class="nav">
    <h2>Wybierz ksiażki</h2>
    <div @click="addSwitch += 1" class="nav_addnewsell-btn">Dodaj nowego sprzedawce</div>

    <div v-if="addSwitch == 1" class="add">
      <div class="add_content">
        <div class="add_tittle">
          <h2>Jak dodać?</h2>
        </div>

        <div> <p>Umieść kod w 200 linijce kodu po komentarzem</p> 
        <p class="red">Uwaga nie da się usunąć już wybranej ksiązki trzeba oswiezyc </p></div>

        <div @click="addSwitch -= 1" class="add_close"></div>

        <div class="add_generator">
          <textarea name id cols="30" rows="10">

          
            <div
          v-bind:class='{{ start + bookShow + end}}'
          class="box_custom"
        >
          <p>{{name}}</p>
          <ul class="custom_ul">
           
            {{bookList}}
          </ul>
          <p>{{manyBook}}</p>
        </div>

        </textarea>
          <div class="add_inputbox">
            <input v-model="name" type="text" />

            <ul>
              <li
                id="kwp"
                :class="{ add_active : kwp >= 1 }"
                @click="addBook('kwp')"
                class="add_inputbox_li"
              >Krok w przedsiębiorczość Podręcznik</li>

              <li
                id="tjc"
                :class="{ add_active : tjc >= 1 }"
                @click="addBook('tjc')"
                class="add_inputbox_li"
              >To jest chemia</li>

              <li
                id="fof"
                :class="{ add_active : fof >= 1 }"
                @click="addBook('fof')"
                class="add_inputbox_li"
              >Fizyka - ODKRYĆ FIZYKĘ - Nowa Era - podstawowy</li>

              <li
                id="og"
                :class="{ add_active : og >= 1 }"
                @click="addBook('og')"
                class="add_inputbox_li"
              >Oblicza geografii</li>

              <li
                id="bnc"
                :class="{ add_active : bnc >= 1 }"
                @click="addBook('bnc')"
                class="add_inputbox_li"
              >Biologia na czasie</li>

              <li
                id="szk"
                :class="{ add_active : szk >= 1 }"
                @click="addBook('szk')"
                class="add_inputbox_li"
              >Spotkania z kulturą podręcznik Liceum i technikum</li>

              <li
                id="ps"
                :class="{ add_active : ps >= 1 }"
                @click="addBook('ps')"
                class="add_inputbox_li"
              >Ponad słowami podręcznik klasa 1 CZ. 1 NOWA ERA</li>

              <li
                id="wcu"
                :class="{ add_active : wcu >= 1 }"
                @click="addBook('wcu')"
                class="add_inputbox_li"
              >W centrum uwagi</li>

              <li
                id="sf"
                :class="{ add_active : sf >= 1 }"
                @click="addBook('sf')"
                class="add_inputbox_li"
              >Świat fizyki Podręcznik. Zakres podstawowy</li>

              <li
                id="wok"
                :class="{ add_active : wok >= 1 }"
                @click="addBook('wok')"
                class="add_inputbox_li"
              >Język polski Świat do przeczytania cz.2</li>

              <li
                id="jps"
                :class="{ add_active : jps >= 1 }"
                @click="addBook('jps')"
                class="add_inputbox_li"
              >Język polski Świat do przeczytania cz.1</li>

              <li
                id="ps1"
                :class="{ add_active : ps1 >= 1 }"
                @click="addBook('ps1')"
                class="add_inputbox_li"
              >PONAD SŁOWAMI 1.2 NOWA ERA</li>

              <li
                id="m1"
                :class="{ add_active : m1 >= 1 }"
                @click="addBook('m1')"
                class="add_inputbox_li"
              >Matematyka 1. Zakres podstawowy i rozszerzony</li>

              <li
                id="ie"
                :class="{ add_active : ie >= 1 }"
                @click="addBook('ie')"
                class="add_inputbox_li"
              >Informatyka Europejczyka Zakres podstawowy Podr.</li>

              <li
                id="mwo"
                :class="{ add_active : mwo >= 1 }"
                @click="addBook('mwo')"
                class="add_inputbox_li"
              >MATEMATYKA W OTACZAJĄCYM NAS ŚWIECIE 1 PODSTAWA</li>

              <li
                id="cng"
                :class="{ add_active : cng >= 1 }"
                @click="addBook('cng')"
                class="add_inputbox_li"
              >Czas na geografię Podręcznik Zakres podstawowy</li>

              <li
                id="pp"
                :class="{ add_active : pp >= 1 }"
                @click="addBook('pp')"
                class="add_inputbox_li"
              >POZNAĆ PRZESZŁOŚĆ WIEK XX PODRĘCZNIK NOWA ERA</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>
<script>
export default {
};
</script>
<style>
.nav {
  width: 99vw;
  height: 75px;
  background-color: white;
  display: flex;
  align-items: center;
  justify-content: space-around;
  border-bottom: 1px solid rgb(221, 221, 221);
}

.nav_addnewsell-btn {
  height: 32.5px;
  padding: 10px;
  border-radius: 3px;
  border: 1px solid rgb(199, 199, 199);
  background-color: rgb(246, 246, 246);
  display: flex;
  align-items: center;
  text-align: center;
  cursor: pointer;
}

.add {
  position: fixed;
  top: 0;
  left: 0;
  height: 100vh;
  width: 100vw;
  background-color: rgba(0, 0, 0, 0.479);
  z-index: 5;
  display: flex;
  justify-content: center;
  align-items: center;
}
.add_content {
  padding-top: 100px;
  position: relative;
  background-color: rgb(223, 223, 223);
  width: 70vw;
  height: 90vh;
  border-radius: 10px;
}
.add_tittle {
  border-radius: 10px 10px 0 0;
  width: 100%;
  height: 50px;
  background-color: white;
  position: absolute;
  top: 0;
  left: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  border-bottom: 1px solid rgb(221, 221, 221);
}
.add_generator{
height: 380px;
  display: flex;
    width: 70vw;
  align-items: center;
  justify-content: center;
  }
.add_generator > textarea {
  height: 310px;
  width: 300px;
margin-right: 50px;
  border: none;
}
.add_inputbox {
  text-align: left;
  list-style: none;
  width: 300px;
}
.add_inputbox > input {
  height: 35px;
  width: 300px;
  text-align: center;
  border-radius: 2px;
  border: none;
}
.add_inputbox > ul {
  margin-top: 15px;
  height: 260px;
  overflow-y: scroll;
  list-style: none;
}
.add_inputbox_li {
  padding: 5px;
  background-color: white;
  cursor: pointer;
}

.add_close {
  position: absolute;
  top: 10px;
  right: 15px;
  height: 25px;
  width: 25px;
  opacity: 0.9;
  cursor: pointer;
}
.add_close:hover {
  opacity: 1;
}
.add_close:before,
.add_close:after {
  position: absolute;
  left: 15px;
  content: " ";
  height: 28px;
  width: 3px;
  background-color: #333;
}
.add_close:before {
  transform: rotate(45deg);
}
.add_close:after {
  transform: rotate(-45deg);
}

/* active */
/* active */
/* active */
.red{
  margin-top: 2px;
  color: rgba(255, 0, 0, 0.76);
}
.add_active {
  border: 1px solid #16cae6;
  background-color: #16cae659;
}
</style>