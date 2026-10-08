# Prospecção → Leads (atendimento rápido)

Abra `prospeccao.html` no navegador (Chrome ou Edge). Não precisa de servidor nem de instalação. Mantenha a pasta `sistema/` ao lado da pasta `fontes/`.

## Tela de Leads
- **Resumo no topo:** leads ativos, leads quentes, retornos para hoje e retornos atrasados.
- **Abas por etapa do funil:** Novo → Em contato → Proposta enviada → Negociação → Ganho / Perdido.
- **Ordem da lista:** primeiro os retornos atrasados, depois os de hoje, os leads novos e por fim os demais.
- **Busca** por nome, telefone ou cidade.
- **＋ Novo lead:** cadastre nome e telefone e clique em *Salvar e atender* para já abrir o atendimento.
- **⬇️ Exportar planilha:** gera um CSV que abre no Excel. Sirva-se dele também como backup.

## ⚡ Atender (painel de atendimento rápido)
O painel abre ao lado da lista. Você anota enquanto fala com o cliente.

1. **Topo:** botões de **WhatsApp** e **Ligar**, e um cronômetro do atendimento.
2. **Etapa e temperatura** (frio, morno ou quente).
3. **Registrar este contato:**
   - escolha o canal e o resultado com um clique;
   - escreva as anotações. As **frases rápidas** inserem textos comuns, como "Quer financiar.";
   - marque o **próximo passo** com data. Os atalhos *Hoje*, *Amanhã*, *+3 dias* etc. preenchem a data. Alguns resultados já sugerem o passo. Exemplo: *Não atendeu* sugere ligar de novo amanhã.
4. **Ficha do cliente:** conta de luz, concessionária, tipo de imóvel, telhado, pagamento e quem decide a compra. Ela **salva sozinha** enquanto você digita.
5. **Roteiro do atendimento:** checklist das perguntas que não podem faltar, com barra de progresso.
6. **Mensagens prontas de WhatsApp:** abrem o WhatsApp com o texto e o nome do cliente já preenchidos. Também dá para copiar o texto.
7. **Histórico:** linha do tempo com todos os contatos anteriores.

**💾 Salvar atendimento** (ou `Ctrl + Enter`) grava o contato no histórico e atualiza o próximo passo. A etapa muda sozinha nestes casos:
- *Novo* vira *Em contato* no primeiro contato;
- *Fechou negócio* vira *Ganho*;
- *Sem interesse* vira *Perdido*.

`Esc` fecha o painel.

## Onde ficam os dados
Os leads ficam salvos **no navegador deste computador** (localStorage). Outro computador ou navegador não vê os mesmos leads, e limpar os dados do navegador apaga tudo. Exporte a planilha de vez em quando como backup.

As listas de frases rápidas, roteiro, mensagens, origens e etapas ficam no início do `<script>` de `prospeccao.html` e podem ser ajustadas ali.
