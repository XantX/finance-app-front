<template>
  <div class="login">
    <div id="form">
      <h1>Login</h1>
      <div class="input-form username">
        <input type="text" id="username" placeholder=" " />
        <label class="user-label" >Username</label>
      </div>
      <div class="input-form password">
        <input type="password" id="password" placeholder=" " />
        <label class="pass-label">Password</label>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1{
  padding: 1.5rem;

}
.login{
  height:100%;
}
#form{
  display: flex;
  flex-direction: column;
  align-items: center;
}
.input-form{
 position:relative;
 display:flex;
 flex-direction: column;
 margin: 4% auto;
}
label{
  position:absolute;
  top:1rem;
  left:1rem;
  padding-right: 0.3rem;
  padding-left: 0.3rem;
  transition: top 200ms;
  cursor: text;
  background-color:white;
}
#username:focus ~ .user-label,
#username:not(:placeholder-shown)#username:not(:focus) ~ .user-label
{
  top: -0.6rem;
}
#password:focus ~ .pass-label,
#password:not(:placeholder-shown)#password:not(:focus) ~ .pass-label
{
  top: -0.6rem;
}
input{
  border:2px solid gray;
  border-radius: 0.5rem;
  font-family: inherit;
  font-size:inherit;
  outline: none;
  padding: 1rem;
  background-color:none;
}
input:hover{
  border-color: blue;
}
input:focus{
  border-color: blue; 
}
</style>
