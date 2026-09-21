
### Questão 1
**Enunciado:** A genealogia das linguagens não é uma escada de progresso. Explique essa afirmação e apresente dois fatores históricos que fazem uma linguagem influenciar outra sem necessariamente substituí-la.

**Resposta:** A genealogia das linguagens não é uma escada porque uma linguagem nova pode se inspirar em várias anteriores e, ainda assim, não eliminar nenhuma delas — elas passam a coexistir em nichos diferentes. **Fator 1 — Especialização por domínio:** linguagens se desenvolvem para resolver problemas distintos (computação científica, processamento comercial, IA simbólica), então Fortran, COBOL e Lisp seguiram caminhos paralelos, cada uma otimizada para seu domínio, sem que uma "vença" a outra. **Fator 2 — Inércia de adoção e legado:** investimentos já feitos em código, ferramentas e programadores treinados mantêm linguagens antigas vivas (COBOL ainda roda em sistemas bancários), então novas ideias costumam ser incorporadas por extensão a linguagens existentes em vez de substituí-las por completo — a influência flui sem substituição.

---

### Questão 4
**Enunciado:** Explique por que o projeto Fortran precisou convencer programadores de que código traduzido podia competir com código de máquina escrito à mão. Relacione desempenho, custo de programação e adoção.

**Resposta:** O time do Fortran (liderado por John Backus) precisou provar que o compilador gerava código quase tão eficiente quanto assembly escrito por especialistas, pois só assim a perda de desempenho seria aceitável frente ao ganho de produtividade. **Desempenho:** grande parte do esforço do projeto foi investido em otimizar o código objeto gerado pelo compilador, já que a comunidade científica/numérica era extremamente sensível a tempo de execução. **Custo de programação:** escrever em assembly era lento e propenso a erros; Fortran prometia reduzir o tempo de desenvolvimento por usar uma notação mais próxima da matemática. **Adoção:** só quando o desempenho do código compilado se tornou aceitável, as organizações passaram a trocar um pequeno custo de desempenho por um grande ganho de produtividade, o que tornou a adoção do Fortran viável.

---

### Questão 6
**Enunciado:** Avalie três contribuições de ALGOL 60 que ultrapassaram sua adoção comercial. Por que uma linguagem pode ser muito influente sem dominar o mercado?

**Resposta:** Três contribuições de ALGOL 60: (1) **Estrutura de blocos**, que introduziu escopos aninhados herdados por praticamente todas as linguagens estruturadas posteriores; (2) **Notação BNF**, que popularizou a definição formal de sintaxe, tornando-se padrão até hoje; (3) **Rigor em procedimentos e recursão**, que influenciou o projeto teórico de linguagens sucessoras como Pascal e C. Uma linguagem pode ser influente sem dominar o mercado porque sua influência se propaga por meio de projetistas de linguagens e do meio acadêmico — as ideias são absorvidas por sucessoras mesmo quando a linguagem original tem pouca adoção industrial.

---

### Questão 8
**Enunciado:** Compare Basic e PL/I como respostas ao desejo de ampliar o acesso ou o alcance da programação. Qual compromisso de projeto aparece em cada caso?

**Resposta:** **Basic** foi projetada para ampliar o *acesso* à programação — sintaxe simples, uso interativo, voltada a estudantes e usuários não especialistas; o compromisso é sacrificar poder de expressão e eficiência em favor da facilidade de aprendizado. **PL/I** foi projetada para ampliar o *alcance* de uma única linguagem, unindo os pontos fortes do Fortran (numérico) e do COBOL (comercial); o compromisso é ter se tornado uma linguagem grande e complexa, difícil de dominar por completo, justamente por tentar atender múltiplos domínios ao mesmo tempo. Em resumo: Basic troca poder por acessibilidade a iniciantes; PL/I troca simplicidade por abrangência de aplicação.

---

### Questão 10
**Enunciado:** Defina ortogonalidade no projeto de linguagens e use ALGOL 68 para discutir a diferença entre regularidade e simplicidade. Uma linguagem muito ortogonal é automaticamente fácil de usar?

**Resposta:** Ortogonalidade é a propriedade de projeto em que construções de linguagem podem ser combinadas em qualquer arranjo possível, sem restrições artificiais nem casos especiais — cada combinação produz um resultado previsível e significativo. ALGOL 68 levou a ortogonalidade a um extremo, permitindo combinar quase qualquer construção com qualquer outra, trazendo grande poder e regularidade, mas às custas de uma sintaxe complexa e difícil de ler/escrever. Regularidade significa consistência (sem exceções arbitrárias); simplicidade significa poucas construções, fáceis de aprender — uma linguagem pode ser altamente regular e, mesmo assim, nada simples. **Não**, uma linguagem muito ortogonal não é automaticamente fácil de usar: ortogonalidade traz poder e consistência, mas pode prejudicar usabilidade e legibilidade quando o espaço de combinações possíveis fica grande demais para o programador dominar.

---

### Questão 13
**Enunciado:** Ada resultou de requisitos e projeto em grande escala. Analise como confiabilidade, tipos, pacotes e concorrência se relacionam ao domínio de sistemas críticos.

**Resposta:** Ada nasceu de um processo de requisitos do Departamento de Defesa dos EUA, que buscava consolidar centenas de linguagens usadas em sistemas embarcados/militares em uma única linguagem padronizada. **Confiabilidade:** sistemas críticos exigem detectar erros antes da execução, pois falhas podem ser catastróficas — Ada prioriza checagem forte em compilação e tratamento robusto de exceções. **Tipos:** tipagem estática e forte reduz erros de tipo em execução, essencial em sistemas embarcados que rodam sem supervisão. **Pacotes:** o suporte a modularização via pacotes viabiliza projetos de grande escala com múltiplas equipes, com compilação separada e controle de interfaces. **Concorrência (tasking):** sistemas embarcados/tempo real monitoram múltiplos processos simultaneamente; Ada incorporou concorrência diretamente na linguagem, refletindo a natureza multiprocessos do domínio.

---

### Questão 14
**Enunciado:** Compare o papel dos objetos em Smalltalk, C++ e Java. Inclua na resposta o compromisso de C++ com C e a estratégia de portabilidade de Java.

**Resposta:** **Smalltalk:** tudo é objeto — orientação a objetos pura desde a concepção, com tipagem dinâmica, influenciando fortemente os conceitos de OOP adotados depois. **C++:** adicionou recursos de OOP *sobre* a linguagem C, priorizando compatibilidade com C para aproveitar código e programadores existentes; é uma linguagem híbrida multiparadigma em que OOP é opcional, não fundamental — trocando pureza por facilidade de adoção. **Java:** teve a portabilidade como objetivo central ("escreva uma vez, rode em qualquer lugar"), compilando para bytecode executado por uma máquina virtual (JVM); removeu complexidades de C++ (herança múltipla, ponteiros) em troca de mais segurança e independência de plataforma, ao custo de desempenho frente a código nativo.

---

### Questão 16
**Enunciado:** Compare Perl, JavaScript, PHP, Python, Ruby e Lua usando três eixos: domínio inicial, estruturas de dados e estratégia de implementação. Evite concluir que todas são iguais por serem chamadas de scripting.

**Resposta:** **Perl** — texto/administração Unix; arrays e hashes com regex forte; interpretada. **JavaScript** — scripting no navegador; objetos/arrays baseados em protótipos; interpretada/JIT nos motores de browser. **PHP** — geração de páginas no servidor; arrays associativos como estrutura central; interpretada. **Python** — scripting geral com foco em legibilidade; listas, dicionários e tuplas; interpretada (CPython). **Ruby** — uso geral com foco em produtividade; totalmente orientada a objetos; interpretada. **Lua** — scripting embutível (jogos, embarcados); estrutura única "table" versátil; interpretador leve embutível em C. Apesar do rótulo comum de "scripting", cada uma nasceu para um nicho distinto e adota uma filosofia diferente de estrutura de dados central — não são intercambiáveis.

---

### Questão 19
**Enunciado:** Crie uma linha do tempo com oito linguagens de pelo menos quatro paradigmas. Para cada ligação, escreva o tipo de influência; não use apenas setas cronológicas.

**Resposta:** Linguagens/paradigmas: Fortran (imperativo), Lisp (funcional), ALGOL 60 (imperativo estruturado), Simula 67 (OO — classes), Smalltalk (OO puro), Prolog (lógico), C++ (OO híbrido sobre C), Java (OO portável). Ligações: **Fortran → ALGOL 60** — influência de contraste/resposta (mais rigor estrutural e sintaxe formal). **ALGOL 60 → linguagens estruturadas seguintes** — influência estrutural/sintática (blocos, BNF). **Simula 67 → Smalltalk** — influência conceitual (classes/objetos tornados centrais e puros). **Smalltalk → C++** — influência de adaptação pragmática (OOP enxertada em linguagem imperativa existente). **C++ → Java** — influência de simplificação (mantém núcleo OOP, remove complexidades). **Lisp → Prolog** — influência paralela mas distinta (ambas de contexto de IA, mas paradigmas diferentes: funcional x lógico).

---

### Questão 20
**Enunciado:** Estudo de caso: uma equipe precisa escolher tecnologias para cálculo científico, regras declarativas, aplicação Web interativa e firmware restrito. Proponha famílias de linguagens, justifique historicamente cada escolha e explicite dois trade-offs.

**Resposta:** **Cálculo científico → família Fortran** (linguagens numéricas compiladas): criada especificamente para computação numérica de alto desempenho, com décadas de bibliotecas maduras. **Regras declarativas → família Prolog** (programação lógica): desenhada para expressar fatos, regras e consultas, e não passos procedurais. **Aplicação Web interativa → família JavaScript** (lado cliente): criada para dar comportamento dinâmico a navegadores, tornando-se padrão de fato pela adoção universal. **Firmware restrito → família C** (ou linguagens como Ada para confiabilidade): C oferece controle de baixo nível e eficiência próxima do hardware; Ada acrescenta determinismo para sistemas embarcados/tempo real. **Trade-off 1 (desempenho x produtividade):** linguagens compiladas de baixo nível (Fortran/C) ganham velocidade, mas custam mais tempo de desenvolvimento. **Trade-off 2 (flexibilidade x previsibilidade):** uma linguagem declarativa/lógica ganha poder expressivo para regras complexas, mas sacrifica previsibilidade de desempenho e facilidade de depuração.
