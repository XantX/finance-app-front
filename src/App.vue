<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style>
  *,
  *::before,
  *::after{
    box-sizing: border-box;
    margin: 0px;
    padding: 0px;
  }
  :root{
    --black-0h: #1d2021;
    --black-0s: #32302f;
    --black-0: #282828;
    --black-1: #3c3836;
    --black-2: #504945;
    --black-3: #665c54;
    --black-4: #7c6f64;
    --white-0: #fbf1c7;
    --white-1: #ebdbb2;
    --white-2: #d5c4a1;
    --white-3: #bdae93;
    --white-4: #a89984;

    --gray: #928374;

    --blue: #83a598;
    --aqua: #8ec07c;
    --yellow: #fabd2f;
    --orange: #fe8019;
    --purple: #d3869b;
    --green: #b8bb26;
    --red: #fb4934;
  }
  @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,200;0,400;0,500;1,900&display=swap');
  #app{
    font-family: 'Montserrat', sans-serif;
    background-color: var(--white-0);
  }
</style>
