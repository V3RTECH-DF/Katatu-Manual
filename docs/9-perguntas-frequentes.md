---
title: Perguntas Frequentes
nav_order: 10
permalink: /9-perguntas-frequentes/
---

# Perguntas Frequentes (FAQ)

## 1. Por que uma pessoa com várias competências nível 3 ficou na Faixa 3 do *Katatu Fit*?
Porque o Katatu **não usa média compensatória**. Se uma competência essencial da função exige Piso `2` no Dia 1 e a evidência observada foi `1` (`delta_piso = -1`), uma nota máxima em outra competência não esconde essa lacuna. A pessoa entra na **Faixa 3**, indicando que ela pode assumir a função **desde que** a organização cadastre o amortecedor, o responsável e o prazo para cobrir aquela competência nos primeiros 90 dias.

## 2. O áudio que gravei na entrevista fica salvo no servidor da empresa?
**Não.** O Katatu segue a regra de **zero banco de voz**: o áudio existe apenas na memória volátil (RAM) durante os segundos necessários para gerar o rascunho de texto e é descartado imediatamente no bloco `finally`. Apenas o texto que você revisou e salvou na tela é armazenado.

## 3. Outra empresa que usa o Katatu consegue ver os certificados que subi na minha Carteira Pessoal?
**Não.** Todo certificado da sua Carteira Pessoal fica em quarentena por organização: a Organização B jamais toma conhecimento de documentos enviados na Organização A a menos que você autorize explicitamente o compartilhamento.

## 4. O que acontece se a chave de IA (BYOK) expirar ou a franquia acabar no meio de uma entrevista?
Nenhum fluxo trava. Todas as telas de estrutura, matriz situada, coleta e equivalência possuem modo manual imediato: se o provedor de IA retornar indisponibilidade (`503`), você preenche ou revisa os campos diretamente na tela sem perder dados.

## 5. O que acontece quando a licença `V3RLicense` da instalação expira?
Após os 14 dias de carência, a plataforma bloqueia **apenas** a abertura de novas vagas e novas campanhas (`402`). Todas as vagas já em andamento, planos *Katatu Gap* de 90 dias, *Katatu Mapa*, leituras e exportações (`PDF`, `XLSX`, `CSV` e portabilidade LGPD) continuam funcionando normalmente.

## 6. Por que a lista de competências está vazia ao criar um modelo de cargo ou uma trilha?
A lista mostra só os referenciais que valem para a unidade escolhida: os dela e os das unidades acima. Se o formulário avisa "Ainda não há nenhuma competência para escolher", não há referencial cadastrado nesse nível ou acima, ou todos estão arquivados. Use o botão **Cadastrar um referencial**, que abre o cadastro e depois volta ao formulário com o que você já tinha digitado. Confira também a coluna **Nível**: na **Organização inteira** só aparecem os referenciais da organização, e os cadastrados numa unidade não aparecem.

## 7. Importei a planilha da Estrutura e os modelos de cargo vieram sem competências. Isso está certo?
Hoje, sim. A importação cria um modelo de cargo para cada cargo da planilha, sem competências. Complete cada modelo em **Catálogo**, opção **Modelos de cargo**, antes de criar a Matriz do cargo. Se a Matriz já foi criada sem competências, acrescente-as nela enquanto ela estiver em rascunho. Uma vez oficializada, a Matriz não muda.

## 8. Cadastrei uma trilha, mas ela não aparece na Matriz. Por quê?
A trilha não entra sozinha. Na Matriz em rascunho, use **Sugerir do catálogo**, na seção **Trilha de aprendizagem**. Confira se a trilha vale para a unidade da Matriz: uma trilha de unidade irmã não aparece. Se a sugestão veio vazia ou com menos etapas do que você esperava, veja se o grau alvo de cada etapa está acima do piso e até o pleno da competência no modelo.

## 9. Posso apagar um referencial, modelo ou trilha que já está em uso?
Não. O sistema recusa e mostra o que usa o item. Arquive-o: ele deixa de ser oferecido, mas continua nas vagas, nos ciclos e nas Matrizes que já o usam. Só se apaga o que ninguém usa, e apagar é definitivo: o item não vai para a lixeira.

## 10. Mudei uma trilha ou um modelo. As vagas que já estão abertas mudam também?
Não. Uma vaga ou ciclo aberto continua na versão em que começou, e uma Matriz oficializada também não muda. A mudança vale para o que for aberto ou criado depois. Em cada item, **Ver as versões** mostra o histórico e qual versão está vigente.
