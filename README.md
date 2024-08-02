# atividade

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página Dinâmica com JavaScript</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0; /* Remove a margem padrão */
            padding: 0; /* Remove o padding padrão */
            height: 100vh; /* Define a altura da tela */
            display: flex; /* Usar flexbox para centralizar */
            flex-direction: column; /* Alinha os itens na vertical */
            justify-content: center; /* Centraliza verticalmente */
            align-items: center; /* Centraliza horizontalmente */
            text-align: center; /* Centraliza o texto do parágrafo */
        }

        h1 {
            color: #333;
        }

        #naoAperte {
            background-color: #f44336; /* Cor vermelha */
            color: white; /* Cor do texto */
            border: none; /* Sem borda */
            padding: 15px; /* Espaçamento interno igual para cima/baixo e laterais */
            text-align: center; /* Centraliza o texto */
            text-decoration: none; /* Sem sublinhado */
            display: inline-block; /* Para que as propriedades de largura e altura funcionem */
            font-size: 16px; /* Tamanho da fonte */
            margin: 20px 0; /* Margem superior e inferior */
            cursor: pointer; /* Muda o cursor para indicar que é clicável */
            border-radius: 50%; /* Bordas arredondadas para formar um círculo */
            width: 100px; /* Largura do botão */
            height: 100px; /* Altura do botão */
            transition: background-color 0.3s, transform 0.2s; /* Transição suave para efeitos */
        }

        #naoAperte:hover {
            background-color: #d32f2f; /* Cor vermelha escura ao passar o mouse */
            transform: scale(1.05); /* Aumenta levemente o botão ao passar o mouse */
        }
        
        #naoAperte:active {
            transform: scale(0.95); /* Diminui levemente o botão ao clicar */
        }
    </style>
</head>
<body>

    <p id="mensagem">Não clique no botão abaixo.</p>
    
    <button id="naoAperte">Não Aperte</button>

    <script>
        document.getElementById('naoAperte').addEventListener('click', function() {
            // Gera uma mensagem dinâmica
            const mensagens = [
                "Não aperte esse botão!",
                "Pare de apertar esse botão!",
                "Por favor, não clique novamente!",
                "Você realmente não deveria apertar isso.",
                "Vamos evitar mais cliques, ok?",
                "Sério, esse botão não é para ser apertado!",
                "Apertar não é uma boa ideia.",
                "Continue sem clicar.",
                "Você ainda está pensando em apertar?",
                "Vamos deixar o botão em paz!",
                "Esse botão não precisa de mais cliques.",
                "Você pode resistir a essa tentação!",
                "Aperte outra coisa, mas não este botão!",
                "Se você não apertar, vai ficar tudo bem.",
                "A vida é mais interessante sem clicar!",
                "Aperte apenas se realmente precisar.",
                "Desista de apertar este botão!",
                "Mantenha seus dedos longe!",
                "Cuidado com esse botão!",
                "Melhor não clicar novamente.",
                "Vamos apenas ignorar esse botão."
            ];

            // Seleciona uma mensagem aleatória
            const mensagemAleatoria = mensagens[Math.floor(Math.random() * mensagens.length)];

            // Atualiza o conteúdo do parágrafo
            document.getElementById('mensagem').innerText = mensagemAleatoria;
        });
    </script>

</body>
</html>
