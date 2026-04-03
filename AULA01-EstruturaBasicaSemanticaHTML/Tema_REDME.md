# 📚 Aula01: [Estrutura Básica Página HTML]

## 🗓 Data [02/03/2026]

## 🎯 Objetivo do estudo
- Compreender a estutura básica de página HTML;
- O que precisa ter na estrutura básica HTML;
- Entender as tags semânticas HTML e sua importância;
- Entender a correta utilização de tags semântica;

## 📖 Conteúdos Abordados
- `<html>`
- `<head>` 
- `<body>`  
- `<header>`
- `<main>`

## 💡 Conceitos Importantes

### `<html>`: 
- É o elemento raiz de um documento HTML, envolvendo todo o conteúdo, como `<head>`e `<body>`
- Ela informa ao navegador que o arquivo é HTML5, devendo ser aberta logo após o `<!DOCTYPE html>` e fechada no final.
        
### `<head>`: 
- Contêiner invisível ao usuário, situado no topo do documento, que armazena metadados essenciais.
- Não são exibidas diretamente na página web para o usuário, mas são cruciais para o navegador e os motores de busca (SEO) processarem e interpretarem o documento.
    
### `<body>`: 
- Representa o corpo de um documento e contém todo o conteúdo visível de um site, como textos, imagens, vídeos, menus e seções. 
- Ela deve ser única em cada documento.   
   
🧪 Exemplo:
```html
<!DOCTYPE html>
<html lang="pt-BR"> <!-- raiz do documento -->
    <head><!-- contêiner que armazena metadados essenciais -->
        <meta charset="UTF-8">
        <title>Minha Página</title>
    </head>

    <body><!-- corpo do ducumento -->
        <h1>Olá mundo!</h1>
    </body>
</html>
```

## Semântica HTML

### `<main>`: 
- Em HTML define o conteúdo principal e dominante do corpo do documento. É um elemento semântico do HTML5 que ajuda a indicar aos navegadores e tecnologias assistivas (como leitores de tela) qual é a parte central e única da página.
- Ele ajuda a estruturar a página e melhora a acessibilidade e o SEO do site.
- Possui apena um <main> por página   
   
- 📌 Regras importantes:      
    -> Só pode existir 1 por página   
    -> Não pode ficar dentro de `<header>`, `<footer>`, etc.   

### `<header>`: 
- É uma tag semântica utilizada para representar um contêiner para conteúdo introdutório ou um conjunto de links de navegação.
- Ele ajuda a estruturar a página e melhora a acessibilidade e o SEO do site.
- Pode ser o Cabeçalho de uma página ou de uma seção.
   
- 👉 É a parte introdutória, onde normalmente ficam:   
    -> Título;   
    -> Logo;   
    -> Menu de navegação;   
    -> Informações iniciais;   
   
🧪 Exemplo:
```html
<header>
    <h1>Meu Site</h1>
    <nav>
        <a href="#">Início</a>
        <a href="#">Contato</a>
    </nav>
</header>
```
   
- 📌 Onde usar `<header>`?   
    -> No topo da página (Representa o cabeçalho principal);   
    -> Dentro de outras seções (Cada bloco pode ter seu próprio header);

### `<section>`: 
- Representa um agrupamento de conteúdo com um mesmo assunto.
- É como um “bloco de assunto” dentro da página.
- Importante sempre colocar título na section
- Conteúdo com tema bem definido
- Use `<section>` quando o conteúdo tiver um contexto claro e separado.
   
- 📌 Características   
✔ Tem tema definido   
✔ Geralmente tem título (`<h1>` - `<h6>`)   
✔ Organiza a página em partes (seções)   
   
🧪 Exemplo básico
```html
<section>
    <h2>Sobre mim</h2>
    <p>Sou estudante de programação...</p>
</section>
```

### `<article>`: 
- É um conteúdo que faz sentido sozinho.   
- Deve, idealmente, conter um título   
- É uma unidade completa de conteúdo   
   
- 📌 Características   
✔ Independente   
✔ Reutilizável   
✔ Pode ser compartilhado   
   
🧪 Exemplo básico
```html
<article>
    <h3>Serviço de criação de sites</h3>
    <p>Desenvolvemos sites profissionais...</p>
</article>
```

### `<nav>`
- Define uma seção semântica contendo links de navegação principais (menus, sumários, índices).
- Representa uma seção de uma página que aponta para outras páginas ou para outras áreas da página 
- Melhora a acessibilidade e o SEO, permitindo que leitores de tela e motores de busca identifiquem facilmente os menus.
- É ideal usar com listas (`<ul>` e `<li>`)
   
- Use apenas para blocos de navegação importantes, não para todos os links da página.
- Se houver múltiplos `<nav>` na página, utilize o atributo aria-label para diferenciá-los.    
🧪 exemplo: `<nav aria-label="Menu Principal">`
---

## 🛠 Exemplo Prático
```html
<!DOCTYPE html> 
<html lang="en"> 
    <head>>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
        <link rel="stylesheet" href="...">
    </head>
    <body>

        <header>
            <h1>Meu site</h1>
        </header>

        <main>   
            <section>
                <header>
                    <h2>Serviços</h2>
                    <p>Veja o que oferecemos</p>
                </header>

                <p>Desenvolvimento web, consultoria...</p>

                <article>
                    <h2>Serviço 1</h2>
                    <p>Descrição do serviço</p>
                </article>
            </section>

            <article>
                <h2>Bog 01</h2>
                <p>Parágrafo do blog</p>
            </article>
        </main> 

        <footer>
            <p>Rodapé</p>
        </footer>
    </body>
</html>
```