<template>
  <div>
    <div class="search_selection">
      <div class="selection_box">
        <div :class="{ box_bookactive : kwp = kwp % 2 }" @click="kwp += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://a.allegroimg.com/s360/03381c/226a37c7453cb051fc1cb466397b" alt />
          </div>
          <p>Krok w przedsiębiorczość Podręcznik</p>
        </div>
        <div :class="{ box_bookactive : tjc = tjc % 2 }" @click="tjc += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://a.allegroimg.com/s360/03c64b/0e1ff22f4c8aadd1496f585c6c6f" alt />
          </div>
          <p>To jest chemia Podręcznik + CD Zakres podstawowy</p>
        </div>
        <div :class="{ box_bookactive : fof = fof % 2 }" @click="fof += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://e.allegroimg.com/s360/031e42/e57bbf3c418bb2253e3d4c02bf9e" alt />
          </div>
          <p>Fizyka - ODKRYĆ FIZYKĘ - Nowa Era - podstawowy</p>
        </div>
        <div :class="{ box_bookactive : og = og % 2 }" @click="og += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://4.allegroimg.com/s360/03b874/dd67a6254d81afcf3026e859b634" alt />
          </div>
          <p>Oblicza geografii</p>
        </div>
        <div :class="{ box_bookactive : bnc = bnc % 2 }" @click="bnc += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://7.allegroimg.com/s360/03fabd/d16f3ff247328422989b421c46f7" alt />
          </div>
          <p>Biologia na czasie</p>
        </div>
        <div :class="{ box_bookactive : szk = szk % 2 }" @click="szk+= 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://a.allegroimg.com/s360/03d23a/da5f8a8241919fde5b2b31a2f01d" alt />
          </div>
          <p>Spotkania z kulturą podręcznik Liceum i technikum</p>
        </div>
        <div :class="{ box_bookactive : wcu = wcu % 2 }" @click="wcu += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://c.allegroimg.com/s360/03385f/696aeb78425b9e9cf19d2dc0d96c" alt />
          </div>
          <p>W centrum uwagi</p>
        </div>
        <div :class="{ box_bookactive : ps = ps % 2 }" @click="ps += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://6.allegroimg.com/s360/03057a/16b389f241f9b556416f607c8306" alt />
          </div>
          <p>Ponad słowami podręcznik klasa 1 CZ. 1 NOWA ERA</p>
        </div>
        <div :class="{ box_bookactive : ie = ie % 2 }" @click="ie += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://a.allegroimg.com/s360/0385bd/90d9dae842e38c2afde514766cfa" alt />
          </div>
          <p>Informatyka Europejczyka Podręcznik z płytą CD</p>
        </div>
        <div :class="{ box_bookactive : sf = sf % 2 }" @click="sf += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://a.allegroimg.com/s360/03cb39/784c6d604149a34f395a3c14b1e9" alt />
          </div>
          <p>Świat fizyki Podręcznik. Zakres podstawowy</p>
        </div>
        <div :class="{ box_bookactive : wok = wok % 2 }" @click="wok += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://8.allegroimg.com/s360/031bf4/4b7fe93c447bb3b24a160be81cb8" alt />
          </div>
          <p>Wiedza o kulturze SPOTKANIA Z KULTURĄ Podręcznik</p>
        </div>
        <div :class="{ box_bookactive : jps = jps % 2 }" @click="jps += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://a.allegroimg.com/s360/034836/84528bff420dbaf631ddfaa60793" alt />
          </div>
          <p>Język polski Świat do przeczytania cz.1</p>
        </div>
        <div :class="{ box_bookactive : ps1 = ps1 % 2 }" @click="ps1 += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://a.allegroimg.com/s360/03743d/bb43213045a7b7be819c312a2d12" alt />
          </div>
          <p>PONAD SŁOWAMI 1.2 NOWA ERA</p>
        </div>
        <div :class="{ box_bookactive : m1 = m1 % 2 }" @click="m1 += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://a.allegroimg.com/s360/03a902/f42a3f3d497c9a36c9228ed3a2a7" alt />
          </div>
          <p>Matematyka 1. Zakres podstawowy i rozszerzony</p>
        </div>
        <div :class="{ box_bookactive : iez = iez % 2 }" @click="iez += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://a.allegroimg.com/s360/038caf/3d01e4334207a0d4abab32f05576" alt />
          </div>
          <p>Informatyka Europejczyka Zakres podstawowy Podr.</p>
        </div>
        <div :class="{ box_bookactive : mwo = mwo % 2 }" @click="mwo += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://e.allegroimg.com/s360/03adbb/a8f0d92142e585e3e9ce1449c41e" alt />
          </div>
          <p>MATEMATYKA W OTACZAJĄCYM NAS ŚWIECIE 1 PODSTAWA</p>
        </div>
        <div :class="{ box_bookactive : cng = cng % 2 }" @click="cng += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://a.allegroimg.com/s360/03ccae/e3f6bd3147b98247f8bddb3ab1bb" alt />
          </div>
          <p>Czas na geografię Podręcznik Zakres podstawowy</p>
        </div>
        <div :class="{ box_bookactive : pp = pp % 2 }" @click="pp += 1" class="box_book">
          <div class="book_imgwrap">
            <img src="https://5.allegroimg.com/s360/03b1e2/3c474d744d908b543e20515bce25" alt />
          </div>
          <p>Poznać przeszłość Wiek XX Podręcznik</p>
        </div>
      </div>
    </div>
    <div class="search_customers">
      <div class="customers_tittle">
        <h2>Sprzedający</h2>
      </div>
      <div class="customers_box">
        <div class="box_custom">
          <ul class="custom_bookbox">
            <li
              :class="{  active_li : kwp = kwp % 2 }"
              class="custom_book"
            >Krok w przedsiębiorczość Podręcznik</li>
            <li :class="{  active_li : tjc = tjc % 2 }" class="custom_book">To jest chemia</li>
            <li
              :class="{  active_li : fof = fof % 2 }"
              class="custom_book"
            >Fizyka - ODKRYĆ FIZYKĘ - Nowa Era - podstawowy</li>
            <li :class="{  active_li : og = og % 2 }" class="custom_book">Oblicza geografii</li>
            <li :class="{  active_li : bnc = bnc % 2 }" class="custom_book">Biologia na czasie</li>
            <li
              :class="{  active_li : szk = szk % 2 }"
              class="custom_book"
            >Spotkania z kulturą podręcznik Liceum i technikum</li>
            <li
              :class="{  active_li : ps = ps % 2 }"
              class="custom_book"
            >Ponad słowami podręcznik klasa 1 CZ. 1 NOWA ERA</li>
            <li
              :class="{  active_li : ie = ie % 2 }"
              class="custom_book"
            >Informatyka Europejczyka Podręcznik z płytą CD</li>
            <li :class="{  active_li : wcu = wcu % 2 }" class="custom_book">W centrum uwagi</li>
            <li
              :class="{  active_li : sf = sf % 2 }"
              class="custom_book"
            >Świat fizyki Podręcznik. Zakres podstawowy</li>
            <li
              :class="{  active_li : wok = wok % 2 }"
              class="custom_book"
            >Wiedza o kulturze SPOTKANIA Z KULTURĄ Podręcznik</li>
            <li
              :class="{  active_li : jps = jps % 2 }"
              class="custom_book"
            >Język polski Świat do przeczytania cz.1</li>
            <li
              :class="{  active_li : ps1 = ps1 % 2 }"
              class="custom_book"
            >PONAD SŁOWAMI 1.2 NOWA ERA</li>
            <li
              :class="{  active_li : m1 = m1 % 2 }"
              class="custom_book"
            >Matematyka 1. Zakres podstawowy i rozszerzony</li>
            <li
              :class="{  active_li : iez = iez % 2 }"
              class="custom_book"
            >Informatyka Europejczyka Zakres podstawowy Podr.</li>
            <li
              :class="{  active_li : mwo = mwo % 2 }"
              class="custom_book"
            >MATEMATYKA W OTACZAJĄCYM NAS ŚWIECIE 1 PODSTAWA</li>
            <li
              :class="{  active_li : cng = cng % 2 }"
              class="custom_book"
            >Czas na geografię Podręcznik Zakres podstawowy</li>
            <li
              :class="{  active_li : pp = pp % 2 }"
              class="custom_book"
            >POZNAĆ PRZESZŁOŚĆ WIEK XX PODRĘCZNIK NOWA ERA</li>
            <!-- nowe ksiazki -->
            <!-- nowe ksiazki -->
            <!-- nowe ksiazki -->
            <!-- nowe ksiazki -->
          </ul>
        </div>

        <!-- Nowi uzytkownicy  -->
        <!-- Nowi uzytkownicy  -->
        <!-- Nowi uzytkownicy  -->
        <!-- Nowi uzytkownicy  -->
        <!-- Nowi uzytkownicy  -->

        <div
          :class="{ box_customactive  : tjc = tjc % 2,box_customactive1 : kwp = kwp % 2,box_customactive2 : wcu = wcu % 2  }"
          class="box_custom"
        >
          <p>Magda magdalena Kamińska</p>
          <ul class="custom_bookbox">
            <li
              :class="{  active_li : kwp = kwp % 2 }"
              class="custom_book"
            >Krok w przedsiębiorczość Podręcznik</li>
            <li :class="{  active_li : tjc = tjc % 2 }" class="custom_book">To jest chemia</li>
            <li :class="{  active_li : wcu = wcu % 2 }" class="custom_book">W centrum uwagi</li>
          </ul>
        </div>

        <div
          :class="{ box_customactive  : bnc = bnc % 2,box_customactive1 : og = og % 2,box_customactive2 : tjc = tjc % 2,box_customactive3 : pp = pp % 2,box_customactive3 : cng = cng % 2  }"
          class="box_custom"
        >
          <p>Klaudia Karłowska</p>
          <ul class="custom_bookbox">
            <li :class="{  active_li : og = og % 2 }" class="custom_book">Oblicza geografii</li>
            <li :class="{  active_li : bnc = bnc % 2 }" class="custom_book">Biologia na czasie</li>
            <li :class="{  active_li : tjc = tjc % 2 }" class="custom_book">To jest chemia</li>
            <li :class="{  active_li : cng = cng % 2 }" class="custom_book">Czas na geografię</li>
            <li
              :class="{  active_li : pp = pp % 2 }"
              class="custom_book"
            >POZNAĆ PRZESZŁOŚĆ WIEK XX PODRĘCZNIK NOWA ERA</li>
          </ul>
        </div>

        <div
          :class="{ box_customactive  : bnc = bnc % 2,box_customactive1 : og = og % 2,box_customactive2 : tjc = tjc % 2,box_customactive3 : pp = pp % 2,box_customactive4 : wcu = wcu % 2 }"
          class="box_custom"
        >
          <p>Sylwia szyszko</p>
          <ul class="custom_bookbox">
            <li :class="{  active_li : og = og % 2 }" class="custom_book">Oblicza geografii</li>
            <li :class="{  active_li : bnc = bnc % 2 }" class="custom_book">Biologia na czasie</li>
            <li :class="{  active_li : tjc = tjc % 2 }" class="custom_book">To jest chemia</li>
            <li :class="{  active_li : wcu = wcu % 2 }" class="custom_book">W centrum uwagi</li>
            <li
              :class="{  active_li : pp = pp % 2 }"
              class="custom_book"
            >POZNAĆ PRZESZŁOŚĆ WIEK XX PODRĘCZNIK NOWA ERA</li>
            <li
              :class="{  active_li : fof = fof % 2 }"
              class="custom_book"
            >Fizyka - ODKRYĆ FIZYKĘ - Nowa Era - podstawowy</li>
          </ul>
        </div>

        <div
          :class="{ box_customactive  : bnc = bnc % 2,box_customactive1 : og = og % 2,box_customactive2 : tjc = tjc % 2,box_customactive3 : pp = pp % 2,box_customactive4 : sf = sf % 2,box_customactive5 : fof = fof % 2  }"
          class="box_custom"
        >
          <p>zuzanna jedrzejewska</p>
          <ul class="custom_bookbox">
            <li
              :class="{  active_li : pp = pp % 2 }"
              class="custom_book"
            >POZNAĆ PRZESZŁOŚĆ WIEK XX PODRĘCZNIK NOWA ERA</li>
            <li :class="{  active_li : og = og % 2 }" class="custom_book">Oblicza geografii</li>
            <li :class="{  active_li : tjc = tjc % 2 }" class="custom_book">To jest chemia</li>
            <li :class="{  active_li : bnc = bnc % 2 }" class="custom_book">Biologia na czasie</li>
            <li
              :class="{  active_li : fof = fof % 2 }"
              class="custom_book"
            >Fizyka - ODKRYĆ FIZYKĘ - Nowa Era - podstawowy</li>
            <li
              :class="{  active_li : sf = sf % 2 }"
              class="custom_book"
            >Świat fizyki Podręcznik. Zakres podstawowy</li>
          </ul>
        </div>

        <div
          :class="{ box_customactive  : bnc = bnc % 2,box_customactive1 : og = og % 2,box_customactive2 : tjc = tjc % 2,box_customactive3 : pp = pp % 2,box_customactive4 : sf = sf % 2,box_customactive5 : kwp = kwp % 2,box_customactive6 : wcu = wcu % 2,box_customactive7 : ps = ps % 2 }"
          class="box_custom"
        >
          <p>Klaudia Arcikiewicz</p>
          <ul class="custom_bookbox">
            <li
              :class="{  active_li : pp = pp % 2 }"
              class="custom_book"
            >POZNAĆ PRZESZŁOŚĆ WIEK XX PODRĘCZNIK NOWA ERA</li>
            <li
              :class="{  active_li : kwp = kwp % 2 }"
              class="custom_book"
            >Krok w przedsiębiorczość Podręcznik</li>
            <li :class="{  active_li : og = og % 2 }" class="custom_book">Oblicza geografii</li>
            <li :class="{  active_li : tjc = tjc % 2 }" class="custom_book">To jest chemia</li>
            <li :class="{  active_li : bnc = bnc % 2 }" class="custom_book">Biologia na czasie</li>
            <li :class="{  active_li : wcu = wcu % 2 }" class="custom_book">W centrum uwagi</li>
            <li :class="{  active_li : szk = szk % 2 }" class="custom_book">Spotkania z kulturą podręcznik Liceum i technikum</li>
            <li :class="{  active_li : ps = ps % 2 }" class="custom_book"> PONAD SŁOWAMI 1.2 NOWA ERA</li>
            <li
              :class="{  active_li : sf = sf % 2 }"
              class="custom_book"
            >Świat fizyki Podręcznik. Zakres podstawowy</li>
          </ul>
        </div>


        <div
          :class="{ box_customactive  : bnc = bnc % 2,box_customactive1 : og = og % 2,box_customactive2 : tjc = tjc % 2,box_customactive2 : ps = ps % 2,box_customactive5 : kwp = kwp % 2,box_customactive6 : wcu = wcu % 2,box_customactive7 : ps = ps % 2 }"
          class="box_custom"
        >
          <p>Radosław rakowski</p>
          <ul class="custom_bookbox">
              <li
                :class="{  active_li : kwp = kwp % 2 }"
                class="custom_book"
              >Krok w przedsiębiorczość Podręcznik</li>
              <li :class="{  active_li : og = og % 2 }" class="custom_book">Oblicza geografii</li>
              <li :class="{  active_li : tjc = tjc % 2 }" class="custom_book">To jest chemia</li>
              <li :class="{  active_li : bnc = bnc % 2 }" class="custom_book">Biologia na czasie</li>
              <li :class="{  active_li : wcu = wcu % 2 }" class="custom_book">W centrum uwagi</li>
              <li :class="{  active_li : szk = szk % 2 }" class="custom_book">Spotkania z kulturą podręcznik Liceum i technikum</li>
              <li :class="{  active_li : ps = ps % 2 }" class="custom_book"> PONAD SŁOWAMI 1.2 NOWA ERA</li>
            </ul>
        </div>

        <div
          :class="{ box_customactive  : bnc = bnc % 2,box_customactive2 : sf = sf % 2,box_customactive3 : pp = pp % 2,box_customactive5 : kwp = kwp % 2,box_customactive6 : wcu = wcu % 2,box_customactive7 : ps = ps % 2 }"
          class="box_custom"
        >
          <p>Piotrek Dąbrowski</p>
          <ul class="custom_bookbox">
            <li
              :class="{  active_li : kwp = kwp % 2 }"
              class="custom_book"
            >Krok w przedsiębiorczość Podręcznik</li>
              <li
              :class="{  active_li : sf = sf % 2 }"
              class="custom_book"
            >Świat fizyki Podręcznik. Zakres podstawowy</li>
            <li :class="{  active_li : bnc = bnc % 2 }" class="custom_book">Biologia na czasie</li>
            <li :class="{  active_li : wcu = wcu % 2 }" class="custom_book">W centrum uwagi</li>
            <li :class="{  active_li : szk = szk % 2 }" class="custom_book">Spotkania z kulturą podręcznik Liceum i technikum</li>
             <li
              :class="{  active_li : pp = pp % 2 }"
              class="custom_book"
            >POZNAĆ PRZESZŁOŚĆ WIEK XX PODRĘCZNIK NOWA ERA</li>
          </ul>
        </div>

        <div
          :class="{ box_customactive  : bnc = bnc % 2,box_customactive1  : jps = jps % 2,box_customactive2  : tjc = tjc % 2,box_customactive5 : kwp = kwp % 2,box_customactive6 : wcu = wcu % 2,box_customactive7 : ps = ps % 2 }"
          class="box_custom"
        >
          <p>Piotrek Dąbrowski</p>
          <ul class="custom_bookbox">
            <li
              :class="{  active_li : kwp = kwp % 2 }"
              class="custom_book"
            >Krok w przedsiębiorczość Podręcznik</li>
            <li :class="{  active_li : bnc = bnc % 2 }" class="custom_book">Biologia na czasie</li>
            <li :class="{  active_li : wcu = wcu % 2 }" class="custom_book">W centrum uwagi</li>
            <li :class="{  active_li : szk = szk % 2 }" class="custom_book">Spotkania z kulturą podręcznik Liceum i technikum</li>
            <li :class="{  active_li : jps = jps % 2 }" class="custom_book">Język polski Świat do przeczytania cz.1</li>
               <li :class="{  active_li : tjc = tjc % 2 }" class="custom_book">To jest chemia</li>
          </ul>
        </div>

        <!-- Nowi uzytkownicy  -->
        <!-- Nowi uzytkownicy  -->
        <!-- Nowi uzytkownicy  -->
        <!-- Nowi uzytkownicy  -->
        <!-- Nowi uzytkownicy  -->
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      bnc: 0,
      kwp: 0,
      tjc: 0,
      fof: 0,
      og: 0,
      szk: 0,
      wcu: 0,
      ps: 0,
      ie: 0,
      sf: 0,
      sok: 0,
      jps: 0,
      wok: 0,
      ps1: 0,
      m1: 0,
      iez: 0,
      mwo: 0,
      cng: 0,
      pp: 0
    };
  }
};
</script>
<style>
.search_selection {
  height: 100%;
  width: 100vw;
  background-color: #eceff1;
}
.selection_box {
  padding: 15px 100px;
  height: 100%;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
.box_book {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-direction: column;
  height: 210px;
  width: 20%;
  background-color: white;
  margin: 10px 20px;
  padding-bottom: 10px;
  border: 1px solid rgb(221, 221, 221);
  cursor: pointer;
}
.box_book > p {
  height: 20%;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 5px;
}
.book_imgwrap {
  width: 100%;
  height: 75%;
  background-color: rgb(156, 156, 156);
}
.book_imgwrap > img {
  height: 100%;
  width: auto;
}
.box_bookactive {
  box-shadow: 0px 0px 15px -4px rgba(0, 0, 0, 0.75);
  border: none;
}
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
.custom_bookbox {
  display: flex;
  flex-wrap: wrap;
  max-width: 67vw;
}
.custom_book {
  list-style: none;
  margin: 5px;
  border: 1px solid rgb(221, 221, 221);
  padding: 5px;
}
.active_li {
  border: 1px solid #16cae6;
  background-color: #16cae659;
}
.box_customactive {
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
.box_customactive7{
  display: flex;
}
</style>