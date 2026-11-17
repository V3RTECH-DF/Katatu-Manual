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
3. **Publicar vagas e integrar canais** (em *Vagas*, pelo botão **Vagas no site**):
   - Gere versões do *Perfil da Vaga* adaptadas aos 5 estilos e 5 canais (sempre sobre a projeção pública fechada que nunca vaza campos internos da Matriz Situada).
   - Ative o mural incorporável ou publique direto no **WordPress** via REST API nativa (`wp/v2`) com *Application Password*, sem instalar plugin no site. Veja a conexão abaixo.

### Conectar o WordPress da organização

Quem administra a organização conecta o WordPress em **Vagas no site**, na seção **WordPress**.

1. Informe o endereço do site (precisa ser HTTPS) e o usuário que vai publicar as vagas.
2. Crie uma senha de aplicativo no WordPress, em **Usuários > Perfil > Senhas de aplicativo**, e cole-a no campo de senha do Katatu.
3. Escolha o tipo de post (o padrão é `posts`) e, se quiser, a categoria, pelo número dela no WordPress.
4. Ao salvar, o Katatu confere a conexão no site antes de gravar. A senha fica guardada de forma protegida: depois de salva, ninguém consegue vê-la de novo na tela.

**Trocar o site, trocar o usuário ou desligar e conectar outro site** é uma troca de destino e exige cuidado:

- O app pede a senha de aplicativo nova e a confirmação em duas etapas, feita agora.
- Ele registra o evento de segurança e avisa por e-mail todas as pessoas da Administração da organização.
- Os posts que já estão no site antigo continuam lá. A senha nova nunca vai para o site antigo.

**Dica:** se a conexão não for conferida, a vaga não é publicada e o app mostra o motivo. Não há um post "fantasma" no site.
4. **Acompanhar o Katatu Mapa (`/mapa`):**
   - Veja cada cargo com a cobertura de sucessão, a sobrecarga e a última avaliação, somados **por unidade**. Você vê números consolidados, sem nomes. Unidades com menos de 3 pessoas entram na soma da unidade de cima. A exportação em PDF, XLSX ou CSV segue o mesmo nível, sem nomes.
5. **Governança LGPD e Retenção (`Governança LGPD`):**
   - Configure os prazos de retenção de candidaturas não selecionadas (padrão: 365 dias) e logs de auditoria.
   - Antes de ativar um novo prazo, clique em **Simular Retenção (Modo de Ensaio)** para visualizar exatamente quantos registros seriam avisados (30 e 7 dias antes) ou eliminados, sem apagar nenhum dado real.

![Tela de Estrutura Organizacional e Organograma em desktop](../assets/capturas/manual-06-estrutura-desktop.png)
![Tela de Assistência e Ingestão Multimodal em desktop](../assets/capturas/manual-07-assistencia-desktop.png)
