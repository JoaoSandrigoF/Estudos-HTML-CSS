# 📚 Aula: [Tags Textuais HTML]

## 🗓 Data [28/03/2026]

---
## 🎯 Objetivo da Aula
- Comprender as tags textua em HTML
- Compreender a forma correta de utilização de cada tag textual em HTML
- A utilização semantica de tags textuais 
---

## 📖 Conteúdos Abordados
|Abertura       | Fechamento        |
| :---          | ---:              |
|`<h1>` a `<h6>`| `</h1>` a `</h6>` | 
|`<p>`          | `</p>`            |
|`<strong>`     | `</strong>`       |
|`<em>`         | `</em>`           | 
|`<mark>`       | `</mark>`         |
|`<small>`      | `</small>`        |
|`<del>`        | `</del>`          |
|`<ins>`        | `</ins>`          |
---

## 💡 Tags
- **(`<h1>`até`<h6>`) Títulos:** Representam hierarquia de títulos na página.
    - Ex.:
    ```html 
        <h1>Título principal</h1>
        <h2>Subtítulo</h2>
        <h3>Subseção</h3>
    ```
    - ⚠️ Boas práticas
        - ✔ Use apenas 1 ``<h1>`` por página
        - ✔ Siga a ordem (h1 → h2 → h3…)
        - ❌ Não use só pelo tamanho

- **`<p>`:** Blocos de texto.
    - 💡 Dica: 👉 Cada ideia → um parágrafo
    - 🧪 Exemplo 
    ```html
        <p>Estou aprendendo HTML.</p>
    ```
---
- FORMATAÇÃO BÁSICA DE TEXTOS
    - **`<strong>`:** importância
    - **`<em>`:** Ênfase
    - **`<mark>`:** "Marcador" de texto - semelhante ao marcador de texto físico
    - **`<small>`:** Texto secundário - fica num tamanho menor

- PROPRIEDADES DE USO AVANÇADO `<ins>` e `<del>`
    - Essas tags não são só visuais — elas representam histórico de mudanças no conteúdo.
    - 👉 Muito usadas em: Sistemas de edição, E-commerce (preço antigo vs novo), Documentação, Versionamento.

    - 🔧 Atributos específicos

        - 📅 datetime: Indica quando a alteração aconteceu
        - 🧪 Exemplo
        ```html
            <ins datetime="2026-03-28"> Novo conteúdo </ins>
            <del datetime="2026-01-10"> Texto antigo </del>

            <p><small>- Formato correto e ano-mês-Dica <small></p>
            <p><small>- <ins">texto descritivo sobre a alteração`</ins>` <small></p>
        ```

        - 🎯 Quando usar\  
            ✔ Sistemas com histórico\  
            ✔ Conteúdo atualizado\ 
            ✔ Auditoria de mudanças\

        - 🔗 cite: Indica a origem da mudança: 
            - 👉 Um link explicando o motivo da alteração
            🧪 Exemplo
            ```html
                <del cite="https://meusite.com/atualizacao">
                    Informação antiga
                </del>
            ```

            - 🎯 Quando usar
                - ✔ Documentação técnica
                - ✔ Sistemas colaborativos
                - ✔ Conteúdo revisado    
                
- Ex.: 🧩 Uso profissional
    - E-commerce (muito comum)
        ```html
            <p>
                <del>R$ 199,90</del>
                <ins>R$ 129,90</ins>
            </p>
        ```
    - 👉 Aqui o significado é:
    - preço antigo → removido
    - preço novo → inserido

    - Atualização de conteúdo
        ```html
            <p>
                A versão atual é <del>1.0</del> <ins>2.0</ins>
            </p>
        ```

    - Documentação / revisão
        ```html
            <p>
                O prazo é de <del datetime="2026-01-01">5 dias</del>
                <ins datetime="2026-03-28">3 dias</ins>
            </p>
        ```

---
## 🛠 Exemplos Práticos
 ```html
    <article>
        <p>
            <del datetime="2026-01-01" cite="/mudancas">
             R$ 200,00
            </del>

            <ins datetime="2026-03-28" cite="/mudancas">
                R$ 150,00
            </ins>
        </p>
    </article>
    ```