# Guia Rápido: Git & GitHub

Este projeto é um guia estático e rápido sobre os conceitos essenciais do Git e GitHub, incluindo termos, comandos básicos, fluxos de trabalho e como resolver conflitos.

## Estrutura do Projeto

O projeto é composto por dois arquivos principais:

1.  `index.html`: Contém toda a estrutura e o conteúdo textual do guia.
2.  `style.css`: Responsável pela estilização e pela apresentação visual da página.

## Documentação do Código

### `index.html`

O HTML está estruturado de forma semântica e organizada para garantir acessibilidade e clareza.

-   **`<head>`**:
    -   `meta charset="utf-8"`: Define a codificação de caracteres como UTF-8 para suportar acentuação.
    -   `meta name="viewport"`: Garante a responsividade em diferentes dispositivos.
    -   `title`: O título da página, exibido no navegador.
    -   `meta name="description"`: Uma breve descrição do conteúdo para mecanismos de busca.
    -   `link rel="stylesheet"`: Vincula o arquivo `style.css` para a estilização.

-   **`<body>`**:
    -   **`<header class="cabecalho-principal">`**: A área superior da página.
        -   `h1` e `p`: O título principal e o subtítulo do guia.
        -   `nav`: A navegação interna (Table of Contents) que leva às seções do guia.

    -   **`<main class="container">`**: Contém todo o conteúdo principal do guia.
        -   **`<section id="conceitos">`**:
            -   Detalha os conceitos básicos.
            -   Utiliza a classe `.duas-colunas` para organizar o conteúdo.
            -   O **Glossário** usa uma lista de definição (`<dl>`), o que é semanticamente mais adequado do que uma lista simples para associar termos (`<dt>`) a suas descrições (`<dd>`).
            -   Os **Comandos Essenciais** são exibidos em um bloco `<pre><code>` para manter a formatação do código.
        
        -   **`<section id="fluxos">`**:
            -   Explica os fluxos de trabalho `GitHub Flow` e `Git Flow`.
            -   Contém um bloco de aviso (`<div class="aviso dica">`) para destacar uma dica importante.
        
        -   **`<section id="conflitos">`**:
            -   Fornece um passo a passo para resolver conflitos.
            -   Contém um bloco de aviso (`<div class="aviso atencao">`) para destacar uma recomendação.

    -   **`<footer>`**:
        -   O rodapé da página com informações de direitos autorais.

### `style.css`

A folha de estilo utiliza variáveis CSS para facilitar a manutenção e a consistência visual do projeto.

-   **Variáveis CSS (`:root`)**:
    -   Define cores e outros valores reutilizáveis, como `var(--cor-primaria)`.

-   **Estilos Gerais**:
    -   `body`: Define a fonte (`'Roboto'`), cores de texto e fundo.
    -   `.container`: Centraliza e limita a largura do conteúdo principal.

-   **Layout de Colunas (`.duas-colunas`)**:
    -   O layout de colunas é implementado com `display: flex` e `flex-direction: column` para garantir que os elementos fiquem sempre um abaixo do outro em todos os tamanhos de tela.

-   **Tipografia e Formatação**:
    -   Estilos para títulos (`h1`, `h2`, `h3`) com cores e bordas para separação visual.
    -   Estilos específicos para as listas de definição (`dt`, `dd`).
    -   `pre` e `code`: Formatam os blocos de código com uma fonte monoespaçada (`'Roboto Mono'`) e fundo cinza claro.

-   **Avisos e Dicas**:
    -   As classes `.aviso`, `.dica` e `.atencao` dão um estilo visualmente distinto aos blocos de informação, usando ícones e cores diferentes para atrair a atenção do leitor.