# Produção & Custo — Sali Meres × Viamar Beach Wear

Ferramenta para cadastrar produtos, lançar a produção mensal e gerar o
documento de custos para a Viamar Beach Wear. É um único arquivo HTML,
sem instalação e sem servidor — funciona direto no navegador.

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (pode ser público ou privado — no
   privado o GitHub Pages exige um plano pago; se for usar de graça,
   crie como **público**).
2. Envie os arquivos deste projeto para o repositório. Duas formas:
   - **Pela web**: na página do repositório, clique em "Add file" →
     "Upload files" e arraste `index.html` (e este `README.md`).
   - **Pelo terminal**, dentro desta pasta:
     ```
     git init
     git add .
     git commit -m "Primeira versão do app"
     git branch -M main
     git remote add origin https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
     git push -u origin main
     ```
3. No repositório, vá em **Settings → Pages**.
4. Em "Build and deployment", escolha **Deploy from a branch**, selecione
   a branch `main` e a pasta `/ (root)`. Salve.
5. Em alguns minutos o GitHub mostra o link do site, algo como:
   `https://SEU-USUARIO.github.io/SEU-REPOSITORIO/`

Esse link funciona para qualquer pessoa, sem precisar de conta no
Claude — é só abrir no navegador do celular ou computador.

## Como atualizar o app depois

Sempre que eu (Claude) fizer um ajuste novo, basta substituir o arquivo
`index.html` deste repositório pelo arquivo atualizado e enviar de novo
(upload pela web ou `git add . && git commit -m "..." && git push`). O
GitHub Pages atualiza o site sozinho em seguida.

## Sobre os dados salvos

Como o GitHub Pages só hospeda arquivos estáticos (sem banco de dados),
os cadastros, lançamentos e o histórico ficam salvos no armazenamento
local do navegador (`localStorage`) de cada dispositivo que abrir o
site. Ou seja:

- Os dados **não são compartilhados automaticamente** entre o celular e
  o computador, nem entre pessoas diferentes — cada navegador guarda a
  sua própria cópia.
- Limpar os dados de navegação/cache do navegador apaga o histórico
  salvo ali.
- Para manter tudo em um único lugar, o ideal é sempre usar o mesmo
  navegador no mesmo aparelho para lançar a produção.

## Adicionar à tela inicial do celular

Abra o link do site em um navegador de verdade (Chrome, Safari) — não
dentro do WhatsApp — e use a opção "Adicionar à tela de início" do
navegador. Assim o app abre em tela cheia, como um aplicativo.
