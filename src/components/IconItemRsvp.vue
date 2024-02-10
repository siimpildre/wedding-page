<template>
    <div class="items">
      <i>
        <slot name="icon"></slot>
      </i>
    </div>
  </template>
  
<style scoped>

  .items {
    margin-top: 2rem;
    display: grid;
    justify-content: center;
    position: relative;
    align-items: center;
  }
  
  i {
    display: flex;
    place-items: center;
    place-content: center;
    width: 32px;
    height: 32px;
  }
  
  @media (min-width: 1024px) {
  
    i {
      border-radius: 8px;
      width: 50px;
      height: 50px;
      padding: 0.5rem;
    }
  /*
    .items:before {
      content: ' ';
      border-left: 1px solid var(--color-border);
      position: absolute;
      left: 0;
      bottom: calc(50% + 25px);
      height: calc(50% - 25px);
    }
  
    .items:after {
      content: ' ';
      border-left: 1px solid var(--color-border);
      position: absolute;
      left: 0;
      top: calc(50% + 25px);
      height: calc(50% - 25px);
    }
  
    .items:first-of-type:before {
      display: none;
    }
  
    .items:last-of-type:after {
      display: none;
    }

*/
    
  }
</style>