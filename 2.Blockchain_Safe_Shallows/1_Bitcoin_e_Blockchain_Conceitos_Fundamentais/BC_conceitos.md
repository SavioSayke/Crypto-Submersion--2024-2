# **Bitcoin e Blockchain - Conceitos Fundamentais**

## **Bitcoin**

Concebido durante o contexto da crise econômica de 2008, onde governos de vários lugares injetaram uma grande quantia em dinheiro para salvar instituições bancárias que estavam perto de quebrar e sem oferecer um retorno digno para a população que foi duramente afetada.

O **bitcoin** é uma unidade de troca, uma moeda digital descentralizada que usa uma combinação de tecnologias como blockchain, criptografia e engenharia de incentivo (consenso) se tornando, assim, um alternativa para pagamentos, comprar bens e serviços além do dinheiro convencional e ser uma reserva de valor.

Lembrando que o bitcoin não substitui totalmente o já consolidado sistema financeiro tradicional que consegue oferecer outras funções e serviços que, ainda, o bitcoin não consegue oferecer.

## **Diferenças entre: Bitcoin x Bancos**
| Características | Bitcoin | Bancos |
| --- | --- | --- |
| Confiabilidade | Blockchain | Centralizada |
| Armazenamento | 100% | Fracionado |
| Segurança | Criptográfica | Institucional |
| Emissão de moeda | Política econômica | Algorítmo |
| Transaççoes | Distribuído, peer-to-peer | Centralizado |
| Autenticação | Blockchain | Centralizado |
| Regulamentação | Ainda indefinida | Banco Central, normas |
| Processo de decisão | Consenso | Arbitrário |
| Controle do dinheiro | Você | Banco |

---

## **Blockchain**

Como o nome sugere, Blockchain é uma **cadeia de blocos** onde cada bloco contém uma série de dados, como: informações de transações ou algo que pode ser traduzido como dados de computador. Essa estrutura de blocos lineares é formada de modo que **cada bloco contenha informações que apontam para o bloco anterior** de modo que se algum dado de um bloco for alterado a cadeia quebre, garantindo assim a integridade da rede. Graças a uma função chamada **hash** que essa integridade pode ser alcançada.

O hash é uma função que recebe como entrada um **_input_ de qualquer tamanho** e retorna um **_output_ de tamanho fixo** e aparentemente aleatórias. Elas são essências para garantir a segurança da blockchain e possuí como principais características:

* **Sua facilidade de computar**
* **Livres de colisões** (praticamente impossível 2 _inputs_ ter o mesmo _output_)
* **Unidirecional** (praticamente impossível descobrir o input dado seu hash)
* **"Puzzle Friendly"** (ou seja, se eu realizar alterações nos meus dados, por mínima que seja, a saída do hash será diferente)

### **Assinaturas digitais**

As assinaturas digitais são uma forma de autenticar documentos no meio digital contendo transações, por exemplo. Sua principal característica é de ser única, já que apenas o dono da assinatura possa utilizá-la para validar uma transação. Cada assinatura é exclusiva para o documento ou transação, isso permite que qualquer pessoa verifique sua autenticidade de forma confiável. Isso é possível graças à combinação de um par chave pública/privada.

A **chave privada** é utilizada para gerar a assinatura digital e deve ser mantida em segurança e sigilo total, já a **chave pública** é compartilhada para que as pessoas possam verificar a validade da assinatura. Vale mencionar que é recomendado que o usuário sempre tenha mais que um par de chave pública/privada para se proteger de roubos e dividindo seus ativos, pois caso alguma chave privada seja violada ele não terá perda total de bens.

### **Criando uma moeda virtual**

A CentralCoin foi a moeda utilizada para explicar como funciona as moedas virtuais, em específico o bitcoin.

A principal diferença entra a CentralCoin e o Bitcoin é que na CentralCoin temos uma **autoridade central** que verifica as transações e mantém a blockchain, enquanto no Bitcoin as transações são feitas em uma rede descentralizada. São armazenadas as transações de criação e de transferência de moedas CentralCoins na sua blockchain.
Para efetuar as transações, o usuário deve informar quais moedas ele deseja utilizar (**destruir**) e quais os destinatários das novas moedas que vão ser **criadas** e adicionar a sua assinatura digital no processo. Vale lembrar que: a soma das moedas que vão ser destruídas deve ser maior que as que vão ser criadas.

Soma das moedas que serão **destruídas** **>** Soma das moedas que serão **criadas **

Essa diferença representa uma taxa de transação que geralmente é destinada aos usuários que validam elas na rede.

### **O bitcoin**

A rede Bitcoin foi feita para ser totalmente descentralizada, funcionando de acordo com um protocolo de consenso compartilhado por todos os usuários da rede. Nessa rede, os computadores conectados são chamados de **nós **(nodes), e existem dois tipos principais: os _full nodes_ e os _lite nodes_.

* **_Full nodes_**: São nós que armazenam uma cópia completa da blockchain, contendo todo o histórico de transações. Eles validam as transações e blocos emitidas pela rede e são essenciais para garantir a integridade e segurança da mesma.

* **_Lite nodes_**: São nós que não armazenam toda a blockchain, mas se conectam a _full nodes_ para realizar operações, tornando-se uma opção mais acessível para usuários com recursos limitados.

A comunicação entre os nós da rede é feita por meio de um protocolo conhecido como "protocolo de fofoca" (_gossip protocol_), onde cada nó repassa as transações que recebeu para outros nós. Essa abordagem distribui rapidamente as informações pela rede, assegurando que todos os nós estejam atualizados sobre as transações mais recentes.

### **Proof of Work**

Proof of Work é o mecanismo de consenso usado pela rede Bitcoin para validar transações e manter a segurança da blockchain. O processo envolve um cálculo complexo no qual os **mineradores competem** para encontrar um valor chamado **Nonce** (um número arbitrário qualquer) que, ao ser combinado com os dados do bloco, produz um hash que cumpre o critério de dificuldade da rede, normalmente exigindo que o hash comece com um número específico de zeros. O nível de dificuldade é ajustada para que a cada 10 minutos, aproximadamente, um novo bloco seja criado.

Ao encontrar o Nonce correto, esse bloco é transmitido pela rede para que outros possam validar sua veracidade. Caso o bloco seja aprovado, ele então é adicionado a cadeia de blocos na blockchain, porém, pode ser que dois mineradores acabem encontrando o Nonce do bloco ao mesmo tempo, a rede então escolherá o bloco que pertence a **cadeia mais longa** (com mais blocos subsequentes) e descartar o outro bloco.

Alguns mineradores visando facilitar esse trabalho realizam as chamadas **_mining pools_** que basicamente os mineradores trabalham em conjunto afim de minerar esses blocos de maneira mais efetiva e dividindo os ganhos de forma proporcional ao poder computacional de cada um.

