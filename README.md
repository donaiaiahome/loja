# Catálogo Dona Iaiá Home

Site estático com catálogo por ambientes, carrinho de compras, cadastro de nome e telefone, geração de PDF com fotos e preços, e botão para encaminhar resumo pelo WhatsApp.

## Publicação no GitHub Pages

1. Crie um repositório no GitHub (ex.: `dona-iaia-home`).
2. Envie **o conteúdo desta pasta** para a raiz do repositório: `index.html`, `app.js`, `products.json` e a pasta `assets`.
3. No repositório, acesse **Settings > Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**, branch `main`, pasta `/ (root)`, e salve.
5. Aguarde o endereço público indicado pelo GitHub.

## Manutenção

- `products.json`: dados dos produtos (`name`, `room`, `stock`, `price`, `image`). Preços são números, sem `R$`.
- `assets/`: fotos e logo.
- Atualize os arquivos no GitHub e aguarde a publicação.
- O carrinho fica no navegador do visitante (localStorage). **Não há reserva nem baixa de estoque compartilhada**.
- A geração do PDF usa jsPDF via CDN: **é necessária conexão com a internet** na primeira abertura. Para uso offline, hospede a biblioteca localmente.
- O botão WhatsApp envia um **resumo textual**; o PDF baixado deve ser anexado manualmente pelo cliente, pois o WhatsApp não permite anexá-lo automaticamente a partir de um site estático.
- Este é um **catálogo para solicitação de pedido**, sem pagamento integrado, banco de dados ou envio automático de pedido para a empresa.
- Para testar localmente, execute `python -m http.server 8000` dentro da pasta e abra `http://localhost:8000`.

## Dados comerciais

Ateliê Dona Iaiá Home · CNPJ 11.339.198/0002-30 · Rua Mosqueiro, 14, Dom Pedro — Manaus/AM · WhatsApp (92) 99318-8716.
