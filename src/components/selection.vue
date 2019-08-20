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
      </div>
    </div>
    <div class="search_customers">
      <div class="customers_tittle">
        <h2>Sprzedający</h2>
      </div>
      <div class="customers_box">
        <div class="box_custom">
          <p>Jan Kowalski</p>
          <ul class="custom_bookbox">
            <li  :class="{  active_li : bnc = bnc % 2 }" class="custom_book">Biologia na czasie</li>
          </ul>
        </div>
        <div class="box_custom">
          <p>Jan Kowalski</p>
          <ul class="custom_bookbox">
            <li :class="{  active_li : bnc = bnc % 2 }" class="custom_book">Biologia na czasie</li>
            <li
              :class="{  active_li : pd = pd % 2 }"
              class="custom_book"
            >Ponad słowami podręcznik klasa 1 CZ. 1 NOWA ERA</li>
            <li :class="{  active_li : wcu = wcu % 2 }" class="custom_book">W centrum uwagi</li>
            <li :class="{  active_li : og = og % 2 }" class="custom_book">Oblicza geografii</li>
            <li
              :class="{  active_li : fof = fof % 2 }"
              class="custom_book"
            >Fizyka - ODKRYĆ FIZYKĘ - Nowa Era - podstawowy</li>
            <li
              :class="{  active_li : kwp = kwp % 2 }"
              class="custom_book"
            >Krok w przedsiębiorczość Podręcznik</li>
          </ul>
        </div>
        <div class="box_custom">
          <p>Jan Kowalski</p>
          <ul class="custom_bookbox">
            <li  :class="{  active_li : bnc = bnc % 2 }" class="custom_book">Biologia na czasie</li>
          </ul>
        </div>
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
      ps: 0
    };
  },
  methods: {}
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
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: white;
  padding: 15px;
  border: 1px solid rgb(221, 221, 221);
  margin-bottom: 5px;
  cursor: pointer;
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
.active_li:nth-of-type(2) {
  border: 1px solid #e616e6;
  background-color: #e616e659;
}
.active_li:nth-of-type(3) {
  border: 1px solid #e6a816;
  background-color: #e6a81659;
}
</style>