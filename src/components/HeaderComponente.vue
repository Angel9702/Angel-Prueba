<template>
  <header>
    <div>
      <svg xmlns="http://www.w3.org/2000/svg" width="86.246" height="26.154" viewBox="0 0 86.246 26.154">
        <path id="Trazado_17109" data-name="Trazado 17109" d="M190.219,442.924h26.154V416.77H190.219Zm1.626-24.528h22.9v22.9h-22.9Zm3.956,3.956h14.755v1.626H197.427v5.055H206.8v1.626h-9.368v5.055h13.129v1.627H195.8Zm24.464,20.572h26.154V416.77H220.265Zm1.626-24.528h22.9v22.9h-22.9Zm18.431,3.832h1.843l-7.815,14.683h-1.436L225.1,422.228h1.843l6.691,12.57Zm9.99-5.458v26.154h26.154V416.77ZM274.839,441.3h-22.9V418.4h22.9Zm-18.431-3.831h-1.843l8.533-16.032,8.533,16.032h-1.843L263.1,424.9Z" transform="translate(-190.219 -416.77)" fill="#fff"/>
      </svg>
    </div>
    <nav>
      <img src="../assets/panel.svg" alt="">
    </nav>
  </header>
</template>

<script>
export default {

}
</script>

<style scoped>
header {
  background-color: black;
  display: flex;
  padding: 0.625rem 10px;
  justify-content: space-between;
  align-items: center;
}
img {
  max-width: 200px;
}

@media (min-width: 576px) { 
  .header {
    padding: 1rem 10px;
  }
}
 /* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) {
  .header {
    padding: 1rem 1.875rem;
  }
  /* .yury {
    display: inline-block;
} */
 }
/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) { 
  .header {
    padding: 1rem 3.75rem;
  }
}
 /* Extra large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) { 
  /* .header {
    padding: 1rem 60px;
  } */
}
</style>