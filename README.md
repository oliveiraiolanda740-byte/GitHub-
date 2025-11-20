# GitHub-
1️⃣ Estrutura de Pastas
fundamentos-html5/
├─ assets/
│  ├─ img/
│  │   ├─ logo.png
│  │   ├─ projeto1.jpg
│  │   └─ projeto2.jpg
├─ css/
│  └─ style.css
├─ index.html
├─ projetos.html
└─ cadastro.html


2️⃣ Páginas HTML
index.html – Página Inicial
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Loja Online - Início</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <header>
        <img src="assets/img/logo.png" alt="Logo Loja Online">
        <nav>
            <ul>
                <li><a href="index.html">Início</a></li>
                <li><a href="projetos.html">Projetos Sociais</a></li>
                <li><a href="cadastro.html">Cadastro</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <h1>Bem-vindo à Loja Online</h1>
        <p>Conheça nossa organização e entre em contato conosco!</p>

        <section>
            <h2>Contato</h2>
            <p>Email: contato@lojaonline.com</p>
            <p>Telefone: (11) 99999-9999</p>
        </section>
    </main>

    <footer>
        <p>© 2025 Loja Online</p>
    </footer>
</body>
</html>


projetos.html – Projetos Sociais
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Loja Online - Projetos Sociais</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <header>
        <h1>Projetos Sociais</h1>
        <nav>
            <ul>
                <li><a href="index.html">Início</a></li>
                <li><a href="projetos.html">Projetos Sociais</a></li>
                <li><a href="cadastro.html">Cadastro</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section>
            <h2>Voluntariado</h2>
            <p>Participe de nossas ações sociais e faça a diferença!</p>
            <img src="assets/img/projeto1.jpg" alt="Voluntariado">
        </section>

        <section>
            <h2>Doações</h2>
            <p>Contribua com doações para nossos projetos.</p>
            <img src="assets/img/projeto2.jpg" alt="Doações">
        </section>
    </main>

    <footer>
        <p>© 2025 Loja Online</p>
    </footer>
</body>
</html>


cadastro.html – Formulário
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Loja Online - Cadastro</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <header>
        <h1>Cadastro</h1>
        <nav>
            <ul>
                <li><a href="index.html">Início</a></li>
                <li><a href="projetos.html">Projetos Sociais</a></li>
                <li><a href="cadastro.html">Cadastro</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <form>
            <fieldset>
                <legend>Informações Pessoais</legend>

                <label for="nome">Nome Completo:</label>
                <input type="text" id="nome" name="nome" required>

                <label for="email">E-mail:</label>
                <input type="email" id="email" name="email" required>

                <label for="cpf">CPF:</label>
                <input type="text" id="cpf" name="cpf" pattern="\d{3}\.\d{3}\.\d{3}-\d{2}" placeholder="000.000.000-00" required>

                <label for="telefone">Telefone:</label>
                <input type="tel" id="telefone" name="telefone" pattern="\(\d{2}\) \d{4,5}-\d{4}" placeholder="(11) 99999-9999" required>

                <label for="nascimento">Data de Nascimento:</label>
                <input type="date" id="nascimento" name="nascimento" required>
            </fieldset>

            <fieldset>
                <legend>Endereço</legend>

                <label for="endereco">Endereço:</label>
                <input type="text" id="endereco" name="endereco" required>

                <label for="cep">CEP:</label>
                <input type="text" id="cep" name="cep" pattern="\d{5}-\d{3}" placeholder="00000-000" required>

                <label for="cidade">Cidade:</label>
                <input type="text" id="cidade" name="cidade" required>

                <label for="estado">Estado:</label>
                <select id="estado" name="estado" required>
                    <option value="">Selecione</option>
                    <option value="SP">São Paulo</option>
                    <option value="RJ">Rio de Janeiro</option>
                    <option value="MG">Minas Gerais</option>
                    <!-- Adicione outros estados -->
                </select>
            </fieldset>

            <button type="submit">Enviar</button>
        </form>
    </main>

    <footer>
        <p>© 2025 Loja Online</p>
    </footer>
</body>
</html>


css/style.css – Básico
body {
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 0;
    padding: 0;
}

header, footer {
    background-color: #007bff;
    color: #fff;
    padding: 1rem;
}

nav ul {
    list-style: none;
    display: flex;
    gap: 1rem;
}

nav a {
    color: #fff;
    text-decoration: none;
}

main {
    padding: 1rem;
}

fieldset {
    margin-bottom: 1rem;
    padding: 1rem;
    border: 1px solid #ccc;
}

input, select, button {
    display: block;
    margin-top: 0.5rem;
    margin-bottom: 1rem;
    padding: 0.5rem;
    width: 100%;
}

button {
    background-color: #007bff;
    color: #fff;
    border: none;
    cursor: pointer;
