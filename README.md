 Alltech

Landing page institucional da Alltech, uma empresa fictícia de serviços de TI. O projeto é totalmente estático, composto por duas páginas HTML e folhas de estilo CSS associadas.

## Visão geral
- **Público-alvo:** equipes de marketing ou produto que precisem de uma página institucional simples para apresentar serviços, clientes atendidos e um formulário de contato sem backend.
- **Páginas:**
  - `index.html`: página principal com seções de home, sobre, serviços, clientes e formulário de contato.
  - `cadastro.html`: formulário de cadastro de interesse (somente front-end, sem envio configurado).
- **Stack:** HTML5 e CSS3, com uso de [Font Awesome](https://cdnjs.com/libraries/font-awesome) via CDN para ícones.

## Estrutura do repositório
```
Alltech/
├─ image/                  # Logotipo principal
├─ templates/              # Folhas de estilo
│  ├─ style_index.css
│  └─ cadastro.css
├─ index.html              # Landing page principal
└─ cadastro.html           # Formulário de cadastro
```

## Pré-requisitos
- Navegador moderno (Chrome, Firefox, Edge ou similar).
- Opcional: Python 3 instalado para servir os arquivos via HTTP local.

## Como rodar localmente (≤10 minutos)
1. Clone ou baixe o repositório.
2. **Opção A: abrir diretamente no navegador**
   - Clique duas vezes em `index.html` para abrir o site.
3. **Opção B: servir via HTTP (recomendado para testes de rota âncora):**
   - No diretório do projeto, rode:
     ```bash
     python -m http.server 8000
     ```
   - Acesse `http://localhost:8000` no navegador.
4. Para ver o formulário de cadastro, navegue até `http://localhost:8000/cadastro.html` (ou abra o arquivo diretamente).

## Variáveis de ambiente
- Não há variáveis de ambiente ou arquivos de configuração ocultos. Toda a configuração está nos arquivos HTML/CSS.

## Comandos úteis
- Subir um servidor local simples (Python 3):
  ```bash
  python -m http.server 8000
  ```

## Deploy
- Por se tratar de um site estático, pode ser publicado em qualquer hospedagem de arquivos estáticos (ex.: GitHub Pages, Vercel, Netlify ou bucket S3). Basta enviar o conteúdo do repositório mantendo a estrutura de pastas.

## Limitações atuais
- Formulários (`index.html` e `cadastro.html`) não possuem backend configurado para envio real de dados.
- Não há testes automatizados ou pipeline de CI configurados.
