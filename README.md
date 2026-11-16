# Naper Creator no Claude

**A sua conta de creator de afiliados dentro do Claude** — no Claude Code e no app do Claude (claude.ai, Desktop e
celular). Peça em português e o Claude consulta e organiza a sua operação no
[Naper Creator](https://creator.naper.ai/?utm_source=github&utm_medium=readme&utm_campaign=claude).

> "Como foi a minha semana?" · "Quais rascunhos estão parados?" · "O que sai hoje nos meus grupos?" ·
> "Quanto ganhei de comissão este mês?"

## Ainda não usa o Naper Creator?

O Naper Creator é o app da creator de afiliados:

- **Posts:** rascunhos com o produto e a legenda prontos, agendados no Instagram, no TikTok, no Facebook, no Pinterest e
  na Shopee.
- **Grupos:** grupos de ofertas no WhatsApp que se enchem sozinhos.
- **Radar de Oportunidades:** o que está vendendo na sua categoria.
- **Números:** os ganhos de todos os canais num lugar só.

**Conta nova ganha 7 dias do plano Creator para testar.**
[Criar a minha conta →](https://creator.naper.ai/?utm_source=github&utm_medium=readme&utm_campaign=claude) ·
[Ver os planos](https://creator.naper.ai/planos?utm_source=github&utm_medium=readme&utm_campaign=claude)

## Instalar

### Claude Code

Pelo plugin, que traz a conexão e os roteiros prontos:

```text
/plugin marketplace add Naper-AI/naper-claude
/plugin install naper@naper
```

Ou só a conexão:

```bash
claude mcp add --transport http --scope user naper https://api.naper.ai/mcp
```

Depois rode `/mcp`, escolha **naper** e **Authenticate**.

### App do Claude (claude.ai, Desktop, celular)

Configurações › Conectores › **Adicionar conector personalizado** › cole `https://api.naper.ai/mcp` › **Conectar**.

## Conectar a sua conta

1. O navegador abre em `creator.naper.ai`.
2. Entre com o seu número de WhatsApp (chega um código).
3. Escolha as contas e o que o Claude pode fazer, e toque em **Autorizar**.

Nenhuma senha nem chave passa pelo terminal. Para ver ou desconectar: no app, **Conta › Claude e API**. Desconectar vale
em até 30 segundos.

## O que o Claude faz hoje

| Peça | Ferramentas |
|---|---|
| A conta, o plano e os créditos | `conta_ver`, `creditos_ver`, `creditos_extrato` |
| As redes conectadas | `conexoes_ver` |
| Os rascunhos e onde cada post vai sair | `rascunhos_listar`, `rascunho_ver`, `publicacoes_estado` |
| Os grupos de WhatsApp e a fila do dia | `grupos_listar`, `grupo_fila` |
| Os ganhos e os números de todos os canais | `ganhos_ver`, `numeros_geral` |
| O Radar de Oportunidades | `radar_categorias` |
| Várias contas (agências e equipes) | `contas_listar`, e a conta em cada pedido |

**Em seguida:** criar rascunhos, gerar legendas, agendar posts e mandar ofertas nos grupos, tudo pelo Claude.

## Segurança e limites

- **Login:** é pelo navegador, com o código do WhatsApp. O Claude só usa as contas e as permissões que você marcou.
- **Ações:** o Claude Code pergunta antes de cada ação, e você pode desconectar a qualquer momento no app.
- **Limites de uso:** existem por minuto, conforme o plano, para proteger a sua conta e as suas redes. Quando bater no
  limite, o Claude espera e tenta de novo.

## Automações e devs

Crie uma **chave de API** no app (Conta › Claude e API) e use a REST em `https://api.naper.ai/v1`, com
`Authorization: Bearer naper_sk_…`. A documentação fica em https://api.naper.ai/docs e o resumo para agentes em
https://api.naper.ai/llms.txt.

---

Feito pela Naper. Termos: https://creator.naper.ai/termos · Privacidade: https://creator.naper.ai/privacidade
