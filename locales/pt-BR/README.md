# Protocolo GUS

[English](../../README.md) | Português (Brasil)

Desenvolvido pelo analista brasileiro de dados e negócios Gustavo "Gus" Figueiredo.

GUS é um conjunto de instruções para que seu assistente de IA atue como um colaborador socrático: fazendo perguntas relevantes, ajudando você a pensar sobre um problema e sugerindo abordagens quando você quiser ajuda. Você participa do raciocínio e das decisões para entender e conseguir explicar o que produzem juntos.

A IA pode pesquisar, escrever e construir. Em tarefas mais longas, ela combina pequenas entregas com você, conclui uma delas e faz uma pausa para mostrar e discutir o trabalho antes de continuar. Perguntas simples continuam recebendo respostas diretas.

O objetivo é preservar o aprendizado e a curiosidade no uso da IA e evitar o hábito de entregar um trabalho que você não consegue explicar. Isso responde ao problema descrito por Molly Graham em [Lazy F'ing Interns](https://mollyg.substack.com/p/lazy-fucking-interns): repassar um trabalho sem compreensão ou discernimento suficientes. GUS amplia o Protocolo LFI do autor para o uso cotidiano, a escola, a universidade, a análise de negócios e o desenvolvimento de software.

## Como instalar

Você pode experimentar o GUS em uma conversa ou adotá-lo como seu modo habitual de trabalhar. As instruções são arquivos de texto comuns; você não precisa de um plugin nem de um modelo específico de IA. Esta versão usa português brasileiro, salvo se você pedir outro idioma. As referências de pesquisa continuam em inglês.

### Experimentar em uma conversa

No GitHub, clique em **Code → Download ZIP** e descompacte a pasta. Dentro dela, abra a subpasta **`locales/pt-BR/`** no seu agente de IA e envie:

```text
Leia profiles/general.md e use o Protocolo GUS nesta conversa. Responda em português brasileiro, salvo se eu pedir outro idioma. Reutilize os dados do parceiro já disponíveis. Na configuração inicial, apresente os perfis disponíveis e pergunte sobre meus principais usos, caso ainda não saiba; atenda primeiro a um pedido que já esteja claro. Pergunte apenas pelas preferências de interação que estiverem faltando e aplique o componente de voz quando pertinente. Se eu escolher um perfil especializado ou se minha tarefa claramente exigir um, leia protocol.md e esse perfil. Não instale nada nem altere minhas instruções padrão de trabalho.
```

Se você usa um chatbot que aceita anexos, anexe `profiles/general.md` dessa subpasta e peça que ele siga as instruções do arquivo. Comece com Geral / uso cotidiano; o agente apresentará os outros perfis. Se escolher um perfil especializado, forneça também `protocol.md` e o arquivo desse perfil. Inclua `components/voice.md` quando pertinente.

### Usar o GUS nas próximas conversas

Se seu agente consegue ler arquivos locais e editar suas instruções salvas, mantenha a pasta descompactada em um local permanente, abra **`locales/pt-BR/`** e envie:

```text
Configure o GUS como meu modo padrão de trabalho. Leia profiles/general.md nesta pasta. Encontre o arquivo de instruções pessoais que este aplicativo realmente carrega, preserve o conteúdo existente e acrescente uma instrução para ler o perfil Geral pelo caminho local absoluto. Use português brasileiro, salvo se eu pedir outro idioma, sem substituir preferências de idioma já registradas apenas por causa de uma mudança temporária. Mantenha os perfis especializados disponíveis para tarefas pertinentes. Reutilize meu registro de parceiro existente e leia a camada Parceiro em protocol.md antes de salvar preferências que estiverem faltando. Verifique as instruções salvas e me diga como conferi-las em uma nova conversa. Se este aplicativo não conseguir carregar esses arquivos entre conversas, explique isso em vez de afirmar que a configuração funcionou.
```

Em um chatbot com instruções personalizadas salvas, você pode colar o conteúdo de `profiles/general.md` ali, se couber. As referências a outros arquivos ainda exigem que esses arquivos estejam disponíveis na conversa. Caso contrário, anexe o perfil Geral ao iniciar um novo chat.

## Escolha um perfil

Comece com [Geral / uso cotidiano](profiles/general.md), um perfil curto que pode ser usado sozinho. Para um contexto especializado, combine o [protocolo compartilhado](protocol.md) com o perfil pertinente:

| Perfil | Para que usar |
| --- | --- |
| [Geral / uso cotidiano](profiles/general.md) (padrão) | Perguntas do dia a dia, curiosidade, planejamento pessoal, criação e conversa |
| [Escola](profiles/school.md) | Aprender matérias escolares, resolver exercícios e desenvolver explicações |
| [Universidade](profiles/university.md) | Estudos avançados, raciocínio da área, leitura de pesquisas e projetos acadêmicos |
| [Análise de negócios](profiles/workplace.md) | Aprender durante investigações e produzir um trabalho que a pessoa consiga explicar e assumir como seu |
| [Desenvolvimento de software](profiles/software-development.md) | Trabalhar em par com código, depuração e decisões técnicas, por meio de pequenas alterações funcionais revisadas em conjunto |

Na primeira configuração do parceiro, o agente apresenta os cinco perfis e pergunta para que você usa IA principalmente. Você pode escolher vários ou começar com Geral. Um pedido claro pode ser atendido primeiro; as perguntas de configuração não impedem uma resposta comum. Você pode mudar de perfil a qualquer momento.

O componente de [voz](components/voice.md) se aplica a todos os perfis. A configuração do parceiro registra a forma principal de interação e ativa as instruções de voz adequadas. Ditar uma mensagem e ouvir uma resposta são preferências distintas.

Para desenvolvimento de software, peça que o agente leia `protocol.md` e `profiles/software-development.md`. Juntos, percorram o comportamento relevante e combinem uma sequência curta de alterações funcionais. O agente implementa e verifica um incremento, mostra o comportamento e o código importante e faz uma pausa para discussão e autorização para continuar. A revisão em par e o rubber ducking — explicar o raciocínio em voz alta para examiná-lo — acontecem nos dois sentidos. As etapas seguintes se ajustam ao que vocês aprendem; aprovar o plano não elimina as pausas.

## Como a colaboração funciona

O [protocolo compartilhado](protocol.md#2-camadas-e-transições) define cinco camadas:

1. **Parceiro:** reutilizar ou estabelecer o nome da pessoa, seus principais usos, um perfil padrão opcional e suas preferências de interação.
2. **Contexto:** estabelecer o objetivo, o público e os requisitos; ler o material solicitado e, em seguida, convidar a pessoa a comentar ou oferecer ajuda para percorrê-lo. A reflexão é opcional.
3. **Investigação:** usar esse contexto para localizar o ponto de partida, escolher o apoio útil e combinar a próxima unidade de trabalho.
4. **Produção e aprendizado:** explicar ou construir o incremento aceito, verificá-lo, mostrá-lo e pausar para discussão e autorização antes do próximo.
5. **Validação (opcional):** oferecer comentários pertinentes ou ensaiar com um revisor interpretando o stakeholder ou destinatário do trabalho. O parceiro tem a oportunidade de explicar suas escolhas e os raciocínios importantes antes que o agente forneça respostas, para desenvolver seu domínio do trabalho. O parceiro decide o que mudar.

Retome no primeiro ponto ainda não resolvido. Reutilize o contexto disponível e não transforme um pedido mecânico específico em uma nova entrevista.

O perfil Geral resume essa abordagem para o uso cotidiano: responder diretamente a perguntas diretas, oferecer explicações ou ajuda para pensar quando útil, preservar o discernimento e a voz da pessoa e manter o trabalho proporcional ao pedido. Uma resposta simples pode estar completa sem uma aula. Trabalhos substanciais continuam sendo feitos em incrementos revisados.

## Modos de trabalho

O padrão é colaborativo: combinar incrementos significativos para trabalhos longos, concluir e mostrar um deles e pausar para ouvir o parceiro e receber autorização antes de iniciar o próximo. Um plano de várias etapas aprovado ainda inclui essas pausas.

Para uma emergência ou outra tarefa que precise de execução sem interrupções, diga algo como: **“Use o modo fire-and-forget para concluir o trabalho conforme o plano combinado.”** O agente conclui esse escopo sem perguntas de aprendizado nem pausas intermediárias de revisão, mantendo as verificações habituais e os limites de escopo. Essa alternativa termina com a tarefa; as seguintes voltam ao modo colaborativo. Veja as [regras de modos do protocolo](protocol.md#21-modos-de-trabalho).

## Registro do parceiro

O protocolo explica como reutilizar ou salvar um pequeno registro do parceiro no arquivo de instruções pessoais designado pela pessoa. Ele inclui os principais usos declarados, as preferências de interação e um perfil padrão apenas se tiver sido escolhido explicitamente. Um perfil escolhido para uma tarefa não se torna o padrão permanente; um padrão salvo se aplica quando for adequado à tarefa atual. Se nenhum arquivo pessoal tiver sido designado, use os dados na conversa atual e ofereça salvá-los sem impedir a tarefa. Salvar essas preferências não instala o GUS como modo padrão de trabalho nem armazena o histórico de tarefas. A mudança de idioma também não cria um novo registro ou reinicia a apresentação do parceiro.

## Pesquisa e fontes

As orientações de aprendizado se apoiam em quatro leituras: Cognitive Apprenticeship, o trabalho de Chi et al. sobre autoexplicação, o capítulo de Sweller sobre carga cognitiva e o trabalho de Bastani et al. sobre matemática com apoio de IA. As [notas sobre as fontes](../../references/source-notes.md) identificam os trechos pertinentes e explicam como eles orientam as instruções.

As instruções ajustam a orientação ao conhecimento prévio, usam autoexplicações focadas, oferecem um caminho que vai de exemplos resolvidos à resolução parcial e depois ao uso com menos apoio, verificam o conteúdo ensinado e consideram as exigências de memória da interação por voz. Essas fontes orientam o projeto; não demonstram a eficácia do GUS em si.

A [lista de leituras](../../references/reading-list.md) registra as fontes revisadas e sugere leituras adicionais. O capítulo de Sweller fundamenta as orientações de voz relacionadas às exigências de memória.

O perfil de desenvolvimento de software se apoia no [Manifesto Ágil](https://agilemanifesto.org/iso/ptbr/manifesto.html) e em seus [princípios](https://agilemanifesto.org/iso/ptbr/principles.html). Seu ciclo de trabalho em par e suas pausas obrigatórias de revisão aplicam esses princípios ao trabalho entre pessoa e agente. São escolhas de projeto do GUS, documentadas nas [notas sobre as fontes](../../references/source-notes.md#6-software-development-agile-principles).

## Licença e atribuição

Copyright © 2026 Gustavo "Gus" Figueiredo.

O Protocolo GUS é licenciado sob [Creative Commons Atribuição 4.0 Internacional (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). Consulte os termos completos em [LICENSE](../../LICENSE).

Ao compartilhar o protocolo ou adaptações, dê crédito ao autor, inclua links para a fonte e a licença e indique as alterações feitas. Sugestão de atribuição:

> Protocolo GUS, desenvolvido pelo analista brasileiro de dados e negócios Gustavo “Gus” Figueiredo. Licenciado sob [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

Essa licença abrange o texto original do protocolo. As publicações citadas mantêm suas respectivas licenças.
