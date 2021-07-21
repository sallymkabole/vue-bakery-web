<template>
  <div class="container txt">
    <div class="">
      <div class="d-flex justify-content-between main">
        <div class="p-2">
          <a class="navbar-brand" href="#">The Bakery</a>
        </div>
        <div class="p-2">
          <div class="" id="navbarResponsive">
            <ul class="ml-auto">
              <li class="nav-item active">
                <a class="nav-link" href="#">Home </a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">About</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Services</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Contact</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="p-2">
          <button class="btn my-2 my-sm-0" type="submit">=</button>
        </div>
      </div>
      <div class="row no-gutters">
        <div class="col-4 col-left">
          <div class="card-body">
            <h1 class="display-1 b fw-bold txtcol">Bakery</h1>
            <h1 class="text-left fw-bold txtcol display-1 b">Shop</h1>

            <div class="b card-text mb-4" style="width: 20rem">
              <h6 class="mt-4 text-left">
                Don't take our word for it. You gotta try them yourself.
              </h6>
            </div>
            <button class="btn1 btn-lg rounded-pill">Shop Now</button>
          </div>
        </div>
        <div class="col-8 circular col-right" :style="img"></div>
      </div>
    </div>

    <div class="d-flex flex-row justify-content-between top">
      <div class="m-2">
        <h1 class="b fw-bold txtcol">Popular Bakes</h1>
        <h6 class="text-left">These are top picks from our clients</h6>
      </div>
      <div class="">
        <button class="btn m-4  rounded-pill">FULL MENU</button>
      </div>
    </div>
    <div class="d-flex flex-row">
      <div class="col-4">
        <div class="card crd m-2">
          <img
            class="card-img-top img-card"
            :src="image1"
            alt="Card image cap"
          />
          <div class="card-body">
            <p class="text-left card-title font-weight-bold">
              3Kg. White Forest
            </p>
            <p class="text-left font-weight-light">Ksh. 1800</p>

          </div>
        </div>
      </div>
      <div class="col-4">
         <div class="card crd m-2">
          <img
            class="card-img-top img-card"
            :src="image1"
            alt="Card image cap"
          />
          <div class="card-body">
            <p class="text-left card-title font-weight-bold">
              3Kg. White Forest
            </p>
            <p class="text-left font-weight-light">Ksh. 1800</p>

          </div>
        </div>
      </div>
      <div class="col-4">
         <div class="card crd m-2">
          <img
            class="card-img-top img-card"
            :src="image1"
            alt="Card image cap"
          />
          <div class="card-body">
            <p class="text-left card-title font-weight-bold">
              3Kg. White Forest
            </p>
            <p class="text-left font-weight-light">Ksh. 1800</p>

            
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Nav",
  props: {
    msg: String,
  },
  data() {
    return {
      img: {
        backgroundImage: `url(${require("@/assets/bread.png")})`,
      },
      image: require("@/assets/sp.png"),
      image1: require("@/assets/white.jpg"),
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #bb987f;
}

/* visited link */
a:visited {
  color: #000;
}

/* mouse over link */
b {
  text-align: left;
}
a:hover {
  color: #521403;
}

/* selected link */
a:active {
  color: #c6723a;
}
.b {
  text-align: left;
}
.btn {
  color: #fff;
  background-color: #c6723a;
}
.btn1 {
  color: #fff;
  background-color: #c6723a;
  float: left;
  text-transform: uppercase;
}
.txtcol {
  color: #521403;
}
.circular {
  background-repeat: no-repeat;
  background-size: contain;
  width: 600px;
  height: 600px;

  margin-bottom: 20px;
}
.col-left,
.col-right {
  display: table-cell;
  vertical-align: middle;
}
.col-right {
  display: flex;
  float: right;
}
.row {
  width: 100%;
  height: 100%;
  display: table-row;
}
.main {
  margin: 20px;
}
.txt {
  font-family: "Be Vietnam", sans-serif;
}
.active {
  color: #a815c5 !important;
  border-bottom: 5px solid #521403;
}
li > a[data-selected="true"]:after {
  content: "\25CF";
  position: absolute;
  top: 1.1em;
  left: 50%;
  width: 10px;
  margin-left: -5px;
  color: cadetblue;
}
.top {
  margin-top: 30px;
}
.row.row-eq-height {
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
}
.col-md-4 {
  border: 1px solid red;
}
</style>
 