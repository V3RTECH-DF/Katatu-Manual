---
title: 5. Administrador da Organização
nav_order: 6
permalink: /5-admin-organizacao/
---

# 5. Administrador da Organização — Estrutura, IA e Governança LGPD

## Por que isto importa

Cada organização tem sua própria topologia (diretorias, regionais, filiais, escolas ou unidades operacionais), sua política de uso de inteligência artificial e seus prazos de retenção de dados pessoais. O Katatu permite desenhar níveis livres sem limite de profundidade, proteger equipes pequenas contra identificação indireta e operar 100% funcional mesmo sem IA ativada.

## Passo a passo

1. **Desenhar unidades e organograma (`Estrutura`):**
   - Crie unidades em qualquer profundidade (`unidades_fecho`) ou importe planilhas `CSV/XLSX` e imagens/PDFs de organograma pela **Ingestão Assistida** (tudo entra como **A confirmar**).
   - Configure o **Piso mínimo de agregação** (padrão: `3` ocupantes, mínimo irredutível: `2`): abaixo desse número, painéis agregados e campanhas 90º/180º/360º ocultam quebras nominais, incidentes críticos, amortecedores e nomes em Faixa 3.
2. **Configurar Assistência de IA e chaves próprias (`Assistência > Configuração e Consumo`):**
   - Escolha entre a franquia da assinatura V3RTECH, chaves próprias cifradas (**BYOK**: Google Gemini, OpenAI ou Anthropic Claude) ou modo **100% manual sem IA**.
   - Acompanhe o painel transparente de consumo filtrado por unidade, empresa-cliente, usuário e operação.
3. **Publicar vagas e integrar canais (`Divulgação`):**
   - Gere versões do *Perfil da Vaga* adaptadas aos 5 estilos e 5 canais (sempre sobre a projeção pública fechada que nunca vaza campos internos da Matriz Situada).
   - Ative o mural incorporável ou publique direto no **WordPress** via REST API nativa (`wp/v2`) com *Application Password*, sem instalar plugin no site.
4. **Governança LGPD e Retenção (`Governança LGPD`):**
   - Configure os prazos de retenção de candidaturas não selecionadas (padrão: 365 dias) e logs de auditoria.
   - Antes de ativar um novo prazo, clique em **Simular Retenção (Modo de Ensaio)** para visualizar exatamente quantos registros seriam avisados (30 e 7 dias antes) ou eliminados, sem apagar nenhum dado real.

![Tela de Estrutura Organizacional e Organograma em desktop](../assets/capturas/manual-06-estrutura-desktop.png)
![Tela de Assistência e Ingestão Multimodal em desktop](../assets/capturas/manual-07-assistencia-desktop.png)
