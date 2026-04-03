# 📚 Aula 03: [Listas em HTML]
---

## 🎯 Objetivo da Aula
- Aprender os tipos de listas
- Compreender a função de listas em HTML
- Compreender a estrutura das listas
- Estudar a forma correta de utilização 

## 📖 Conteúdos Abordados
- `<ul>` e `<ol>` com `<li>`
- `<dl>` com `<dt>` e `<dd>` 
--- 

## 💡 Conceitos Importantes
### Como são as listas em HTML?
- São uma forma de organização de informações usando tegs específicas para estruturar conteúdos em intens
- Principais tipos de listas:
- `<ul>` - Não ordenadas: Cria uma lista não ordenada com marcadores (bolinhas, quadrados)      
→ Use quando a ordem NÃO importa   
   
- `<ol>` - Ordenadas - numeradas: Cria uma lista ordenada, numerada automaticamente (número ou letras/romanos);   
→ Use quando a ordem IMPORTA
   
- `<li>` - Tag utilizada para os itens dentro de uma lista   
   
- `<dl>` - De descrição - Cria uma lista de definição ou descrição;  
    - `<dt>` - Define o termo na lista de descrição.
    - `<dd>` - Define a descrição do termo na lista de descrição.

- Tipo de lista que utiliza dois elemento casados   
→ Use quando é TERMO + EXPLICAÇÃO      
   
→ Pense: “estou explicando algo”   
      
      
🧪 Exemplos 
- Uso mais clássico:
```html
<dl>
  <dt>Cache</dt>
  <dd>Memória temporária para acesso rápido a dados.</dd>
  
  <dt>Cookies</dt>
  <dd>Pequenos arquivos salvos no navegador para identificar o usuário.</dd>
</dl>
```
- Metadados de um Produto ou Ficha Técnica
```html
<dl>
  <dt>Material</dt>
  <dd>Alumínio escovado</dd>
  
  <dt>Peso</dt>
  <dd>1.2 kg</dd>
  
  <dt>Garantia</dt>
  <dd>12 meses</dd>
</dl>
```
- Você pode colocar vários `<dd>` para um único `<dt>` ou vários `<dt>` para um único `<dd>`.   
   
🧪 Exemplo
```html
<dl>
  <dt>CSS</dt>
  <dd>Linguagem usada para estilizar páginas web.</dd>
  <dd>Sigla para "Cascading Style Sheets".</dd>
  <dd>O terror de muitos desenvolvedores iniciantes (brincadeira!).</dd>
</dl>
```
```html
<dl>
  <dt>Mouse</dt>
  <dt>Rato</dt>
  <dt>Trackpad</dt>
  <dd>Dispositivo periférico utilizado para controlar o cursor na tela.</dd>
  
  <dt>Login</dt>
  <dt>Entrar</dt>
  <dt>Sign In</dt>
  <dd>Ação de acessar uma conta protegida por credenciais.</dd>
</dl>
```
## 🛠 Exemplos Práticos