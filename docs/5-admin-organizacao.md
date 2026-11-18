---
title: 5. Administrador da Organização
nav_order: 6
permalink: /5-admin-organizacao/
---

# 5. Administrador da Organização — Estrutura, IA e Governança LGPD

## Por que isto importa

Cada organização tem sua própria topologia (diretorias, regionais, filiais, escolas ou unidades operacionais), sua política de uso de inteligência artificial, os dados do controlador dos dados pessoais e os termos que as pessoas aceitam. Os prazos de retenção são definidos pela plataforma (capítulo 6). O Katatu permite desenhar níveis livres sem limite de profundidade, proteger equipes pequenas contra identificação indireta e operar 100% funcional mesmo sem IA ativada.

## Configurar a organização

O assistente **Configurar a organização** é o caminho guiado para deixar a organização pronta para uso. Ele tem oito passos, em ordem:

1. **Identidade visual:** nome, logo e cores que aparecem nas telas e nos e-mails.
2. **Unidades da estrutura:** diretorias, escolas ou setores. Você digita uma a uma, lê a estrutura de um documento com a IA ou importa uma planilha.
3. **Cargos e posições:** cada cargo do organograma fica numa unidade e tem as posições que alguém ocupa.
4. **Catálogo:** competências, modelos de cargo e trilhas, e como cada um se liga aos cargos.
5. **Pessoas:** cadastrar pessoas sem acesso, por planilha, ou convidá-las.
6. **Papéis:** quem administra e quem gere cada unidade.
7. **IA (opcional):** chave própria ou franquia da plataforma. Pode ficar para depois.
8. **Calendário de ciclos:** a programação das campanhas de avaliação. Também pode ficar para depois.

Cada passo mostra para que serve, o que você vai precisar e o caminho mais curto até onde se resolve. Um passo se libera quando os passos de que depende estão feitos. Por exemplo, o Catálogo espera os Cargos, e os Papéis esperam as Pessoas e as Unidades. A IA e o Calendário podem ser feitos a qualquer momento.

- **Como um passo fica feito:** sozinho, quando o mínimo está cadastrado. Por exemplo, o passo de Unidades fica feito com a primeira unidade. Também dá para marcar um passo como feito à mão, desde que os passos de que ele depende estejam feitos.
- **Como pular:** qualquer passo pode ser pulado. Pular um passo não libera os passos que dependem dele. Marcar e pular podem ser desfeitos.
- **Quem vê:** só a Administração da organização vê o assistente.
- **Onde fica:** ao entrar pela primeira vez como Administração de uma organização nova, o assistente abre sozinho uma vez. Depois, a lista **Primeiros passos** aparece no Início, com o que falta e um link para cada passo; ela pode ser recolhida. O assistente também tem entrada fixa em **Configurações da Organização**.

**Dica:** o "?" ao lado de termos como cadeira, cargo, posição, referencial, modelo de cargo e trilha explica o significado do termo nas telas de Cargos, Catálogo e Mapa.

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
5. **Governança LGPD (`/governanca`, em Configurações da Organização):**
   - **Controlador dos dados pessoais:** informe o endereço completo e o canal de atendimento ao titular, que são obrigatórios. O encarregado de dados (DPO), com nome, e-mail e telefone, é opcional. Os dados passam a valer para as pessoas da organização ao salvar, e cada mudança fica registrada na auditoria.
   - **Termos e Política da organização:** publique a versão de cada documento. Quando uma versão nova muda o conteúdo, as pessoas da organização aceitam de novo no acesso seguinte. Uma versão pode ser marcada como correção, que não pede novo aceite. Quem publica vê quem ainda não aceitou.
   - **Prazos de retenção:** a organização não configura prazos. Eles são iguais para todas as organizações da plataforma e definidos pela Administração do Serviço.

![Tela de Estrutura Organizacional e Organograma em desktop](../assets/capturas/manual-06-estrutura-desktop.png)
![Tela de Assistência e Ingestão Multimodal em desktop](../assets/capturas/manual-07-assistencia-desktop.png)
