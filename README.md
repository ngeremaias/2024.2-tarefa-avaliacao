# 2024.2 Avaliação do 1o período de Sistemas Operacionais
Nome: Jeremias Bezerra Lucas
## Informações gerais
- **Objetivo do repositório**: Avaliação do 1o bimestre da Disciplina de sistemas operacionais do curso de TADS do IFRN-CNAT
- **Público alvo**: alunos da disciplina de SO (Sistemas Operacionais) do curso de TADS (Superior em Tecnologia em Análise e Desenvolvimento de Sistemas) no CNAT-IFRN (Instituto Federal de Educação, Ciência e Tecnologia do Rio Grande do Norte - Campus Natal-Central).
- disciplina: **SO** Sistemas Operacionais
- professor: [Leonardo A. Minora](https://github.com/leonardo-minora)
- Nome: Jeremias Bezerra Lucas
## Avaliação
- **Lembre de fazer o fork deste repositório**
- As questões foram construídas com o auxílio do [copilot](https://copilot.microsoft.com/)

# Questão 1. Introdução a sistemas operacionais

Considere as funções e objetivos principais de um sistema operacional conforme discutido no texto. Explique como um sistema operacional gerencia os recursos de hardware e software de um computador para garantir eficiência e segurança. Em sua resposta, aborde os seguintes pontos:

- Gerenciamento de processos
   O SO gerencia a execução de processos, atribuindo tempo de CPU e gerenciando suas prioridades. Isso garante que múltiplos processos possam rodar simultaneamente, sem interferir uns nos outros. Exemplos práticos incluem o multitasking em sistemas como o Windows, onde vários aplicativos podem ser abertos ao mesmo tempo.
- Gerenciamento de memória
  O SO gerencia a alocação e liberação de memória para os processos. Isso é feito através de técnicas como a paginação e a segmentação, garantindo que os processos tenham a memória necessária sem interferir uns nos outros. Em sistemas modernos, como Linux e Windows, a memória virtual permite que os processos usem mais memória do que fisicamente disponível, utilizando disco rígido como extensão.
- Gerenciamento de dispositivos de entrada e saída
  O SO gerencia as interações com dispositivos de hardware, como impressoras e teclados. Isso é feito por meio de drivers, que atuam como intermediários entre o dispositivo físico e os processos do sistema. Por exemplo, ao imprimir um documento no Windows, o SO utiliza um driver de impressora para enviar os dados ao dispositivo.
- Gerenciamento de arquivos
  O SO organiza e controla o acesso a arquivos através de um sistema de arquivos. Ele mantém informações sobre a localização de arquivos no disco rígido e gerencia permissões de leitura e escrita. Em sistemas como o Linux e Windows, é possível configurar permissões de acesso para diferentes usuários a arquivos e pastas.

**Dica**: Pense em exemplos práticos de como o sistema operacional realiza essas tarefas no dia a dia de um usuário.

**Copilot informa**: Essa questão incentiva os alunos a explorarem os conceitos fundamentais e a aplicarem o conhecimento teórico em situações práticas. Se precisar de mais alguma coisa, estou aqui para ajudar!

# Questão 2. Estrutura de sistemas operacionais

## Texto informativo
### Estrutura de Sistemas Operacionais: Custo de Desenvolvimento e Segurança da Informação

A estrutura de um sistema operacional (SO) é fundamental para determinar tanto o custo de desenvolvimento e manutenção quanto a segurança da informação. Existem várias arquiteturas de SO, como monolítica, microkernel e em camadas, cada uma com suas próprias implicações em termos de custo e segurança.

#### Custo de Desenvolvimento e Manutenção

1. **Arquitetura Monolítica**:
   - **Desenvolvimento**: Geralmente, mais rápida de desenvolver inicialmente, pois todos os componentes do SO são integrados em um único bloco de código.
   - **Manutenção**: Pode ser mais complexa e cara, pois qualquer alteração em um componente pode afetar todo o sistema, exigindo testes extensivos e cuidadosos.

2. **Arquitetura Microkernel**:
   - **Desenvolvimento**: Pode ser mais demorada e cara inicialmente, pois envolve a criação de um núcleo mínimo e a implementação de serviços adicionais como processos separados.
   - **Manutenção**: Mais fácil e menos custosa, já que os componentes são isolados. Atualizações e correções podem ser feitas em módulos específicos sem impactar o núcleo do sistema.

3. **Arquitetura em Camadas**:
   - **Desenvolvimento**: Moderadamente complexa, pois cada camada deve ser bem definida e interagir corretamente com as outras.
   - **Manutenção**: Relativamente fácil, pois problemas podem ser isolados e corrigidos em camadas específicas sem afetar o restante do sistema.

#### Segurança da Informação

1. **Arquitetura Monolítica**:
   - **Segurança**: Pode ser mais vulnerável, pois uma falha em qualquer parte do sistema pode comprometer todo o SO. A integração de todos os componentes em um único bloco de código pode dificultar a implementação de medidas de segurança robustas.

2. **Arquitetura Microkernel**:
   - **Segurança**: Geralmente mais segura, pois isola os serviços em processos separados. Isso limita o impacto de uma falha ou ataque a um único componente, protegendo o núcleo do sistema e outros serviços.

3. **Arquitetura em Camadas**:
   - **Segurança**: Oferece um bom equilíbrio, pois cada camada pode implementar suas próprias medidas de segurança. No entanto, a comunicação entre camadas deve ser cuidadosamente gerenciada para evitar vulnerabilidades.

### Conclusão

A escolha da arquitetura de um sistema operacional tem um impacto significativo tanto no custo de desenvolvimento e manutenção quanto na segurança da informação. Arquiteturas monolíticas podem ser mais rápidas e baratas de desenvolver inicialmente, mas podem acarretar custos de manutenção mais altos e maiores riscos de segurança. Por outro lado, arquiteturas microkernel e em camadas podem exigir um investimento inicial maior, mas oferecem vantagens em termos de manutenção e segurança.

## Questão
Com base no texto sobre a estrutura de sistemas operacionais, analise como as diferentes arquiteturas (monolítica, microkernel e camadas) impactam o custo com a equipe de desenvolvimento e a segurança do sistema operacional. Em sua resposta, considere os seguintes pontos:
- Complexidade de implementação e manutenção
- Necessidade de especialização da equipe
- Potenciais vulnerabilidades de segurança
- Facilidade de atualização e correção de falhas

Arquitetura Monolítica:

Complexidade de Implementação: Menos complexa inicialmente, pois todos os componentes são integrados em um único bloco. Exemplo: Linux.
Manutenção: Mais cara e difícil, já que alterações em qualquer parte do sistema afetam o todo.
Segurança: Menos segura devido à alta interdependência entre os componentes, facilitando a propagação de falhas.

Arquitetura Microkernel:

Complexidade de Implementação: Mais demorada, pois o núcleo do sistema operacional é minimalista e os serviços são isolados.
Manutenção: Mais simples, pois a modificação de um módulo não afeta o núcleo do sistema.
Segurança: Mais segura, pois a falha em um módulo não compromete o núcleo ou outros módulos. Exemplo: Minix.

Arquitetura em Camadas:

Complexidade de Implementação: Moderada, pois as camadas precisam ser bem definidas e interagir corretamente.
Manutenção: Relativamente fácil, já que problemas podem ser isolados em camadas específicas.
Segurança: Equilibrada, pois cada camada pode ter suas próprias medidas de segurança, mas a comunicação entre elas deve ser bem controlada. Exemplo: Windows NT.

**Dica:** Utilize exemplos de sistemas operacionais reais que adotam essas arquiteturas para ilustrar sua análise.

**Copilot informa**: Essa questão incentiva os alunos a considerarem tanto os aspectos econômicos quanto os de segurança ao avaliar diferentes arquiteturas de sistemas operacionais.

# Questão 3. Introdução à Segurança de Sistemas Operacionais

## Texto informativo

A segurança de um sistema operacional é um aspecto crucial que visa proteger os recursos do sistema contra acessos não autorizados, ataques maliciosos e falhas. Um sistema operacional seguro deve garantir a integridade, confidencialidade e disponibilidade dos dados e serviços. Para alcançar esses objetivos, várias técnicas e mecanismos são implementados, incluindo:

1. **Controle de Acesso**: Define quem pode acessar o sistema e quais recursos podem ser utilizados. Isso é feito através de autenticação (verificação de identidade) e autorização (permissão de acesso).

2. **Criptografia**: Utilizada para proteger dados em trânsito e em repouso, garantindo que apenas usuários autorizados possam acessar informações sensíveis.

3. **Auditoria e Monitoramento**: Registra atividades do sistema para detectar e responder a comportamentos suspeitos ou anômalos.

4. **Isolamento de Processos**: Garante que os processos sejam executados em ambientes isolados, evitando que um processo comprometa a segurança de outro.

5. **Atualizações e Patches**: Manter o sistema operacional atualizado é essencial para corrigir vulnerabilidades conhecidas e proteger contra novas ameaças.


## Questão

Considerando os mecanismos de segurança discutidos, analise como a implementação de controles de acesso e criptografia pode impactar a performance e a usabilidade de um sistema operacional. Em sua resposta, aborde os seguintes pontos:
- Benefícios e desafios de cada mecanismo
- Impacto na experiência do usuário
- Exemplos de situações onde esses mecanismos são críticos

Controle de Acesso:

Benefícios: Protege dados e recursos, garantindo que apenas usuários autorizados acessem determinados arquivos ou funções.
Desafios: Pode adicionar sobrecarga no sistema, pois cada acesso precisa ser verificado.
Impacto na Experiência do Usuário: A usabilidade pode ser prejudicada, já que o usuário precisará autenticar-se constantemente.

Criptografia:

Benefícios: Protege dados sensíveis, garantindo a confidencialidade.
Desafios: Pode reduzir a performance, pois a criptografia e a descriptografia exigem poder de processamento.
Impacto na Experiência do Usuário: Pode resultar em latência, principalmente em sistemas com recursos limitados. Exemplo crítico: Armazenamento de senhas e dados bancários em sistemas como macOS e Linux.

**Dica:** Pense em como esses mecanismos são aplicados em sistemas operacionais que você utiliza no dia a dia, como Windows, Linux ou macOS.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre o equilíbrio entre segurança, performance e usabilidade, aplicando conceitos teóricos a contextos práticos.


# Questão 4. Custo de Processamento versus Algoritmo Ótimo de Escalonamento

## Texto informativo

O escalonamento de processos é uma função crítica de um sistema operacional, responsável por determinar a ordem em que os processos são executados pelo processador. O objetivo é maximizar a eficiência do sistema, garantindo que os recursos sejam utilizados de maneira justa e eficaz. No entanto, encontrar o algoritmo de escalonamento ótimo envolve um equilíbrio delicado entre o custo de processamento e a eficiência do escalonamento.

### Custo de Processamento

O custo de processamento refere-se ao tempo e aos recursos necessários para executar um algoritmo de escalonamento. Algoritmos mais complexos podem oferecer melhores resultados em termos de tempo de resposta e utilização do processador, mas também podem exigir mais recursos computacionais para tomar decisões de escalonamento. Isso pode incluir tempo de CPU, memória e outras operações de sistema.

### Algoritmo Ótimo de Escalonamento

Um algoritmo ótimo de escalonamento é aquele que maximiza a eficiência do sistema operacional, minimizando o tempo de espera dos processos, o tempo de resposta e o tempo de retorno. Alguns dos algoritmos de escalonamento mais comuns incluem:

- **First-Come, First-Served (FCFS)**: Simples e fácil de implementar, mas pode levar a longos tempos de espera para processos curtos.
- **Shortest Job Next (SJN)**: Minimiza o tempo médio de espera, mas pode ser difícil de implementar devido à necessidade de prever o tempo de execução dos processos.
- **Round Robin (RR)**: Oferece uma abordagem justa, atribuindo fatias de tempo iguais a todos os processos, mas pode resultar em maior sobrecarga de contexto.
- **Priority Scheduling**: Processos com maior prioridade são executados primeiro, mas pode levar à inanição de processos de baixa prioridade.

## Questão

Considerando os conceitos de custo de processamento e algoritmo ótimo de escalonamento, analise como diferentes algoritmos de escalonamento podem impactar a performance de um sistema operacional em termos de tempo de resposta, tempo de espera e utilização do processador. Em sua resposta, aborde os seguintes pontos:
- Vantagens e desvantagens de pelo menos dois algoritmos de escalonamento
- Impacto do custo de processamento na escolha do algoritmo
- Exemplos de situações onde um algoritmo pode ser preferível a outro

First-Come, First-Served (FCFS):

Vantagens: Simples de implementar.
Desvantagens: Pode causar longos tempos de espera, especialmente para processos curtos.
Impacto do Custo de Processamento: O custo de processamento é baixo, mas a eficiência no uso do processador pode ser comprometida.
Round Robin (RR):

Vantagens: Justo, pois distribui o tempo de CPU igualmente entre os processos.
Desvantagens: Pode resultar em uma sobrecarga de contexto (troca frequente de processos), afetando a performance.
Exemplos de Situação Preferível: Sistemas de uso geral, onde a equidade na alocação de CPU é importante.

Shortest Job Next (SJN):

Vantagens: Minimiza o tempo médio de espera.
Desvantagens: Difícil de implementar, pois requer previsão do tempo de execução dos processos.
Exemplos de Situação Preferível: Processamento de trabalhos em servidores de alto desempenho, onde a previsão de tempo é possível.

**Dica:** Pense em como esses algoritmos são aplicados em diferentes cenários, como sistemas de tempo real, servidores web e sistemas operacionais de uso geral.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre a complexidade e os trade-offs envolvidos na escolha de um algoritmo de escalonamento, aplicando conceitos teóricos a contextos práticos.

# Questão 5. Aplicativo em python vs aplicativos em c

## Questão

Explique o caminho que as instruções seguem desde um aplicativo escrito em Python e um aplicativo escrito em linguagem C até serem executadas pelo hardware. Em sua resposta, considere os seguintes pontos:
- O papel do interpretador no caso do Python
- O processo de compilação no caso do C
- A interação entre o kernel do sistema operacional e os drivers de dispositivo

  Python (Interpretado):

O código-fonte Python é lido pelo interpretador (como o CPython), que traduz as instruções para um formato intermediário (bytecode). O interpretador executa o bytecode no ambiente de execução, interagindo com o kernel do sistema operacional e usando drivers de dispositivo para realizar operações de entrada/saída. O Python não gera código binário diretamente, o que pode resultar em uma performance inferior.

  C (Compilado):

O código-fonte em C é compilado para código de máquina específico da arquitetura, criando um executável binário. Esse código binário é carregado pelo sistema operacional, que interage com o kernel e os drivers de dispositivo para executar as operações no hardware. O processo de compilação resulta em um código mais otimizado e executado diretamente pela CPU, oferecendo desempenho superior.
Comparação:

Python é mais flexível, mas mais lento devido à interpretação.
C é mais eficiente em termos de performance, pois gera código nativo, mas é mais difícil de desenvolver e depurar.
- A tradução final das instruções para o formato binário (0 e 1) executado pelo hardware

**Dica:** Compare e contraste os dois processos, destacando as principais diferenças e semelhanças na forma como as instruções são processadas e executadas.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre os diferentes caminhos que as instruções seguem em linguagens interpretadas e compiladas, aplicando conceitos teóricos a contextos práticos.
