<template>
<div>
 <section id="app">
    <div><img src="./assets/main2.jpg" /></div>
    <div>
      <div class="imput-desk">
        <div class=" text-imput">
          <input placeholder="Login" class="input" type="text" name="login" id="login-text"/>
        </div>
        <div class=" text-imput">
          <input placeholder="Password" class="input" type="text" id="pass-text"/>
        </div>
      </div>
      <div class="checkbox-imput">
        <input class="checkbox" type="checkbox" unchecked />
        <label class="">Запомнить</label>
      </div>
      <div id="button-div">
        <button class="button-3" role="button" v-on:click="signUp1">Login</button>
        <button class="button-3" role="button" v-on:click="signUp">Регистрация</button>
      </div>
    </div>
  </section>
</div>
  
</template>

<script lang="ts">
import axios from "axios";

export default {
    methods: {
      signUp() {
        const regLogin: HTMLInputElement = document.getElementById(
          "login-text"
        ) as HTMLInputElement;
        const config = {
          url: 'https://6c52de2e-a739-41c5-83fe-d1c1348ee2b0.mock.pstmn.io/reg',
        };
        const data = {
          Login: regLogin.value,
        };
        axios
          .post(config.url, data, {
            headers: { 'Content-Type': 'application/json',
        'x-mock-match-request-body': 'true', },
          })
         .then(
          (res: any) => {
            alert("Данный логин уже занят");
          },
        ).catch(
        (err: any) => {
          alert("Регистрация прошла успешно");
          });
      },
      signUp1() {
        const regLogin: HTMLInputElement = document.getElementById(
          "login-text"
        ) as HTMLInputElement;
        const pass: HTMLInputElement = document.getElementById(
          "pass-text"
        ) as HTMLInputElement;
        const config = {
          url: 'https://6c52de2e-a739-41c5-83fe-d1c1348ee2b0.mock.pstmn.io/auth',
        };
        const data = {
          Login: regLogin.value,
          password : pass.value,
        };
        axios
          .post(config.url, data, {
            headers: { 'Content-Type': 'application/json',
        'x-mock-match-request-body': 'true', },
          })
         .then(
          (response) => {
            if(response.data.good){
              alert("Успешная авторизация");
            }
          },
        ).catch(
        (error) => {
          alert("Неверный логин или пароль");
          });
      },
    },
  };
</script>

<style>
#app {

    display: flex;
    flex: row;
    flex-wrap: wrap;
    justify-content: center;
    align-items:center;
  }
  #button-div {
    display: flex;
    justify-content: center;
  }
  .input {
    max-width: 200px;
    height: 50%;
    margin-bottom: 8px;
    margin-top: 8px;
    color: rgb(0, 0, 0);
    border: 0;
    border-radius: 5px;
    box-shadow: inset 0 1px 4px rgba(0, 0, 0, 0.3), 0 1px rgba(255, 255, 255, 0.06);
    padding: 10px;
  }
  .text-imput {
    display: flex;
    width: 300px;
    align-items: center;
    justify-content: center;
  }
  .checkbox-imput {
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .checkbox {
    width: 17px;
    height: 17px;
    margin-top: 8px;
    margin-right: 12px;
    margin-bottom: 8px;
    cursor: pointer;
  }
  .checkbox:disabled{
    cursor: default;
  }

  /* CSS */
  .button-3 {
    appearance: none;
    background-color: #912f2f;
    border: 1px solid rgba(27, 31, 35, 0.15);
    border-radius: 6px;
    box-shadow: rgba(27, 31, 35, 0.1) 0 1px 0;
    box-sizing: border-box;
    color: #fff;
    cursor: pointer;
    display: inline-block;
    font-family: -apple-system, system-ui, 'Segoe UI', Helvetica, Arial,
      sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji';
    font-size: 14px;
    font-weight: 600;
    line-height: 20px;
    padding: 6px 16px;
    position: relative;
    text-align: center;
    text-decoration: none;
    user-select: none;
    touch-action: manipulation;
    vertical-align: middle;
    white-space: nowrap;
    margin-left: 10px;
  }

  .button-3:focus:not(:focus-visible):not(.focus-visible) {
    box-shadow: none;
    outline: none;
  }

  .button-3:hover {
    background-color: #c96159;
  }

  .button-3:focus {
    box-shadow: rgba(46, 164, 79, 0.4) 0 0 0 3px;
    outline: none;
  }

  .button-3:disabled {
    background-color: #912f2f;
    border-color: rgba(27, 31, 35, 0.1);
    color: rgba(255, 255, 255, 0.8);
    cursor: default;
  }

  .button-3:active {
    background-color: #eb817a;
    box-shadow: rgba(20, 70, 32, 0.2) 0 1px 0 inset;
  }

</style>
