<template>
  <div class="py-40 img-background w-full min-h-full">
    <div class="flex flex-col justify-center items-center h-full">
      <p class="text-6xl select-none text-center">
        <span class="font-thin glitch" data-glitch="LOST">
          LOST
        </span>
        <br>
        <span class="font-black glitch" data-glitch="PARADISE">
          PARADISE
        </span>
      </p>
      <p class="text-3xl pt-12">
        06.11.2020
      </p>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.img-background {
  background-image: url('../../assets/img/earth.jpg');
  background-position: center;
  background-repeat: no-repeat;
}
.glitch {
  animation: glitch-skew 1s infinite linear alternate-reverse;
  position: relative;
  &::before{
    position: absolute;
    width: 100%;
    height: 100%;
    content: attr(data-glitch);
    left: 2px;
    text-shadow: -2px 0 #ff00c1;
    clip: rect(44px, 450px, 56px, 0);
    animation: glitch-anim 8s infinite linear alternate-reverse;
  }

  &::after {
    position: absolute;
    width: 100%;
    height: 100%;
    content: attr(data-glitch);
    left: -2px;
    text-shadow: -2px 0 #00fff9, 2px 2px #ff00c1;
    animation: glitch-anim2 2s infinite linear alternate-reverse;
  }
}

@keyframes glitch-anim {
  $steps: 20;
  @for $i from 0 through $steps {
    #{percentage($i*(1/$steps))} {
      clip: rect(random(100)+px, 9999px, random(100)+px, 0);
      transform: skew((random(100) / 100) + deg);
    }
  }
}

@keyframes glitch-anim2 {
  $steps: 20;
  @for $i from 0 through $steps {
    #{percentage($i*(1/$steps))} {
      clip: rect(random(100)+px, 9999px, random(100)+px, 0);
      transform: skew((random(100) / 100) + deg);
    }
  }
}

@keyframes glitch-skew {
  $steps: 10;
  @for $i from 0 through $steps {
    #{percentage($i*(1/$steps))} {
      transform: skew((random(10) - 5) + deg);
    }
  }
}
</style>
