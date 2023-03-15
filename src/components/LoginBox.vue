<template>
    <div class="login-box">
        <img src="../assets/image.png">
        <div class="textfield_wrapper">
            <input class="textfield" style="margin-bottom: 30px ;" type="text" placeholder="Email">
            <input class="textfield" type="password" placeholder="Senha">
        </div>
        <span class="link" @click="this.showAlert()">Esqueci a senha</span>
        <button class="button" @click="$emit('login');">Entrar</button>
    </div>
</template>
<script>
export default{
    methods: {
        showAlert(){
            alert("problema seu, burro!");
        }
    }
}
</script>

<style scoped>
@media only screen and (max-width: 320px){
    .link{
        font-size: 8pt; 
    }
}
.link{
    color: #579bd6;
    font-size: 10pt;
    cursor: pointer;
    margin-right: 200px;
    margin-top: -30px;
    font-family: "Raleway-Bold";
}
.login-box{
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    height: 400px;
    width: fit-content;
    background-color: white;
    color: #383838;
    padding: 5px 50px;
    border: none;
    border-radius: 5px;
    /* box-shadow: 10px 5px 5px #00000040; */
}
.textfield_wrapper{
    margin-top: -20px ;
    width: 300px;
    display: flex;
    justify-content: space-between;
    flex-direction: column;
}
.textfield{
    border-bottom-left-radius: 0px;
    border-bottom-right-radius: 0px;
    padding: 10px;
    font-family: 'Raleway';
    width: 100%;
    border-bottom: solid #383838;
    border-top: none;
    border-left: none;
    border-right: none;
    font-size: 14px;
}
input:focus {
    outline: none;
}

.button{
    background-color: #a8c33f;
    color: white;
    border: none;
    border-radius: 5px;
    width: 100%;
    padding: 10px;
    font-size: 20pt;
    cursor: pointer;
    font-family: 'Raleway-Bold';
    transition: 0.5s;
}

.button:hover{
    background-color: #383838;
    color: white;
}

img{
    width: 300px;
}

</style>