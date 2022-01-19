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
      <div class="button-form">
        <router-link to="/about">
        <button class="login-button" to="/about">Sign in</button>
        </router-link>
        <a class="forget-pass" href="#$">Forget password</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Login',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.login{
  color:var(--gray);
}
.button-form .forget-pass{
  text-decoration: none;
  color: var(--gray);
  margin-top: 0.5rem;
}

.button-form .forget-pass:hover{
  color: var(--aqua);
}
.button-form .login-button{
  border: none;
  background-color: var(--green);
  border-radius: 2rem;
  color: var(--white-0);
  font-size: 1.2rem;
  transition: box-shadow 300ms, color 300ms;
  padding: 1rem 4rem;
}
.button-form .login-button:hover{
  cursor: pointer;
  color: var(--black-0);
  -webkit-box-shadow: 33px 29px 21px -17px rgba(0,0,0,0.53);
  -moz-box-shadow: 33px 29px 21px -17px rgba(0,0,0,0.53);
  box-shadow: 20px 20px 21px -17px rgba(0,0,0,0.53);
  background-color: var(--yellow);
}
.button-form{
  margin-top: 1rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}
h1{
  padding: 1.5rem;
  color:var(--aqua);
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
  color:var(--aqua);
  background-color:var(--white-0);
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
  width:17rem;
  border:2px solid gray;
  border-radius: 0.5rem;
  font-family: inherit;
  font-size:inherit;
  outline: none;
  padding: 1rem;
  background-color:var(--white-0);
}
input:hover{
  border-color: var(--blue);
}
input:focus{
  border-color: var(--blue); 
}
</style>
