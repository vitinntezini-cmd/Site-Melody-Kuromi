# Restaurante Melody e Kuromi

Site estático criado a partir do HTML enviado, com calculadora de vendas, cálculo de 30% do restaurante e temas claro e escuro.

## Executar

Abra `index.html` em um navegador ou inicie um servidor local:

```sh
cd /workspace/Site-Melody-Kuromi
python3 -m http.server 8000 --bind 0.0.0.0
```

Não há dependências para instalar nem etapa de compilação. Para hospedar o site, publique `index.html` e `favicon.ico` em um serviço de hospedagem estática.

## Publicar com GitHub Pages

No repositório do GitHub, abra **Settings → Pages**. Em **Build and deployment**, escolha **Deploy from a branch**, selecione a branch **main** e a pasta **/ (root)** e clique em **Save**.

Depois que a publicação terminar, o GitHub Pages mostrará o endereço do site. Os visitantes poderão acessar a calculadora sem fazer login. A conta do proprietário só é necessária para configurar e atualizar a hospedagem.

O arquivo `.nojekyll` indica que o conteúdo deve ser servido como site estático.

## Como usar

1. Selecione o produto e a quantidade.
2. Clique em **Adicionar item**. Remova um item com o botão **✕**, se necessário.
3. Clique em **Confirmar venda** para atualizar o acumulado e a parcela de 30%.
4. Use **TEMA** para alternar entre os temas claro e escuro.
5. Use **Limpar acumulado** para zerar o total após confirmar a ação.

O acumulado e a preferência de tema ficam no armazenamento local do navegador. Os dados não são compartilhados entre navegadores ou dispositivos; os itens da venda em andamento não são salvos ao atualizar a página.

O layout, os produtos, os preços e a lógica do HTML original foram preservados.
