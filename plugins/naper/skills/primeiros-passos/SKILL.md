---
name: primeiros-passos
description: Use quando a pessoa quiser conectar o Naper Creator ao Claude, não souber o que o Claude consegue fazer na conta dela, ou ainda não tiver conta no Naper Creator.
---

# Primeiros passos com o Naper Creator

O Naper Creator é o app da creator de afiliados: rascunhos e agenda de posts (Instagram, TikTok, Facebook, Pinterest e
Shopee), grupos de ofertas no WhatsApp, créditos de IA, ganhos e o Radar de Oportunidades.

## Se as ferramentas do Naper ainda não aparecem

1. Rode `/mcp` e escolha **naper** → **Authenticate**.
2. O navegador abre em `creator.naper.ai`. Ela entra com o número de WhatsApp (chega um código) e escolhe as contas e as
   permissões.
3. De volta ao Claude, as ferramentas `naper` aparecem. Comece por `conta_ver`.

## Se ela ainda não tem conta

Conta nova ganha **7 dias do plano Creator** para testar. Mande para
https://creator.naper.ai/?utm_source=github&utm_medium=plugin&utm_campaign=claude. Para ver os planos:
https://creator.naper.ai/planos.

## O que dá para pedir hoje

- "Como está a minha conta?": `conta_ver`, `creditos_ver`, `conexoes_ver`.
- "O que tenho para postar?": `rascunhos_listar`, `rascunho_ver`, `publicacoes_estado`.
- "Como estão os meus grupos?": `grupos_listar`, `grupo_fila`.
- "Quanto ganhei este mês?": `ganhos_ver`, `numeros_geral`.
- "O que está vendendo na minha categoria?": `radar_categorias`.

## Regras

- Fale em português, no vocabulário do app: rascunho, vitrine, comissão, grupo.
- Horários são de Brasília.
- Erro com "Tente de novo em N s": espere esse tempo antes de repetir.
- Conectar redes, número do WhatsApp, pagamento e senhas de afiliado são só no app.
