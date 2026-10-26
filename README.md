# Guia do Calouro BCC

Site estático (HTML + CSS, sem build) para publicar no GitHub Pages.

## Publicar
1. Coloque o conteúdo desta pasta na raiz do repositório.
2. No GitHub: **Settings → Pages → Build and deployment**, escolha *Deploy from a branch*, branch `main`, pasta `/ (root)`.
3. Em alguns minutos o site fica em `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

O arquivo `.nojekyll` já está incluído para o GitHub servir os arquivos como estão.

## Adicionar um vídeo
1. Suba o vídeo no YouTube (pode ser "não listado").
2. Pegue o ID (a parte depois de `v=` no link).
3. Em `topicos/<tópico>.html`, troque a div `video-placeholder` pelo bloco em comentário logo abaixo dela, com o ID.
4. Na `index.html`, troque o selo "Vídeo em breve" do card por "Vídeo" (ou apague o selo).

## Escrever o texto
Em cada página de tópico, substitua a caixa "Rascunho" pelo texto final. Use `<h3>` para subtítulos, `<ul>` para listas e inclua os links das fontes oficiais.

## Estrutura
- `index.html`: página inicial com os tópicos por categoria
- `glossario.html`: siglas e termos
- `topicos/*.html`: uma página por tópico (vídeo + texto)
- `style.css`: estilos (cores no topo do arquivo, em `:root`)
