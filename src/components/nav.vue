<template>
<nav class="nav">
        <h2>Wybierz ksiażki</h2>
        <div class="nav_searchinput">
          <img src="https://img.icons8.com/ios-filled/50/000000/search.png" />
          <input type="text" placeholder="Przeszukaj zbiór" />
        </div>
      </nav>
</template>
<script>
</script>
<style>
.nav {
  padding: 35px;
  width: 99vw;
  height: 75px;
  background-color: white;
  display: flex;
  align-items: center;
  border-bottom: 1px solid rgb(221, 221, 221);
}

.nav_searchinput {
  margin-left: 13.5vw;
  height: 32.5px;
  width: 38vw;
  border-radius: 3px;
  border: 1px solid rgb(199, 199, 199);
  background-color: rgb(246, 246, 246);
  display: flex;
  align-items: center;
  padding: 3px;
}
.nav_searchinput > input {
  color: rgb(116, 115, 115);
  border: none;
  background-color: transparent;
  outline: none;
  text-align: center;
  width: 100%;
  height: 100%;
  margin-left: 3px;
  border-left: 1px solid rgb(199, 199, 199);
}
.nav_searchinput > img {
  margin: 3px;
  height: 18px;
  width: 18px;
}
</style>