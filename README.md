# Controle Financeiro

App de controle financeiro em um único arquivo (`index.html`), feito para usar no celular.

## Publicar no GitHub Pages

1. Crie um repositório novo no GitHub (ex.: `financeiro`).
2. Clique em **Add file → Upload files** e envie o `index.html`.
3. Vá em **Settings → Pages**, em *Branch* escolha `main` e `/ (root)`, e salve.
4. Em 1–2 minutos o app fica disponível em `https://SEU-USUARIO.github.io/financeiro/`.
5. No celular, abra o link e use **Adicionar à tela inicial** (Chrome: menu ⋮ · Safari: botão compartilhar).

## Onde os dados ficam guardados

- **Por padrão**, os lançamentos ficam salvos no próprio navegador do aparelho. Eles **não** vão para o repositório — mesmo que o repositório seja público, ninguém vê seus dados.
- **Para usar no celular e no computador**, ative a sincronização em ⚙︎ Configurações:
  1. Crie um token em <https://github.com/settings/tokens/new?scopes=gist> marcando só **gist**.
  2. No primeiro aparelho: cole o token, deixe o ID do Gist vazio e toque em *Salvar e sincronizar*. Um Gist **privado** é criado e o ID aparece na tela.
  3. Nos outros aparelhos: cole o mesmo token **e** o ID do Gist.
  - O token fica salvo só no aparelho. Nunca coloque o token dentro do `index.html` nem no repositório.
- **Backup**: em ⚙︎ Configurações → *Exportar* baixa um arquivo `.json` com tudo. Faça isso de vez em quando (principalmente se não usar a sincronização). Limpar os dados do navegador apaga os lançamentos locais.

## Como usar no dia a dia

**Comece pela aba Cadastros:** cadastre os cartões (com o dia de fechamento e de vencimento), as pessoas e ajuste as categorias.

- **＋ Lançar** tem 3 tipos:
  - **Receita**: salário, PLR, 13º etc.
  - **Despesa**:
    - Forma de pagamento: Débito, Pix, Dinheiro ou Crédito. No crédito, você escolhe o cartão e o app calcula sozinho em qual fatura a compra entra.
    - **Parcelas**: escolha 2x, 3x… e diga se o valor digitado é o total ou o de cada parcela. As parcelas são lançadas automaticamente nos meses seguintes.
    - **Dividir despesa**: *Dividida* (você informa a parte da outra pessoa, o padrão é metade) ou *De outra pessoa* (a compra inteira é dela).
  - **Guardar**: dinheiro que você guardou ou resgatou (reserva, poupança, investimentos).
- **Contas fixas**: marque *Fixo* nas contas que se repetem. Ao virar o mês, toque em **↻ Copiar fixos** (entram como pendentes).
- Toque em qualquer lançamento para editar ou excluir. Em uma parcela, dá para aplicar a mudança às parcelas seguintes.
- **Visão geral do mês** (topo): totais do mês e o total de cada cartão. Toque no cartão para ver as compras da fatura e marcá-la como paga.
- **Check de pago**: toque no círculo ao lado de uma despesa para marcar ou desmarcar como paga. Na aba Lançamentos, use os filtros *Falta pagar* e *Pagos*.
- **Dashboard**:
  - **Contas do mês**: checklist do que já foi pago e do que falta, com uma linha por fatura de cartão.
  - **Previsão dos próximos 6 meses**: parcelas já lançadas + contas fixas do mês, com o saldo previsto.
  - **Quem me deve**: toque numa pessoa para ver o extrato e registrar um pagamento recebido.
  - Gastos por categoria (só a sua parte), formas de pagamento, receitas, dinheiro guardado acumulado e os últimos 12 meses.
