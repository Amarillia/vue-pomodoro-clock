<template>
  <div class="container">
    <button class="myButton">
      <slot>{{name}}</slot>
    </button>
  </div>
</template>

<script>
export default {
  name: "AppButton",
  props: {
    name: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.myButton {
  -moz-box-shadow: 0px 10px 14px -7px #8a240b;
  -webkit-box-shadow: 0px 10px 14px -7px #8a240b;
  box-shadow: 0px 10px 14px -7px #8a240b;
  background: -webkit-gradient(
    linear,
    left top,
    left bottom,
    color-stop(0.05, #db6e53),
    color-stop(1, #9d4f3c)
  );
  background: -moz-linear-gradient(top, #db6e53 5%, #9d4f3c 100%);
  background: -webkit-linear-gradient(top, #db6e53 5%, #9d4f3c 100%);
  background: -o-linear-gradient(top, #db6e53 5%, #9d4f3c 100%);
  background: -ms-linear-gradient(top, #db6e53 5%, #9d4f3c 100%);
  background: linear-gradient(to bottom, #db6e53 5%, #9d4f3c 100%);
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#db6e53', endColorstr='#9d4f3c',GradientType=0);
  background-color: #db6e53;
  -moz-border-radius: 8px;
  -webkit-border-radius: 8px;
  border-radius: 8px;
  display: inline-block;
  cursor: pointer;
  color: #ffffff;
  font-family: Arial;
  font-size: 20px;
  font-weight: bold;
  padding: 13px 32px;
  text-decoration: none;
  text-shadow: 0px 1px 0px #d53811;
  border: none;
  margin: 10px;
}
.myButton:hover {
  background: -webkit-gradient(
    linear,
    left top,
    left bottom,
    color-stop(0.05, #9d4f3c),
    color-stop(1, #db6e53)
  );
  background: -moz-linear-gradient(top, #9d4f3c 5%, #db6e53 100%);
  background: -webkit-linear-gradient(top, #9d4f3c 5%, #db6e53 100%);
  background: -o-linear-gradient(top, #9d4f3c 5%, #db6e53 100%);
  background: -ms-linear-gradient(top, #9d4f3c 5%, #db6e53 100%);
  background: linear-gradient(to bottom, #9d4f3c 5%, #db6e53 100%);
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#9d4f3c', endColorstr='#db6e53',GradientType=0);
  background-color: #9d4f3c;
}
.myButton:active {
  position: relative;
  top: 1px;
}

.container {
  text-align: left;
  max-width: 40%;
}
</style>
