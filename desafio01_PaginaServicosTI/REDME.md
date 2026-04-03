
# Sobre o Projeto
Aqui estão:
- Proposta do desafio.
- Dificuldades: Relato das dificuldades enfrentadas na execução do desafio e anotações. 
- Como o projeto me ajudo.
- Aprofundamentos de temas ou assuntos que ficaram um pouco vago, e que  foram necesários para cumprir o desafio.

## Desafio
- 💻 🚀 DESAFIO: Página de Serviços de TI   
   
🎯 Objetivo   
- Criar uma página simples de um profissional de TI (tipo você 👨‍💻), com:
- Menu
- Serviços
- Passo a passo
- Glossário   
---
- 🧱 Estrutura que você deve montar   
   
🔹 1. Cabeçalho + Navegação   
    - Use: `<header>`, `<nav>`, `<ul>`   
   
    👉 Deve conter:
    - Início
    - Serviços
    - Contato   
   
🔹 2. Conteúdo principal   
    - Use: `<main>`   
   
🔹 3. Seção de Serviços   
    - Use: `<section>` , `<article>`, `<ul>`   
    👉 Cada serviço deve ter:   
    Título (`<h3>`)   
    Descrição com: `<strong>` (destaque) `<em>`(ênfase)   
   
🔹 4. Passo a passo de atendimento   
    - Use: `<section>`, `<ol>`   
   
🔹 5. Glossário de termos   
    - Use: `<section>`, `<dl>`, `<dt>`, `<dd>`   
   
🔹 6. Rodapé   
    - Use: `<footer>`

## Dificuldades + aprofundamento

### 1ª Dificuldade: Utilização da tag `<a>`
- Tag `<a>` - link, para transformar um 'elemento' textual em link de direcionamento para outra página é necessário que este 'elemento' esteja dentro da tag, ou seja    
   
❌ Eu estava fazendo da seguinte forma:
```html
<li><a href="paginas/servicos.html" target="_blank"></a>Serviços</li>
```
- Neste caso o 'elemento' Serviços é apenas uma lista sem link

✔ Corretos é:
```html
<li><a href="paginas/servicos.html" target="_blank">Serviços</a></li>
```
- Neste caso o 'elemento' Serviços é clicável e redireciona para a página do link

### 2ª Dificuldade: Semântica

🧪 Exemplo:   
❌ Eu estava fazendo da seguinte forma:
```html
<ol>
    <li> Primeiro Contato </li>
    <p>
        O cliente entra em contato informando sua necessidade, dúvida ou problema. Nesse momento, são coletadas as informações iniciais para entender a demanda.
    </p>
</ol>
```
- obs.: desta forma o <p> está 'solto' do elemento da lista   
   
✔ O correto é:
```html
<ol>
    <li> Primeiro Contato 
        <p>
            O cliente entra em contato informando sua necessidade, dúvida ou problema. Nesse momento, são coletadas as informações iniciais para entender a demanda.
        </p>
    </li> 
</ol>
```   
- obs.: Faze mais sentido já que a decrição do parágrafo faz parte do elemento da lista

### Como o projeto me ajudou

- A compreender a impostância da posição das tags para que tudo funcione corretamente;
- A comprender melhor a lógica semântica com relação as listas;
- Compreender melhor o uso de lista semântica `<dl>`
- Compreender quando e como utilizar lista semântica da forma correta; 

- Minha opinião: Pequenos projetos com este agregam um valor significativo para o se desenvolver técnicamente pois possibitam a busca e principalmente a compreesão e aplicação prática dos consitos estudados. Em resumo: Um paso mais próximo do meu objetivo de me tronar um desenvolvedor front-end e posteriormente full-stack. 

### Aprofundamento: Uso de `<dl>` 

- `<dt>`- (Definition Term) - definição do termo;
- `<dd>`- (Definition Description) - descrição do termo;   
🎯 Objetivo real dessas tags   
👉 Representar relações de explicação   
→ Não é uma lista comum — é uma lista semântica de conceitos.   

📌 Use `<dl>` quando tiver:   
✔ Glossário   
✔ Perguntas e respostas   
✔ Termos técnicos   
✔ Metadados

- 🔹 `<dl>` — Use quando é TERMO + EXPLICAÇÃO   
→ Trata-se de uma lista de definições (termo + explicação)   
→ “estou explicando algo”   

🧪 Exemplo
```html
<dl>
  <dt>HTML</dt>
  <dd>Linguagem de estruturação de páginas</dd>

  <dt>CSS</dt>
  <dd>Responsável pelo visual</dd>
</dl>
```

- 🚀 Conclusão   
`<dl>` → estrutura   
`<dt>` → termo   
`<dd>` → descrição   
   
👉 Usado para explicar coisas, não listar coisas