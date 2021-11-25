<template>
  <div class="about">
    <transition
      appear
      name="fade"
      @before-enter="beforeEnter"
      @enter="enter"
      @after-enter="afterEnter"
    >
      <div>
        <h1>About</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum aperiam
          officia possimus delectus inventore quod quisquam culpa voluptas
          iusto, quae maiores quo dolorum, corporis laboriosam a dolore
          consequatur assumenda nam!
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum aperiam
          officia possimus delectus inventore quod quisquam culpa voluptas
          iusto, quae maiores quo dolorum, corporis laboriosam a dolore
          consequatur assumenda nam!
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum aperiam
          officia possimus delectus inventore quod quisquam culpa voluptas
          iusto, quae maiores quo dolorum, corporis laboriosam a dolore
          consequatur assumenda nam!
        </p>
      </div>
    </transition>
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    const showTitle = ref(true);
    const beforeEnter = () => {
    };
    const enter = () => {
    };
    const afterEnter = () => {
    };
    return { beforeEnter, enter, afterEnter, showTitle };
  },
};
</script>

<style>
.about {
  max-width: 600px;
  margin: 20px auto;
}
.fade-enter-from {
  opacity: 0;
  transform: scale(0.6);
}
.fade-enter-to {
  opacity: 1;
  transform: scale(1);
}
.fade-enter-active {
  transition: all 0.3s ease;
}
</style>