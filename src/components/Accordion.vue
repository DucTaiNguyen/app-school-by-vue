<template>
  <div class="lecture-detail-container">
    <div class="lecture-detail-container01">
      <div class="lecture-detail-container02">
        <div class="lecture-detail-title" @click="open = !open">
          <span class="lecture-detail-text"> {{ title }}</span>
          <span class="lecture-detail-text01">+</span>
        </div>
      </div>
      <div class="lecture-detail-container03" v-show="open">
        <div class="lecture-detail-container07">
          <span class="lecture-detail-text09">{{ description }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Accordion",
  data() {
    return {
      open: false,
    };
  },
  props: {
    title: {
      type: String,
      default: "Lecture 1",
    },
    description: {
      type: String,
      default: "Lecture 1",
    },
  },
};
</script>

<style scoped>
.lecture-detail-container {
  width: 100%;
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: column;
  justify-content: flex-start;
}
.lecture-detail-container01 {
  flex: 0 0 auto;
  display: flex;
  width: 100%;
  align-items: flex-start;

  padding-right: var(--dl-space-space-halfunit);
  flex-direction: column;
}
.lecture-detail-container02 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: center;
  grid-row-gap: var(--dl-space-space-unit);
  flex-direction: column;
  justify-content: flex-start;
}
.lecture-detail-title {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  transition: 0.3s;
  align-items: center;
  padding-left: 0px;
  padding-right: 0px;
  flex-direction: row;
  justify-content: space-between;
  background-color: #e0eff2;
}
.lecture-detail-text {
  margin-left: var(--dl-space-space-doubleunit);
}
.lecture-detail-text01 {
  margin-right: var(--dl-space-space-doubleunit);
  padding-right: 0px;
}
.lecture-detail-container03 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  grid-gap: var(--dl-space-space-unit);
  align-items: flex-start;
  padding-top: var(--dl-space-space-unit);
  padding-bottom: var(--dl-space-space-unit);
  flex-direction: column;
}

a {
  text-decoration: none;
}
</style>
