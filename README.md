# instagram
desafio de projeto
index.html
<!DOCTYPEhtml >
< html  lang =" en " >
< cabeça >
    < meta  charset =" UTF-8 " >
    < meta  name =" viewport " content =" largura=largura do dispositivo, escala inicial=1.0 " >
    < link  rel =" folha de estilo " href =" style.css " >
    < title > Instagram </ title >
</ cabeça >
< corpo >
    < div  class =" instagram-wrapper " >
        < div  class =" instagram-phone " >
            < img  src =" ./img/instagram-celular.png " alt =" celular " >
        </ div >
        < div  class =" instagram-continuar " >
            < classe div  =" grupo " >
                < img  src =" ./img/instagram-logo.png " class =" instagram-logo " alt =" instagram logo " >
                < div  class =" foto do perfil " >
                    < img  src =" ./img/perfil-instagram.jpg " alt =" foto de perfil " >
                </ div >
                < a  href =" # " class =" instagram-login " > Continuar como marcospmarinhoo </ a >
                < a  href =" # " class =" instagram-logout " > Remover conta </ ​​a >
            </ div >
            < classe div  =" grupo " >
                < p  class =" não conta " > Não é marcospmarinho? </ p >
                < p  classe =" não conta " >
                    < span  class =" link-blue " > Contas alternativas </ span >
                    ou
                    < span  class =" link-blue " > inscrever-se </ span >
                </ p >
            </ div >
            < div  class =" obtenha o aplicativo " >
                < p  class =" get-app " > Baixe o aplicativo </ p >
                < classe div  =" baixar " >
                    < a  href =" # " class =" app-download " > </ a >
                    < a  href =" # " class =" app-download " > </ a >
                </ div >
            </ div >
        </ div >
    </ div >
</ corpo >
</ html >


style.css
{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    text-decoration: none;
    font-family: sans-serif;
    font-size: 14px;
}

body {
    width: 100%;
    min-height: 100vh;
    background-color: rgb(243, 243, 243);
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
}

.instagram-wrapper {
    display: flex;
    align-items: center;
    justify-content: start;
    width: 60%;
    height: 100vh;
}

.instagram-phone {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 50%;
}

.instagram-phone img {
    height: 50rem;
}

.instagram-continue {
    display: flex;
    align-items: center; /* horizontal */
    justify-content: space-around; /* vertical */
    flex-direction: column;
    width: 50%;
    min-height: 34rem;
}

.group {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-direction: column;
    background-color: #ffffff;
    width: 100%;
    padding: 1.3rem 0;
    border: 1px solid lightgray;
}

.group:nth-child(1) {
    min-height: 19rem;
}

.instagram-logo {
    height: 3rem;
}

.profile-photo {
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    overflow: hidden;
}

.profile-photo img {
    height: 6rem;
}

.instagram-login {
    background-color: #0095f6;
    color: #ffffff;
    padding: 8px;
    border-radius: 4px;
}

.instagram-logout {
    color: #0095f6;
    margin-top: 1rem;
}

.not-account {
    color: rgb(160, 160, 160);
}

.link-blue {
    color: #0095f6;
}

.get-the-app {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 100%;
    padding: 1.3rem 0;
}

.download {
    display: flex;
    width: 100%;
    justify-content: space-evenly;
    align-items: center;
    padding: 1rem;
}

.app-download {
    height: 3rem;
    width: 10rem;
    background-size: cover;
}

.app-download:nth-child(1) {
    background-image: url('./img/apple-button.png');
}

.app-download:nth-child(2) {
    background-image: url('./img/googleplay-button.png');
}

/* media queries */


@media (max-width: 1024px) {
    .instagram-wrapper {
        width: 90%;
    }
}

@media (max-width: 650px) {
    body {
        background-color: #ffffff;
    }

    .instagram-wrapper {
        width: 90%;
    }

    .instagram-phone {
        display: none;
    }

    .instagram-continue {
        width: 100%;
    }
    
    .group {
        border: 1px solid transparent;
    }
}
