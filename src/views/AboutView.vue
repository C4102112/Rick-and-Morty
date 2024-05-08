<template>
<body>
    <section>
        <img src="..\assets\perfil.jpg" class="img-thumbnail" alt="...">
    </section>
    <header>
        <h1>Caio Vinicius Costa Nascimento</h1>
    </header>
    <section>
        <h2>Sobre Mim</h2>
        <p>Olá, meu nome é Caio Vinicius. Eu sou estudante de T.I na Unimar. Eu tenho interesse em tudo que tem a ver com Tecnologia.</p>
    </section>
    <section>
        <h2>Educação</h2>
        <p>Atualmente, estou cursando Analise e desenvolvimento de Sistemas na Unimar.</p>
    </section>

    <section>
        <h2>Trabalho</h2>
        <p>Atualmente, estou trabalhando como Técnico de Manutenção de Eletrônicos na Empresa Alpha Cell.</p>
    </section>

    <section>
        <h2>Hobbies e Interesses</h2>
        <ul class="text-center">
            <li>Jogar Futebol</li>
            <li>Jogar Video Game</li>
            <li>Programar</li>
        </ul>
    </section>
    <footer>
        <p>Contato: caioc0415@gmail.com</p>
    </footer>
</body>
</template>

<style>
    body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f9;
    color: #333;
}

        .img-thumbnail {
        width: 150px;
        height: 150px;
        border-radius: 50%;
        border: 5px solid #0056b3;
    }

header, section, footer {
    margin-bottom: 20px;
    padding: 20px;
    border-radius: 8px;
    background-color: white;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 10px;
}

h1, h2 {
    color: #0056b3;
    display: flex;
    justify-content: center; 
    align-items: center; 
    margin: 14px;
    flex-direction: column;
    gap: 10px;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    padding: 8px;
    background-color: #e9ecef;
    margin-bottom: 5px;
    border-radius: 4px;
}

footer {
    font-size: small;
    text-align: center;
    color: #666;
}
    
</style>
