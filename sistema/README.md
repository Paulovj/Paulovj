# Sistema Energizando House

Aplicação web local: basta abrir o arquivo `index.html` no navegador (Google Chrome ou Microsoft Edge). Não precisa de servidor, instalação nem internet. A internet só é usada para preencher o endereço pelo CEP.

> Mantenha a pasta `sistema/` ao lado da pasta `fontes/`, porque as etiquetas usam as fontes da marca.

## Menu Vendas → Etiqueta de entrega

Imprime **uma etiqueta por volume**, numerada `1/10`, `2/10` … `10/10`. Cada etiqueta traz:

- remetente e nº do pedido/NF;
- nome, endereço completo, CEP e telefone do destinatário;
- item(ns) da venda;
- data de entrega;
- número do volume em destaque.

### Como usar
1. Preencha o pedido, a quantidade de volumes e o item.
2. Digite o **CEP**: rua, bairro, cidade e UF são preenchidos sozinhos. Falta só o número.
3. Confira a pré-visualização e clique em **🖨️ Imprimir etiquetas**.
4. Para reimprimir, use **Últimas etiquetas → Carregar**, que guarda os 20 últimos envios.

Em **⚙️ Configurações** você escolhe o tamanho da etiqueta (100×50, 100×75, 100×100, 100×150 mm ou outro) e os dados do remetente. As configurações ficam salvas no navegador.

## Configurar a Elgin L42 (uma vez só)

1. **Driver:** instale o driver Windows da Elgin L42, disponível no site da Elgin, na área de suporte da impressora.
2. **Tamanho da etiqueta no driver:**
   1. No Windows, abra *Painel de Controle → Dispositivos e Impressoras*.
   2. Clique com o botão direito em **Elgin L42** e escolha *Preferências de impressão*.
   3. Crie um papel com o tamanho da sua etiqueta (ex.: 100 × 75 mm). Use o mesmo tamanho escolhido nas configurações do sistema.
   4. Em tipo de mídia, escolha **etiqueta com espaço (gap)** e o método de impressão que você usa: térmica direta ou com ribbon.
3. **Calibração:** depois de trocar o rolo, calibre o sensor de etiqueta conforme o manual da L42. Isso evita etiquetas impressas pela metade.
4. **Primeira impressão no Chrome/Edge:** na janela de impressão, configure:
   - Destino: **Elgin L42**
   - *Mais configurações* → Tamanho do papel: **o tamanho da etiqueta**
   - Margens: **Nenhuma**
   - Escala: **Padrão (100%)**
   - Desmarque **Cabeçalhos e rodapés**

   O navegador lembra dessas opções nas próximas vezes.

### Dica: imprimir sem a janela de impressão
Crie um atalho do Chrome com a opção `--kiosk-printing`. Com ela, o clique em "Imprimir" manda a etiqueta direto para a **impressora padrão** do Windows, sem perguntar nada:

```
"C:\Program Files\Google\Chrome\Application\chrome.exe" --kiosk-printing "C:\caminho\para\sistema\index.html"
```

Use esse atalho só se a Elgin L42 for a impressora padrão desse computador. Feche todas as janelas do Chrome antes de abrir pelo atalho.
