<template>
  <div></div>
</template>

<script>
export default {
  name: 'PageHome'
}
</script>

<style>
body {
  padding: 0;
  margin: 0;
}

div {
  height: 100vh;
  background: linear-gradient(45deg, #000 0, #000 50%, #fff 50%);
}
div::before {
  content: "欢乐的小盖盖";
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: #fff;
  font-size: 50px;
  mix-blend-mode: difference;
  animation: move 3s infinite linear alternate;
}
@keyframes move {
  0% {
    transform: translate(-30%, -50%);
  }
  100% {
    transform: translate(-70%, -50%);
  }
}

</style>
