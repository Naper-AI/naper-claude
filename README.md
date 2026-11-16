# Naper Creator no Claude

**O seu braço direito de afiliados, dentro do Claude**, no Claude Code e no app do Claude (claude.ai, Desktop e
celular). O Claude lê os seus números, acha os produtos que estão vendendo, monta os seus posts e grupos e faz tudo por
você no [Naper Creator](https://creator.naper.ai/?utm_source=github&utm_medium=readme&utm_campaign=claude). Você
confirma antes de qualquer coisa sair.

> "Como estou este mês?" · "Analisa o meu TikTok e me diz o que postar" · "Me acha 10 produtos de beleza para divulgar"
> · "Monta a minha semana de posts" · "Revisa os meus grupos de WhatsApp" · "Liga o EU QUERO nos meus últimos posts"

## Ainda não usa o Naper Creator?

O Naper Creator é o app da creator de afiliados:

- **Posts:** rascunhos com o produto e a legenda prontos, agendados no Instagram, no TikTok, no Facebook, no Pinterest e
  na Shopee.
- **Grupos:** grupos de ofertas no WhatsApp que se enchem sozinhos, com o link pela sua página.
- **Radar de Oportunidades:** o que está vendendo na sua categoria, com a comissão de cada produto.
- **Números:** os ganhos de todos os canais num lugar só, com a meta do mês.
- **EU QUERO:** quem comenta recebe o link na DM.

**Comece de graça: conta nova ganha 7 dias do plano Creator.** Ao conectar o Claude pela primeira vez, você cria a conta
no caminho, com o número do WhatsApp, e volta para o Claude com o teste ativo.
[Criar a minha conta →](https://creator.naper.ai/?utm_source=github&utm_medium=readme&utm_campaign=claude) ·
[Ver os planos](https://creator.naper.ai/planos?utm_source=github&utm_medium=readme&utm_campaign=claude)

## Instalar

### App do Claude (claude.ai, Desktop, celular)

Configurações › Conectores › **Adicionar conector personalizado** › cole `https://api.naper.ai/mcp` › **Conectar**.

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

## Conectar a sua conta

1. O navegador abre em `creator.naper.ai`.
2. Entre com o seu número de WhatsApp (chega um código). Sem conta, ela é criada aqui.
3. Escolha as contas e o que o Claude pode fazer, e toque em **Autorizar**.

Nenhuma senha nem chave passa pelo terminal. Para ver ou desconectar: no app, **Conta › Claude e API**. Desconectar vale
em até 30 segundos.

## Roteiros prontos

São os pedidos mais comuns, prontos para usar. No app do Claude, ficam no **+** › **Naper Creator**. No Claude Code,
viram comandos:

| Roteiro | No Claude Code |
|---|---|
| Começar no Naper Creator | `/mcp__naper__primeiros_passos` |
| Como estou? | `/mcp__naper__como_estou` |
| Analisar meu perfil | `/mcp__naper__analisar_perfil` |
| Planejar minha semana | `/mcp__naper__planejar_semana` |
| Achar produtos para divulgar | `/mcp__naper__produtos_para_divulgar` |
| Revisar meus grupos | `/mcp__naper__revisar_grupos` |
| Configurar o EU QUERO | `/mcp__naper__configurar_eu_quero` |
| Criar um post | `/mcp__naper__criar_post` |

Também dá para pedir com as suas palavras. O Claude começa pelo panorama da conta e acha o resto.

## O que o Claude faz

| Área | O que dá para pedir |
|---|---|
| Panorama | Plano, créditos, redes, vendas e comissão, meta do mês, grupos, agenda e o que pede atenção, numa resposta |
| Perfil | TikTok e Instagram em números: os vídeos que mais venderam e os melhores dias, horários e formatos |
| Produtos | Radar da semana por categoria, achados do dia, busca de produtos, ficha e histórico de preço, vitrine |
| Posts | Rascunhos, produto vinculado, legenda gerada pela IA, publicar e agendar, reagendar e cancelar |
| Grupos | Criar e ajustar grupos, a fila do dia (pular, trocar, adiar, mandar agora), mandar uma oferta, números |
| EU QUERO | Ver e configurar, ligar por post, as respostas e os cliques |
| Agências | Várias contas num acesso: `contas_listar` e a conta em cada pedido |

Cada resposta traz o link da tela no app, para você conferir com foto e detalhes.

## Segurança e limites

- **Login:** é pelo navegador, com o código do WhatsApp. O Claude só usa as contas e as permissões que você marcou.
- **Ações:** o Claude mostra o que vai sair e pede o seu "pode" antes de publicar, agendar, mandar no grupo ou gastar
  crédito. O Claude Code também pergunta antes de cada ação.
- **Links:** o link que vai ao público é sempre o da sua página no Naper, nunca o da loja.
- **Limites de uso:** existem por minuto, conforme o plano, para proteger a sua conta e as suas redes. Quando bate no
  limite, o Claude espera e tenta de novo.

## Automações e devs

Crie uma **chave de API** no app (Conta › Claude e API) e use a REST em `https://api.naper.ai/v1`, com
`Authorization: Bearer naper_sk_…`. A documentação fica em https://api.naper.ai/docs e o resumo para agentes em
https://api.naper.ai/llms.txt.

---

Feito pela Naper. Termos: https://creator.naper.ai/termos · Privacidade: https://creator.naper.ai/privacidade
