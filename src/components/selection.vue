<template>
  <div>
    <div class="search_selection">
      <div
        v-bind:id="item.id"
        :key="item.id"
        v-for="item in books"
        class="selection_bookbox"
      >
        <img
          v-on:click="checkBook"
          class="bookbox_img"
          v-bind:src="`${item.url}`"
          alt="imges book"
        />
        <p v-on:click="checkBook" class="bookbox_tittle">{{ item.tittle }}</p>
      </div>
    </div>
    <div class="search_seller">
      <div class="seller_tittle">
        <h2>Sprzedający</h2>
      </div>

      <div v-for="items in person" :key="items.id" class="box_seller">
        <p>{{ items.nick }}</p>
        <ul class="seller_ul">
          <li v-for="list in items.books" :key="list.id" class="seller_li">
            {{ list }}
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
import bookJson from "./jsonFiles/bookList.json";
import person1 from "./jsonFiles/userList.json";

export default {
  data() {
    return {
      books: bookJson,
      person: person1,
    };
  },
  methods: {
    checkBook: function(e) {
      const li = [...document.querySelectorAll(".seller_li")];
      const current = e.target.parentElement.textContent;
      let result = li;
      console.log(result[1].textContent);

      result = result.filter((li) => li.textContent.includes(current));

      for (let i = 0; i < result.length; i++) {
        let c = result[i];
        c.style.backgroundColor = "rgb(142, 181, 253)";
        let parent = c.parentElement;
        if (parent.parentElement.classList == "box_seller") {
          parent.parentElement.style.display = "flex";
        }
      }
      this.addBoxShadow(e);
    },
    addBoxShadow: function(e) {
      e.target.parentElement.style.boxShadow =
        "0px 0px 35px rgb(142, 181, 253)";
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
.selection_bookbox {
  height: 180px;
  width: 180px;
  background-color: rgb(199, 199, 199);
  margin-top: 25px;
  margin-bottom: 25px;
  cursor: pointer;
}
.bookbox_img {
  width: auto;
  padding: 0px 40px;
  height: 120px;
}
.bookbox_tittle {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 70px;
  width: 180px;
  padding: 5px;
  background-color: white;
}
/* seller */
/* seller */
/* seller */

.search_seller {
  background-color: #eceff1;
}

.seller_tittle {
  padding: 10px;
  width: 99vw;
  height: 75px;
  background-color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  border: 1px solid rgb(221, 221, 221);
}
.seller_box {
  padding: 20px 100px 100px 100px;
}
.box_seller {
  display: flex;
  width: 95vw;
  margin: 0 auto;
  justify-content: space-between;
  align-items: center;
  background-color: white;
  padding: 15px;
  border: 1px solid rgb(221, 221, 221);
  margin-top: 15px;
  cursor: pointer;
}
.seller_ul {
  display: flex;
  flex-wrap: wrap;
  max-width: 67vw;
}
.seller_li {
  list-style: none;
  margin: 5px;
  border: 1px solid rgb(192, 192, 192);
  padding: 7px;
  background-color: white;
}
</style>
