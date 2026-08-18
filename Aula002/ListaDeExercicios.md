1. A genealogia das linguagens não é uma escada de progresso. Explique essa afirmação e apresente dois fatores históricos que fazem uma linguagem influenciar outra sem necessariamente substituí-la. 
R: A afirmação significa que a evolução das linguagens de programação não segue uma linha reta e cumilativa, na qual uma nova linguagem surge simplesmente para tornar todaas as anteriores obsoletas e substituí-las. 
1° Fator: O Fortran foi concebido para computação científica de alto desempenho e o COBOL para aplicações comerciais e bancárias. Linguagens posteriores que herdaram conceitos imperativos ou de controle de fluxo não extinguram Fortran ou COBOL, pois estes já possuíam otimizações extremas e bibliotecas consolidadas em seus respectivos domínios.
2° Fator: Linguagens como C influenciaram profundamente a criação e a sintaxe de linguagens como C++, Java, C# e JavaScript. No entanto, C continua amplamnete utilizada até hoje devido à sua proximidade com o hardware, eficiência e base de código existente.

2. Plankalkül não foi implementada em sua época. Ainda assim, por que ela é relevante para a história das linguagens? Cite três recursos antecipados por seu projeto e explique o valor de um deles. 
R: Porque é historicamente relevante por extraordinariamente completa e precursora para o ano de 1945. Demonstra um conceito muito a frente de seu tempo, contendo algoritmos complexos e recursos de alto nível que só foramm reinventados ou apareceram em outras linguagens tempos depois.
1°: Estruturas de Dados Avançadas: Permitia a criação e alinhamento de registros (structs) e vetores.
2°: Controle de Fluxo Estruturado sem goto explícito: Sentença similar ao laço for da linguagem Ada, acompanhada pelo comando Fin para controle e saída de laços.
3°: Inclusão de Expressões de Relacionamento/Asserções: Expressões matemáticas que mostravam o que deveria ser verdadeiro durante a execução do programa em determinados pontos. 

A introdução de registros aninhados e vetores foi revolucionária porque permitiu agrupar e organizar dados heterogêneos sob uma única entidade abstrata, em vez de exigir que o programador manipulasse bits e endereços de memória isolados. Isso elevou o nível de abstração da programação, facilitando a modelagem de problemas do mundo real de forma muito mais legível e estruturada, servindo como o alicerce para o conceito de registros/estruturas (structs) e, mais tarde, para os objetos na computação.

3. Compare Short Code, Speedcoding e os sistemas A-0/A-1/A-2 quanto ao problema enfrentado e à estratégia adotada. Por que chamá-los simplesmente de compiladores modernos seria impreciso? 
R:
Problemas enfrentados:
O uso de códigos numéricos difíceis de memorizar e ler (em vez de nomes textuais).
O problema do endereçamento absoluto, em que a simples inserção ou remoção de uma instrução exigia recalcular manualmente todos os endereços de memória subsequentes.
A ausência de suporte de hardware para aritmética de ponto flutuante e indexação de vetores nas máquinas da época, exigindo que essas rotinas fossem implementadas manualmente.

Estratégias Adotadas:
Short Code, Interpretador Puro - Representava equações matemáticas convertendo operadores e variáveis em pequenos códigos numéricos de pares de bytes empacotados em palavras de memória. Não gerava código de máquina; executava as instruções por interpretação direta, simplificando a escrita ao custo de rodar cerca de 50 vezes mais devagar.
Speedcoding, Interpretador de Máquina Virtual - Transformava o computador IBM 701 em uma calculadora virtual de ponto flutuante de três endereços. Fornecia pseudoinstruções para operações transcendentais (raiz quadrada, seno, logaritmo) e auto-incremento de registradores de endereço, reduzindo semanas de programação para poucas horas, embora consumisse muita memória e tempo de processamento.
Sistemas A-0, A-1 e A-2, Expansor de Pseudocódigo - Em vez de interpretar a cada execução, o sistema pegava o pseudocódigo-fonte primitivo e o expandia em subprogramas em código de máquina, funcionando de maneira similar à expansão de macros em linguagens de montagem.

É incorreto chamar de compiladores modernos porque shortCode e Speedcoding não eram compiladores, mas interpretadores puros. Os sistemas A-0/A-1/A-2 eram sistemas primitivos de expansão de macros. 

4. Explique por que o projeto Fortran precisou convencer programadores de que código traduzido podia competir com código de máquina escrito à mão. Relacione desempenho, custo de programação e adoção. 
R: Porque a comunidade de desenvolvimento mantinha um forte ceticismo em relação a tradutores e linguagens de alto nível. As experiências anteriores com sistemas de interpretação de pseudocódigo eram marcadas por severa lentidão em tempo de execução. Muitos programadores da época preferiam a eficiência do código de máquina (ou em linguagem de montagem) escrito à mão e acreditavam que nenhum programa traduzido automaticamente conseguiria atingir um desempenho comparável.

Alto Custo do Hardware vs. Desempenho:
Naquele período, o custo dos computadores era exorbitante quando comparado ao custo dos programadores. As máquinas possuíam memória muito limitada e processamento lento. Por conta desse alto custo do tempo de máquina, qualquer perda considerável de desempenho em tempo de execução tornava inviável a utilização de uma ferramenta. Portanto, o desempenho do código objeto gerado era o objetivo primário absoluto.

Redução do Custo de Programação:
Embora o tempo de máquina fosse caro, programar diretamente em linguagem de máquina exigia enorme esforço manual e tempo de desenvolvimento. O Fortran propôs reduzir drasticamente o custo de programação ao permitir que cientistas e engenheiros expressassem problemas matemáticos com facilidade e menos esforço humano, aproximando a facilidade dos pseudocódigos da velocidade do código manual.

Impacto Direto na Adoção:
A adoção em larga escala só foi viabilizada porque o compilador Fortran cumpriu sua promessa de desempenho: entregou um código compilado altamente otimizado e próximo da eficiência manual, sem penalizar os recursos caros da máquina. Uma vez eliminado o medo da perda de performance, a vantagem da facilidade de programação fez a adoção disparar — tanto que, apenas um ano após o lançamento de Fortran I, cerca de metade do código escrito para o IBM 704 já era em Fortran.

5. Lisp surgiu em um contexto diferente de Fortran. Compare os domínios, a representação de dados e o estilo de computação favorecido pelas duas linguagens. 
R:

6. Avalie três contribuições de ALGOL 60 que ultrapassaram sua adoção comercial. Por que uma linguagem pode ser muito influente sem dominar o mercado? 
R:
Introdução da Estrutura de Bloco e Escopo Local:
ALGOL 60 introduziu formalmente o conceito de blocos de código delimitados (com suas próprias declarações de variáveis). Isso permitiu aos programadores criar ambientes de dados locais e controlar escopos, estabelecendo a base estrutural para praticamente todas as linguagens imperativas e orientadas a objetos posteriores (como C, Pascal, Java e C#).

Recursão em Linguagens Imperativas e Vetores Dinâmicos na Pilha:
Foi pioneira ao permitir subprogramas recursivos dentro do paradigma imperativo e ao introduzir vetores dinâmicos na pilha (cujo tamanho era determinado em tempo de execução ao alcançar a declaração). Essas inovações impulsionaram a teoria de gerenciamento de memória e influenciaram inclusive o desenvolvimento de novas arquiteturas de hardware baseadas em pilha (como as máquinas Burroughs B5000).

Formalização Sintática com a BNF (Backus-Naur Form):
ALGOL 60 foi a primeira linguagem a ter sua sintaxe descrita formalmente usando a notação BNF. Essa contribuição transcendeu a linguagem em si e fundou áreas inteiras da ciência da computação, incluindo a teoria de linguagens formais, análise sintática (parsing) e o projeto moderno de compiladores.

Uma linguagem pode atuar como um divisor de águas conceitual mesmo falhando em se consolidar comercialmente, devido ao descompasso entre inovação teórica e viabilidade prática/mercadológica

7. COBOL foi desenhada para processamento comercial. Mostre como domínio e público influenciaram sua legibilidade, seus registros e sua relação com FLOW-MATIC. 
R:

8. Compare Basic e PL/I como respostas ao desejo de ampliar o acesso ou o alcance da programação. Qual compromisso de projeto aparece em cada caso? 
R:

9. APL, SNOBOL e SIMULA 67 seguiram direções distintas. Associe cada linguagem ao seu foco e identifique uma contribuição duradoura de cada uma. 
R:

10. Defina ortogonalidade no projeto de linguagens e use ALGOL 68 para discutir a diferença entre regularidade e simplicidade. Uma linguagem muito ortogonal é automaticamente fácil de usar? 
R:

11. Construa uma cadeia de influência que passe por ALGOL, Pascal e C. Depois contraste essa linhagem imperativa com a proposta declarativa de Prolog. 
R: 

12. Modele em linguagem natural uma pequena base Prolog com dois fatos, uma regra e uma consulta. Explique por que isso representa programação lógica, não apenas armazenamento de dados. 
R:
Fato 1: Joanne é mãe de Jake (mae(joanne, jake)).
Fato 2: Vern é pai de Joanne (pai(vern, joanne)).
Regra: Uma pessoa $X$ é avô/avó de uma pessoa $Z$ se $X$ for progenitor(a) de $Y$ e $Y$ for progenitor(a) de $Z$ (avo(X, Z) :- progenitor(X, Y), progenitor(Y, Z)).
Consulta (Sentença-Objetivo): "Vern é avô de Jake?" (avo(vern, jake)).

O sistema utiliza uma técnica formal de inferência chamada resolução (baseada no cálculo de predicados) para avaliar as relações e regras, provando de forma automatizada a veracidade do objetivo proposto e respondendo se a sentença é verdadeira (true) ou falsa (false). O programador não precisa escrever um algoritmo instruindo a máquina sobre o caminho passo a passo de busca ("como fazer"). Ele apenas define as características formais do domínio e das relações ("o que é").

13. Ada resultou de requisitos e projeto em grande escala. Analise como confiabilidade, tipos, pacotes e concorrência se relacionam ao domínio de sistemas críticos. 
R:
Confiabilidade: Em sistemas críticos de tempo real, uma falha inesperada em tempo de execução não pode simplesmente abortar o sistema sem recuperação. Ada introduziu recursos robustos para tratamento de exceções, permitindo que os programadores detectem erros em tempo de execução e executem rotinas de contingência para manter o controle operacional do dispositivo controlado.

Tipos: Sistemas embarcados exigem garantia máxima de correção de dados antes mesmo da execução, evitando conversões implícitas perigosas ou cálculos com unidades incompatíveis. Ada adota uma tipagem estática e rigorosa, baseada na herança estruturada de Pascal. Além disso, oferece unidades genéricas (como procedimentos e pacotes parametrizados por tipo), permitindo construir algoritmos reutilizáveis e seguros sem abrir mão da verificação estrita de tipos em tempo de compilação.

Pacotes: Sistemas militares e aeroespaciais envolvem milhões de linhas de código construídas por grandes equipes multidisciplinares. Sem encapsulamento rígido, alterações locais podem corromper subsistemas críticos. Os pacotes (packages) fornecem uma barreira formal de encapsulamento, separando a especificação (interface pública) da implementação interna (ocultação de informação). Isso viabiliza a abstração de dados, minimiza efeitos colaterais indesejados e maximiza a manutenibilidade e o reuso de código.

Concorrência: Dispositivos embarcados interagem simultaneamente com múltiplos sensores, atuadores e eventos físicos externos em tempo real. Ada foi uma das primeiras linguagens a incorporar suporte nativo à execução concorrente por meio de unidades de programa chamadas tarefas (tasks). A comunicação e a sincronização entre processos paralelos são coordenadas de forma determinística por meio do mecanismo de rendezvous (e, posteriormente em Ada 95, por objetos protegidos), garantindo controle sobre a concorrência sem depender de artifícios inseguros do sistema operacional.

14. Compare o papel dos objetos em Smalltalk, C++ e Java. Inclua na resposta o compromisso de C++ com C e a estratégia de portabilidade de Java. 
R:
Smalltalk - Orientada a objetos pura: O mundo Smalltalk é constituído exclusivamente por objetos — desde inteiros e constantes escalares até grandes sistemas complexos. Toda computação ocorre por meio de envio uniforme de mensagens a objetos para disparar métodos. - Não há tipos primitivos isolados nem funções globais soltas. A vinculação dinâmica é total e a sintaxe é orientada a mensagens em vez das expressões imperativas tradicionais.
C++ - Linguagem híbrida (multiparadigma): Os objetos atuam como uma camada adicional sobre a base imperativa. Suporta tanto funções procedurais autocontidas clássicas quanto classes com métodos. - Coexistem dois mundos: tipos primitivos do C e tipos de classe. A orientação a objetos é opcional; o uso de polimorfismo exige declaração explícita de métodos virtuais (virtual), permitindo controle direto de alocação (na pilha ou no heap).
Java - Orientada a objetos baseada no paradigma imperativo: Todos os subprogramas devem ser obrigatoriamente métodos encapsulados dentro de classes; não existem funções globais avulsas como em C++. - Mantém a distinção entre tipos primitivos escalares e referências a objetos. Todos os objetos são alocados no heap e gerenciados por coleta de lixo (garbage collection), eliminando manipulação direta de ponteiros.

O projeto de C++ por Bjarne Stroustrup foi guiado pela premissa de compatibilidade quase total com C:

Sem penalidades de desempenho: O modelo de objetos foi desenhado para não gerar custo de tempo de execução (zero overhead principle) em comparação ao C tradicional. Por exemplo, recursos que diminuíssem a performance (como verificação de limites de vetores) foram evitados.

Compatibilidade e preservação de código: Praticamente nenhum recurso de C foi excluído, mantendo ponteiros brutos, tipos primitivos e compatibilidade direta para compilar e vincular bases de código C existentes. A herança de C permitiu adoção massiva imediata, embora tenha importado também suas vulnerabilidades e complexidades.

Para resolver o problema da dependência de hardware e viabilizar a execução segura em plataformas heterogêneas (e na Web), Java adotou uma estratégia em camadas:

Código Intermediário (Bytecode) e Máquina Virtual: O compilador Java não gera código de máquina nativo para um processador específico, mas traduz o código-fonte em bytecode intermediário neutro.

Execução via JVM / JIT: Cada arquitetura de destino requer apenas a implementação da Máquina Virtual Java (JVM) para interpretar o bytecode ou compilá-lo dinamicamente via compilação Just-in-Time (JIT) em código nativo.

Independência de Ambiente: Isso viabilizou o modelo de portabilidade "escreva uma vez, execute em qualquer lugar", acompanhado por um modelo de segurança que isola a execução (como nos applets de navegadores e servidores).

15. A primeira aplicação de Java não foi a Web, mas a Web impulsionou sua adoção. Explique como mudanças de contexto podem reposicionar uma linguagem. 
R: Aparecimento de novos ambientes e plataformas:
Uma linguagem desenhada para uma restrição (ex.: dispositivos com hardware heterogêneo) pode ter suas características aproveitadas por uma nova infraestrutura emergente (como a Web aberta, que também exigia independência de plataforma e execução segura em clientes remotos). Reaproveitamento de pilares de projeto em novos nichos:
Decisões voltadas à confiabilidade de hardware (como eliminação de ponteiros diretos, verificação de limites de vetores e coleta de lixo) tornaram o Java inerentemente resistente a falhas críticas, características que se mostraram essenciais para conter códigos maliciosos ou instabilidades dentro de navegadores Web e servidores distribuídos. Efeito multiplicador da disponibilidade e da demanda:
Mudanças no ecossistema (ferramentas gratuitas na internet, novos navegadores e a insatisfação com a complexidade de linguagens como C++) criam o ambiente ideal para que uma ferramenta encontre um mercado muito mais amplo do que aquele para o qual foi originalmente desenhada.

16. Compare Perl, JavaScript, PHP, Python, Ruby e Lua usando três eixos: domínio inicial, estruturas de dados e estratégia de implementação. Evite concluir que todas são iguais por serem chamadas de scripting. 
R: 

17. C# foi apresentada como evolução no ambiente .NET. Compare duas decisões de C# com suas correspondentes em Java ou C++ e explique o problema que pretendem resolver. 
R: Em C++: Callbacks e manipuladores eram implementados com ponteiros para funções/métodos, que compartilhavam a insegurança de memória típica dos ponteiros brutos.

Em Java: O tratamento de callbacks exigia a criação formal e verbosa de interfaces auxiliares e classes anônimas.

Permitir a implementação simples, direta e segura de manipuladores de eventos, execução de threads e rotinas de notificação/retorno (callbacks), eliminando tanto os riscos de violação de memória do C++ quanto a verbosidade indireta de classes/interfaces utilitárias do Java.

18. Diferencie XSLT e JSP quanto a entrada, processamento e saída. Por que ambas podem ser chamadas de linguagens híbridas de marcação e programação? 
R:

19. Crie uma linha do tempo com oito linguagens de pelo menos quatro paradigmas. Para cada ligação, escreva o tipo de influência; não use apenas setas cronológicas. 
R:

20. Estudo de caso: uma equipe precisa escolher tecnologias para cálculo científico, regras declarativas, aplicação Web interativa e firmware restrito. Proponha famílias de linguagens, justifique historicamente cada escolha e explicite dois trade-offs. 
R:

