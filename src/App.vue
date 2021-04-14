<template>
  <div class="container">
    <Header title="Task Tracker" />
  </div>
</template>

<script>
import Header from "./components/Header";

export default {
  name: "App",
  components: {
    Header,
  },
  data() {
    return {
      tasks: []
    }
  },
  created() {
    this.tasks = [
      {
      id: 1,
      text: "Memancing Ikan di Dapur",
      day: "Senen, 8 Mharet 2000",
      reminder: true,
    },
    {
      id: 2,
      text: "Memakan Sate Abang Adek",
      day: "Jumahat, 10 AgusHarimurti 2077",
      reminder: true,
    },
    {
      id: 3,
      text: "Mencagkul Tobat di Kampung",
      day: "Rebo, 13 Martumpol 1945",
      reminder: false,
    },
    {
      id: 4,
      text: "Mencuri Ikan tapi Bayar",
      day: "Marminggu, 30 Februari 2020",
      reminder: false,
    },
  ]);
    ]
  }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;400&display=swap");
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: "Poppins", sans-serif;
}
.container {
  max-width: 500px;
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  border: 1px solid steelblue;
  padding: 30px;
  border-radius: 5px;
}
.btn {
  display: inline-block;
  background: #000;
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
}
.btn:focus {
  outline: none;
}
.btn:active {
  transform: scale(0.98);
}
.btn-block {
  display: block;
  width: 100%;
}
</style>
