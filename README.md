# Electro Tech — site institucional

Site de uma página (landing page) para a Electro Tech, instalações elétricas residenciais em Maputo.

## Estrutura de ficheiros

```
index.html        estrutura da página
css/styles.css     todo o estilo (cores e tipos centralizados no topo, em :root)
js/main.js         menu mobile, animações ao rolar a página
copy/copy.md        todo o texto do site, separado do código — edita aqui sem tocar no HTML
README.md           este ficheiro
```

## Como editar o texto

Abre `copy/copy.md`, muda o texto que quiseres, e depois copia a frase equivalente para o sítio certo em `index.html` (procura pelo texto atual com Ctrl+F). Não precisas de saber programar para isto — é só encontrar e substituir.

## Como mudar a logo, cores e contacto

- **Cores da marca:** abre `css/styles.css`, procura o bloco `:root{ }` no topo. A paleta segue o logótipo — branco, azul e cinza. As variáveis `--blue` (azul de destaque, usado em botões e nos traços de circuito) e `--bg` (fundo escuro) controlam a maior parte do visual do site — mudando aqui, muda em todo o site de uma vez.
- **Número de WhatsApp:** procura `258876508691` em `index.html` (aparece nos botões "WhatsApp"/"Falar no WhatsApp") e substitui pelo número correto, incluindo o código do país (258 para Moçambique).
- **Logo:** o logótipo atual é um ícone de raio (SVG) desenhado diretamente no código, junto com o texto "ElectroTech". Para trocar por uma logo própria, substitui o bloco `<svg>...</svg>` dentro de `.logo` por `<img src="caminho-para-a-tua-logo.png" alt="Electro Tech">`.

## Dados em falta

No ficheiro `copy/copy.md` e em `index.html`, há um marcador `[SUBSTITUIR]` na secção "Diferencial" — está reservado para um número real (anos de experiência ou quantidade de instalações feitas). Substitui assim que tiveres o dado; não deixes o marcador no site publicado.

## Como publicar (deploy grátis)

Opção mais simples — **Netlify Drop**:
1. Vai a https://app.netlify.com/drop
2. Arrasta a pasta inteira do projeto (com `index.html`, `css/`, `js/`) para a página.
3. Recebes um link público em segundos. Podes depois ligar um domínio próprio (ex: electrotech.co.mz) nas definições do site.

Alternativa — **GitHub Pages**: cria um repositório, envia estes ficheiros, e ativa "Pages" nas definições do repositório.

## Testado em

Mobile (~375px), tablet (~768px) e desktop (~1440px). O menu principal passa a menu de hambúrguer abaixo de 860px de largura.
