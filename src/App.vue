<template>
  <div>
    <p>Horizontal and Vertical</p>
    <a-row class="grid-demo" :gutter="[24, 12]">
      <a-col :span="6">
        <div>col - 6</div>
      </a-col>
      <a-col :span="6">
        <div>col - 6</div>
      </a-col>
      <a-col :span="6">
        <div>col - 6</div>
      </a-col>
      <a-col :span="6">
        <div>col - 6</div>
      </a-col>
      <a-col :span="6">
        <div>col - 6</div>
      </a-col>
    </a-row>
  </div>
</template>

<style scoped>
.grid-demo .arco-col {
  height: 48px;
  color: var(--color-white);
}
.grid-demo .arco-col > div {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
}
.grid-demo .arco-col:nth-child(2n) > div {
  background-color: rgba(var(--arcoblue-6), 0.9);
}
.grid-demo .arco-col:nth-child(2n + 1) > div {
  background-color: var(--color-primary-light-4);
}
</style>
