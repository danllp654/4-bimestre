<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página Responsiva</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Minha Página Responsiva</h1>
        <nav>
            <ul>
                <li><a href="#">Início</a></li>
                <li><a href="#">Sobre</a></li>
                <li><a href="#">Serviços</a></li>
                <li><a href="#">Contato</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero">
            <h2>Bem-vindo à nossa página!</h2>
            <p>Esta é uma página de exemplo que demonstra responsividade com HTML e CSS.</p>
        </section>

        <section class="content">
            <article>
                <h3>Seção 1</h3>
                <p>Este é o conteúdo da seção 1.</p>
            </article>
            <article>
                <h3>Seção 2</h3>
                <p>Este é o conteúdo da seção 2.</p>
            </article>
            <article>
                <h3>Seção 3</h3>
                <p>Este é o conteúdo da seção 3.</p>
            </article>
        </section>
    </main>

    <footer>
        <p>&copy; 2023 Minha Página Responsiva. Todos os direitos reservados.</p>
    </footer>
</body>
</html>

/* Reset básico */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
}

header {
    background-color: #333;
    color: #fff;
    padding: 1em;
    text-align: center;
}

header nav ul {
    list-style: none;
    display: flex;
    justify-content: center;
    gap: 1em;
}

header nav ul li a {
    color: #fff;
    text-decoration: none;
}

.hero {
    padding: 2em;
    background: #f4f4f4;
    text-align: center;
}

.content {
    display: flex;
    gap: 1em;
    padding: 1em;
}

.content article {
    flex: 1;
    background: #e2e2e2;
    padding: 1em;
    border-radius: 5px;
}

footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1em;
}

/* Responsividade */
@media (max-width: 768px) {
    .content {
        flex-direction: column;
    }
}

@media (max-width: 480px) {
    header nav ul {
        flex-direction: column;
    }

    header nav ul li {
        margin: 0.5em 0;
    }
}


