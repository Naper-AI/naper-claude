# Naper Creator no Claude

**O seu braço direito de afiliados, dentro do Claude**, no Claude Code e no app do Claude (claude.ai, Desktop e
celular). O Claude lê os seus números, acha os produtos que estão vendendo, monta os seus posts e grupos e faz tudo por
você no [Naper Creator](https://creator.naper.ai/?utm_source=github&utm_medium=readme&utm_campaign=claude). Você
confirma antes de qualquer coisa sair.

> "Como estou este mês?" · "Analisa o meu TikTok e me diz o que postar" · "Me acha 10 produtos de beleza para divulgar"
> · "Quem mais vende em moda feminina?" · "Monta as ofertas do meu grupo para amanhã" · "Organiza a minha Bio" ·
> "Define a minha meta do mês" · "Liga o EU QUERO nos meus últimos posts"

## Ainda não usa o Naper Creator?

O Naper Creator é o app da creator de afiliados:

- **Posts:** rascunhos com o produto e a legenda prontos, agendados no Instagram, no TikTok, no Facebook, no Pinterest e
  na Shopee.
- **Grupos:** grupos de ofertas no WhatsApp que se enchem sozinhos, com o link pela sua página.
- **Bio:** a sua página do link da bio, com a vitrine, as coleções e os seus links.
- **Radar de Oportunidades:** o que está vendendo na sua categoria, com a comissão de cada produto e o ranking de quem
  mais vende.
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

São os pedidos mais comuns, prontos para usar. No Claude Code, digite `/` e o nome do roteiro: ele aparece como
`…:como_estou (MCP)`, e o que vier depois do nome vai junto (ex.: `produtos_para_divulgar beleza 5`).

| Roteiro | O que faz |
|---|---|
| `primeiros_passos` | O que já dá para fazer, o que falta ligar e o primeiro resultado de hoje |
| `como_estou` | Vendas e comissão, meta, redes, grupos e o que pede atenção agora |
| `meta_do_mes` | A meta do mês pela sugestão do app, e o que fazer por dia para chegar lá |
| `analisar_perfil` | O que dá alcance, o que vende e o que repetir no TikTok e no Instagram |
| `planejar_semana` | A agenda dos próximos 7 dias com os seus rascunhos e os produtos certos |
| `produtos_para_divulgar` | Os melhores produtos para divulgar agora, com o porquê |
| `quem_vende_mais` | O ranking das creators e das lojas da sua categoria, e o que aplicar |
| `organizar_bio` | O que subir, tirar e agrupar na sua Bio, com coleções prontas |
| `revisar_grupos` | O diagnóstico dos grupos de WhatsApp e os ajustes que trazem clique e venda |
| `ofertas_do_grupo` | Ofertas novas para o grupo, a agenda montada com você e agendada |
| `configurar_eu_quero` | Em quais posts ligar o EU QUERO, com a palavra e a mensagem |
| `criar_post` | Do produto ao post agendado |

Em qualquer Claude também dá para pedir com as suas palavras: o Claude começa pelo panorama da conta e acha o resto.

## O que o Claude faz

| Área | O que dá para pedir |
|---|---|
| Panorama | Plano, créditos, redes, vendas e comissão, meta do mês, grupos, agenda e o que pede atenção, numa resposta |
| Perfil | TikTok e Instagram em números: os vídeos que mais venderam e os melhores dias, horários e formatos |
| Meta | A meta do mês: o realizado, a projeção, a sugestão do app e definir a sua |
| Produtos | Radar da semana por categoria, ranking das creators e das lojas, achados do dia, busca, ficha e histórico de preço |
| Posts | Rascunhos, produto vinculado (direto do Radar), legenda gerada pela IA, a DM do EU QUERO, publicar, agendar e cancelar |
| Grupos | Buscar ofertas novas e montar a agenda com você, aprovar, a fila do dia (pular, trocar, juntar, adiar, mandar agora), criar e ajustar grupos, números |
| Bio | A vitrine e as coleções da sua página: pôr produto, subir, tirar, agrupar, a bio e os links |
| EU QUERO | Ver e configurar, ligar por post, as respostas e os cliques |
| Agências | Várias contas num acesso: `contas_listar` e a conta em cada pedido |

Cada resposta traz o link da tela no app, para você conferir com foto e detalhes.

## Segurança e limites

- **Login:** é pelo navegador, com o código do WhatsApp. O Claude só usa as contas e as permissões que você marcou.
- **Ações:** o Claude mostra o que vai sair e pede o seu "pode" antes de publicar, agendar, mandar no grupo, mudar a sua
  página ou gastar crédito. O Claude Code também pergunta antes de cada ação.
- **Links:** o link que vai ao público é sempre o da sua página no Naper, nunca o da loja.
- **Limites de uso:** existem por minuto, conforme o plano, para proteger a sua conta e as suas redes. Quando bate no
  limite, o Claude espera e tenta de novo.

## Automações e devs

Crie uma **chave de API** no app (Conta › Claude e API) e use a REST em `https://api.naper.ai/v1`, com
`Authorization: Bearer naper_sk_…`. A documentação fica em https://api.naper.ai/docs e o resumo para agentes em
https://api.naper.ai/llms.txt.

---

Feito pela Naper. Termos: https://creator.naper.ai/termos · Privacidade: https://creator.naper.ai/privacidade
