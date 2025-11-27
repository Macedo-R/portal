# Portal IBS - Sete Lagoas/MG

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)

Centraliza informações, legislações, manuais e ferramentas sobre a Reforma Tributária do Consumo (EC 132/2023, LC 214/2025) para contadores e contribuintes do município. Projeto desenvolvido com foco em performance, acessibilidade e facilidade de manutenção.

## Funcionalidades

- **Busca Inteligente**: Motor de busca *client-side* que indexa conteúdo visível e metadados ocultos (comentários HTML) para resultados semanticamente relevantes.
- **Acessibilidade**: Conformidade com práticas de ARIA, alto contraste e navegação via teclado.
- **Design Responsivo**: Interface *Mobile First* adaptável a qualquer dispositivo.

## Estrutura do Projeto

O projeto é composto por páginas HTML estáticas, estilização CSS centralizada e lógica JavaScript modular.

### Páginas (HTML)

| Arquivo | Descrição |
| :--- | :--- |
| `index.html` | **Dashboard Principal**. Apresenta visão geral, cronograma de implementação (timeline horizontal) e acesso rápido aos serviços. |
| `material.html` | **Biblioteca Digital**. Contém o motor de busca (`SearchEngine`) e o acervo de manuais, notas técnicas e documentos. |
| `legislacao.html` | **Repositório Legal**. Lista organizada de leis, decretos, emendas constitucionais e normas técnicas. |
| `faq.html` | **Perguntas Frequentes**. Accordion interativo com respostas para as dúvidas mais comuns dos contribuintes. |
| `comunicado.html` | **Central de Avisos**. Publicação de comunicados oficiais, prazos e alertas importantes. |
| `videos.html` | **Galeria Multimídia**. Acervo de vídeos educativos, tutoriais e gravações de webinars. |
| `ibs.html` | **Sobre o IBS**. Informações detalhadas, alíquotas e regras específicas do Imposto sobre Bens e Serviços. |
| `nfse.html` | **Portal NFS-e**. Informações gerais sobre a Nota Fiscal de Serviços Eletrônica no padrão nacional. |
| `emitir-nfse.html` | **Guia de Emissão**. Passo a passo e links diretos para o ambiente de emissão de notas. |

### Recursos (Assets)

#### CSS (`/assets/css`)

- **`estilos.css`**: Arquivo de estilo monolítico que gerencia todo o design system.
  - **Variáveis (`:root`)**: Define paleta de cores, tipografia, espaçamentos e sombras.
  - **Reset & Base**: Normalização de estilos para consistência entre navegadores.
  - **Componentes**: Classes para botões, cards, timeline, accordions e inputs.
  - **Responsividade**: Media queries para adaptação a tablets e dispositivos móveis.

#### JavaScript (`/assets/js`)

- **`script.js`**: Núcleo lógico da aplicação.
  - **`SearchEngine`**: Classe responsável pela indexação e busca ponderada na biblioteca.
  - **Interatividade**: Gerencia abas (tabs), expansão de menus, modais e comportamento da timeline.
  - **DOM Manipulation**: Funções para renderização dinâmica de estados e feedback visual.

## Arquitetura da Busca (Search Engine)

O sistema utiliza uma classe proprietária `SearchEngine` (ES6) que opera inteiramente no navegador do cliente, eliminando a necessidade de banco de dados para esta finalidade.

## Instalação e Uso

Este é um projeto estático (HTML/CSS/JS). Não requer *build system* (Webpack, Vite, etc.).

1. Clone o repositório.
2. Abra o arquivo `index.html` diretamente em seu navegador.
3. Para desenvolvimento, recomenda-se o uso da extensão **Live Server** (VS Code) ou similar para *hot-reload*.

## Contribuindo

1. Adicione o novo link no arquivo `material.html` seguindo a estrutura de dados acima.
2. Garanta que o comentário de síntese contenha palavras-chave relevantes que não estão no título.
3. Verifique a renderização em dispositivos móveis.

## Registro de Domínio

© 2025 Prefeitura de Sete Lagoas — Todos os direitos reservados

## Créditos

**Prefeitura Municipal de Sete Lagoas**
Secretaria Municipal da Fazenda
