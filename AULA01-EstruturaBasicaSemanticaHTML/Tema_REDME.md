# 📚 Aula01: [Estrutura Básica Página HTML]

## 🗓 Data [02/03/2026]
---
## 🎯 Objetivo da Aula
- Compreender a estutura básica de página HTML
- O que precisa ter na estrutura básica HTML
---
## 📖 Conteúdos Abordados
    - <html>
    - <head> 
    - <body>  
    - <header>
    - <main>
---
## 💡 Conceitos Importantes

### **`<html>`** 
- É o elemento raiz de um documento HTML, envolvendo todo o conteúdo, como `<head>`e `<body>`
- Ela informa ao navegador que o arquivo é HTML5, devendo ser aberta logo após o `<!DOCTYPE html>` e fechada no final

### **`<head>`**
- Contêiner invisível ao usuário, situado no topo do documento, que armazena metadados essenciais
- Não são exibidas diretamente na página web para o usuário, mas são cruciais para o navegador e os motores de busca (SEO) processarem e interpretarem o documento.
- Exemplo

### **`<body>`** 
- Representa o corpo de um documento e contém todo o conteúdo visível de um site, como textos, imagens, vídeos, menus e seções. 
- Ela deve ser única em cada documento

### **`<main>`**
- Em HTML define o conteúdo principal e dominante do corpo do documento. É um elemento semântico do HTML5 que ajuda a indicar aos navegadores e tecnologias assistivas (como leitores de tela) qual é a parte central e única da página.
- Ele ajuda a estruturar a página e melhora a acessibilidade e o SEO do site.

### **`<header>`**
- É uma tag semântica utilizada para representar um contêiner para conteúdo introdutório ou um conjunto de links de navegação.
- Ele ajuda a estruturar a página e melhora a acessibilidade e o SEO do site.
- Cabeçalho de uma página ou de uma seção.

    - 👉 É a parte introdutória, onde normalmente ficam:   
        Título;   
        Logo;   
        Menu de navegação;   
        Informações iniciais;

    - 📌 Onde usar `<header>`?
        - No topo da página (Representa o cabeçalho principal);
        - Dentro de outras seções (Cada bloco pode ter seu próprio header);
    
### **`<section>`**
- Representa um agrupamento de conteúdo com um mesmo assunto.
- É como um “bloco de assunto” dentro da página.
- Importante sempre colocar título na section
- Conteúdo com tema bem definido
- Use `<section>` quando o conteúdo tiver um contexto claro e separado.

- 📌 Características   
    ✔ Tem tema definido   
    ✔ Geralmente tem título (h1-h6)   
    ✔ Organiza a página em partes

- 🧪 Exemplo básico
```html
<section>
    <h2>Sobre mim</h2>
        <p>Sou estudante de programação...</p>
</section>
```

### **`<article>`**
- É um conteúdo que faz sentido sozinho.
- Deve, idealmente, conter um título
- É uma unidade completa de conteúdo
    
- 📌 Características   
    ✔ Independente   
    ✔ Reutilizável   
    ✔ Pode ser compartilhado   
            
- 🧪 Exemplo básico
```html
<article>
    <h3>Serviço de criação de sites</h3>
    <p>Desenvolvemos sites profissionais...</p>
</article>
```
---

## 🛠 Exemplo Prático
```html
<!DOCTYPE html> <!--define HTML5-->
<html lang="en"> <!--raiz do documento-->
    <head><!--configurações invisíveis-->
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
        <link rel="stylesheet" href="...">
    </head>
    <body><!--corpo - conteúdo visível-->

        <header><!-- Cabeçalho principal da página-->
            <h1>Meu site</h1>
        </header>

        <main> <!--conteúdo principal - dominante-->   
            <section>
                <header><!-- Cabeçalho da seção-->
                    <h2>Serviços</h2>
                    <p>Veja o que oferecemos</p>
                </header>

                <p>Desenvolvimento web, consultoria...</p>

                <article>
                    <h2>Serviço 1</h2>
                    <p>Descrição do serviço</p>
                </article>
            </section>

            <article><!-- Conteúdo independente-->
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