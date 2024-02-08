<template>
  <div class="item">
    <div class="details">
      <h3>
        <slot name="heading"></slot>
      </h3>
      <slot></slot>
      <h3>
        <slot name="heading2"></slot>
      </h3>
    </div>
  </div>
</template>

<style scoped>
.item {
  margin-top: 2rem;
  margin-bottom: 2rem;
  position: relative;
}

.details {
  margin-left: 1rem;
  margin-right: 1rem;
  justify-content: center;
  text-align: center;
}

i {
  display: flex;
  place-items: center;
  place-content: center;
  width: 32px;
  height: 32px;

  color: var(--color-text);
}

h3 {
  font-size: 1.2rem;
  font-weight: 500;
  margin-bottom: 0.4rem;
  color: var(--color-heading);
  justify-content: center;
}

@media (min-width: 1024px) {

  h3 {
    font-size: 1.5rem;
  }
  .item {
    margin-top: 0;
    padding: 1rem;
    font-size: 1.2rem;
  }

  i {
    top: calc(50% - 25px);
    left: -26px;
    position: absolute;
    border: 1px solid var(--color-border);
    background: var(--color-background);
    border-radius: 8px;
    width: 50px;
    height: 50px;
  }

  .item:before {
    content: ' ';
    border-left: 1px solid var(--color-border);
    position: absolute;
    left: 0;
    bottom: calc(50% + 25px);
    height: calc(50% - 25px);
  }

  .item:after {
    content: ' ';
    border-left: 1px solid var(--color-border);
    position: absolute;
    left: 0;
    top: calc(50% + 25px);
    height: calc(50% - 25px);
  }

  .item:first-of-type:before {
    display: none;
  }

  .item:last-of-type:after {
    display: none;
  }
}
</style>
