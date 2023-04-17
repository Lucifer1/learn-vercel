<template>
  <p>
    <span id="a">欢</span>
    <span id="e">乐</span>
    <span id="i">的</span>
    <span id="o">小</span>
    <span id="u">盖</span>
    <span id="p">盖</span>
  </p>
</template>

<script>
export default {
  name: 'PageHome'
}
</script>

<style>
body {
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #000000;
}

p {
  background: none;
  color: #999;
  font-family: 'Dancing Script', 'Warnes', cursive;
  font-size: 100px;
  letter-spacing: -26px;
  cursor: pointer;
}

p span {
  animation: flicker 3s linear infinite;
  padding: 0 10px;
}

p #a {
  animation-delay: .2s;
}

p #e {
  animation-delay: .5s;
}

p #i {
  animation-delay: .8s;
}

p #o {
  animation-delay: 1.1s;
}

p #u {
  animation-delay: 1.2s;
}

p #p {
  animation-delay: 1.3s;
}

@keyframes flicker {
  0% {
    color: #333;
  }
  2%, 7%, 12%, 15%, 50% {
    color: #fff;
    text-shadow:
      0px 0px 5px #42fff6,
      0px 0px 10px #42fff6,
      0px 0px 20px #42fff6,
      0px 0px 50px #42fff6;

  }

  5%, 10% {
    color: #333;
    text-shadow: none;
  }
}

</style>
