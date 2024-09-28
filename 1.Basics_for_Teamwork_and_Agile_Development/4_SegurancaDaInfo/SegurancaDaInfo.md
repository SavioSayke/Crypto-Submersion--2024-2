# Segurança da Informação

![SegurançaDaInformacao](https://blog.compass.uol/wp-content/uploads/2023/07/CSIRT-A-Equipe-de-Resposta-a-Incidentes-de-Segurani-da-Informaiio-470x250.jpg)

## **O que é segurança da informação?**
De acordo com o NIST (National Institute of Standards and Technology) a segurança da Informação é a proteção de informações e sistemas de informação contra o acesso, o uso, a divulgação, a interrupção, a modificação ou a destruição não autorizados, a fim de fornecer confidencialidade, integridade e disponibilidade.

---

**Os pilares da Segurança de Informação**

A triade dos pilares de segurança da informação é o conjunto de tecnologias, processos e políticas que tem como finalidade manter as informações **confidenciais, integras e disponíveis.**

## <u>Confidencialidade</u>:
   * Para proteger a informação de acessos não autorizados, evitando situações de ataques por acesso indevido.
   * O objetivo é controlar o acesso por múltiplos fatores de autenticação e criptografias.

**É assim o dia a dia em autenticação!**

- Especificar requisitos mínimos para uma senha segura.
- Autenticação multifator.
- Verificação de senha fraca.
- Identificador e gerenciador de sessões.

## <u>Integridade</u>:
Esté é o pilar que devemos atender para manter as características originais dos dados, conforme sua criação.

A implementação de controles para impedir a alteração não autorizada devem ser pensados e implementados.

**Original e confiável é a regra aqui!**

- Validação de dados, como hashes.
- Verificação de duplicidade.
- Tratamento de dados de entrada, como caracteres especiais e comandos.

## <u>Disponibilidade</u>:
Queremos que os dados estejam disponíveis para o que for necessário, quando precisarmos. Isso demanda a estabilidade e acesso permanente ao ambiente e aos sistemas.

Pense aqui nos controles existentes para acessar e usar informações.

**A qualquer hora que precise!**

- Recursos de redundância, como backup de dados e balanceamento de carga.
- Infraestrutura de carga.
- Gestão de vulnerabilidades.

---

**A segurança da informação é responsabilidade de todos**

Você é quem faz nosso ambiente mais seguro e para isso precisa ao mínimo conhecer quais são nossas políticas e as principais diretrizes de segurança da informação.

Aprofundaremos nas principais diretrizes nos próximos módulos.

**Política de Segurança da Informação (PSI)**

Em nossa PSI você encontra as boas práticas a seguir para proteger as informações, tudo que estiver contrário a isso considere um incidente de segurança e deve ser reportado ao time InfoSec.

Nós, assim como todas as demais empresas do grupo, seguimos atualmente as orientações da PSI publicada pelo Grupo UOL que diz:

"A política de Segurança da Informação e Segurança Cibernética pretende (i) descrever as melhores práticas de Segurança da Informação e Segurança Cibernética quanto à confidencialidade, integridade e disponibilidade de informações; (ii) estabelecer diretrizes para todos os usuários, e (iii) minimizar os riscos de Segurança.

**Política de Classificação da Informação**

Para definir o controle mais adequado é necessário conhecer o tipo de informação, a sua criticidade e o público,

O melhor guia é a política de classificação da informação.

"Está política descreve o processo de classificação da informação, caracterizado pela definição do nível de sensibilidade e os grupos de acesso à informação, visando assegurar que esta receba um nível adequado de proteção, conforme seu valor, sensibilidade e criticadade para a organização."

---

## **Classificação da Informação**

“A classificação da informação tem como obtivo definir níveis de proteção que cada informação deve receber”. 

Toda e qualquer informação deve ser classificada, seja física ou lógica, de acordo com sua sensibilidade, criticidade e valor. A classificação deve tratar as informações durante o seu ciclo de vida, ou seja, sua criação, edição, compartilhamento, armazenamento e descarte.

**Por que classificar?**

Para aplicar a devida proteção das informações e reduzir a probabilidade de ocorrer incidentes.

O vazamento de informações, por exemplo, pode ocasionar impactos financeiro, regulatório e reputacional, trazendo sanções e prejuízos a Compass, seus clientes, parceiros e profissionais.

---

### **Níveis de Classificação**

**<u>Confidencial</u>**

São informações altamente sigilosas e que não podem ser divulgadas para evitar danos à empresa, terceiros, funcionários e clientes.

Seu uso requer medidas de controle e proteção rigorosos contra acessos, cópias, reproduções ou divulgações não autorizados.

Devido à sensibilidade dessas informações, várias restrições de uso são aplicadas e o destinatário consegue apenas consultar o documento.

**ATENÇÃO:** Sob está classificação, um possível vazamento de dados certamente causaria grandes danos à empresa.

**<u>Restrita</u>**

São informações exclusivas de alguns profissionais e/ou determinadas áreas. Significa que nem todos têm acesso à elas, pois os dados desta categoria são disponibilizados apenas aos destinatários nos quais você delega confiança para tratar do assunto.

_Exemplos_:
* E-mail com feedback;
* Divulgação de metas e resultados institucionais;
* Informações sobre produtos, serviços e projetos; Dados ou informações referentes às políticas comerciais.

**ATENÇÃO:** Sob está classificação, um possível vazamento de dados pode causar um impacto significativo à empresa, seus profissionais, seus parceiros ou seus clientes.

**<u>Interna</u>**

São informações que competem aos profissionais, estagiários, prestadores de serviços da empresa e precisam de cuidados para evitar a divulgação ao público externo.

_Exemplos:_
* Comunicados;
* Políticas e normas corporativas;
* Procedimentos operacionais e técnicos;
* Relação de endereços de e-mail internos;
* Informações disponibilizadas no Intranet.

**<u>Pública</u>**

São informações que podem ser divulgadas sem restrição para o público em geral, incluindo clientes, fornecedores, imprensa, concorrentes, entre outros.

As informações públicas são aqueles dados que podem ser divulgados sem oferecer risco algum à empresa, seus colaboradores e clientes.

---

## **Engenharia Social**

Engenharia Social é a habilidade de conseguir acesso a informações ou áreas importantes de algo ou alguém através de habilidades de persuasão.

O atacante se aproveita da faita de conhecimento, da boa vontade e simpatia da sua vítima para convencê-la a passar informações ou tomar ações de forma que lhe pareçam legítimas.

**Por que a engenharia social funciona?**

O ser humano confia e coopera por natureza, praticamente qualquer pessoa pode ser induzida a compartilhar informações, seja por capricho, carência de comunicação, coloca-se como centro das atenções, sentir-se útil, curiosidade, ambição, medo, compaixão, inocência, toda característica pode ser explorada com a abordagem correta.

Os investimentos para proteção das informações estão cada vez maiores e as tecnologias mais avançadas, com isso os fraudadores atacam o fator humano, a parte do processo de controles de segurança que tem menos atenção das empresas.

**_Tácticas de abordagem_**

As abordagens variam de acordo com a exposição do atacante, abaixo os mais comuns.

* **Baiting**: Uma isca física ou digital como um pendrive ou download de um filme, podem trazer um malware para o computador ao inserir o pendrive ou baixar e executar um arquivo, o malware oculto ganha acesso ao computador.
* **Phishing**: O mais famoso, porém, também mais eficiente! O atacante criar conteúdo enganoso muito próximo de algo legítimo e confiável, afim de obter credenciais ou instalar um malware. É comum se utilizar do e-mail, mas é muito comum também por SMS (Smishing) ou ligações de voz (Vishing).
* **Dumpster Diving**: é uma das abordagens menos óbvias, porém, caso as empresas não tenham cuidados com o descarte de informações o atacante pode encontrar relatórios inteiros, discos removíveis entre outros tipos de mídia com informações de todos os níveis de classificação.

**Dicas de prevenção**

"Ah, mas quem cai nisso? Como as pessoas não percebem que isso são estratégias para enganá-las?"

* Sempre desconfie! Leia de novo!;
* Não baixe arquivos e anexos em e-mail suspeitos;
* Não responda nem interaja com mensagens de textos suspeitas;
* Valide os links e o remetente dos e-mails;
* Descarte corretamente documentos e equipamentos;
* Pratique "mesa e tela limpa" ao menos o bloquear a tela e deixar o necessário em seu ambiente de trabalho.

---

## **Boas práticas e diretrizes**

Conheça alguns dos dilemas de segurança mais comuns em nosso dia-a-dia e saiba como lidar da melhor maneira para evitar interrupções, destruição ou modificação não autorizados, acesso e uso indevido ao trabalho que você tem se dedicado tanto.

**Compartilhamento de Acesso**

As credenciais de acesso, de qualquer sistema, constituem a identificação do usuário, isto é, se ele é autorizado a acessar e trabalhar aquelas informações.

As ações executadas com uma credencial são de responsabilidade do próprio profissional e todos os acessos podem ser monitorados, portanto proteja seu login e senha.

**Alerta de clichê!**

_"Não compartilhamos escova de dentes, assim também devemos fazer com credenciais de acesso."_

**Armazenamento**

As informações devem ser armazenadas nos repositórios oficiais, onde estarão seguras com os devidos controles de proteção.

Faça uso dos recurso da Udemy, do OneDrive e do Sharepoint de seu respectivo iStudio para armazenar suas informações.

**Softwares e malwares**

Softwares maliciosos e malwares são muito comuns em programas ou arquivos baixados da internet, portanto, é necessário ter muita cautela!

Nosso antivírus gera um alerta à todo software não autorizado e damos o devido tratamento envolvendo os profissionais e seus gestores, porém, o ideal é que você avalie sempre a lista de software homologados antes de instalar algo em seu equipamento.

**Dica de Ouro**: "Não assuma um risco sozinho, busque orientação."

Utilizar software não homologado pode gerar riscos desnecessários às nossas informações.

**Senha segura**

Suas senhas concedem o acesso ao ambiente e sistemas na Compass e em nossos clientes, por isso, é preciso seguir alguns cuidados básicos para criar uma senha forte.

* Evite nomes, sobrenomes, apelidos, datas de aniversário, nº de celular, placa de carro;
* Crie senha diferentes para cada conta, sistema ou site que precisar;
* Troque suas senhas com frequência;
* Use um aplicativo de "cofre de senhas";
* Sempre que disponível, utilize um segundo fator de autenticação (MFA);
* Reporte ao time InfoSec situações suspeitas que pedem suas informações;
* Sempre que possível use letras maiúsculas e minúsculas, números e caracteres especiais.

**Uso da internet**

O conteúdo acessado na internet e o uso do e-mail corporativo deve respeitar todas as diretrizes e nomes de segurança e privacidade publicadas e divulgadas em nossas políticas.

Com a disseminação de ferramentas de comunicação instatânea o uso destas para tratar assuntos profissionais se tornou cada vez mais comum. Evite-os para tratar assuntos sensíveis e compartilhar arquivos.

Quando precisar trafegar informação sensível, procure pelo "cadeadinho"!

> Conteúdo ilícito? Uma lista pra você se lembrar, mas não limitada a esta.

> Ataques, ameaças, violência, pornografia, spoofing, sniffer, defacement, disseminação de vírus, worms, trojans, spywares, spam, roubo de informação, espionagem, sabotagem, destruição, divulgação e alteração de informações não autorizadas, pirataria, engenharia reversa e/ou depuração de código não autorizado.

**Multi-factor Authenticator (MFA)**

MFA é um controle de segurança que demanda dois ou mais elementos de autenticação para identificar um usuário, afim de dificultar acessos não autorizados.

Existem diversos tipos de autenticação e os mais utilizados são:

| O que sei| O que tenho | Quem sou |
| --- | --- | --- |
| É exigido algo conhecido, como login, senha ou resposta a uma pergunta secreta. | Necessário algo físico como um token, um cartão inteligente ou um aplicativo em dispositivos móvel para obter a informação, geralmente randômica, para autenticação. | Utiliza-se características físicas do ser humano como a impressão digital, reconhecimento de voz ou face, ou leitura de retina. |

**Atualização de software**

Somos todos do mundo de tecnologia, e queremos sempre o melhor, o mais novo, o último modelo. **Por que seria diferente com os softwares e sistemas operacionais que utilizamos?**

Além das correções e proteção contra as novas vulnerabilidades identificadas pelos vendors, você tem ganhos em desempenho, compatibilidade, estabilidade, evita interrupções, aproveita de novos recursos e funcionalidades.

**Redes Wi-fi**

Quem nunca procurou uma rede Wi-fi aberta quando atingiu o limite do plano dde dados da sua operadora, que atire a primeira pedra.

Inúmeras vezes nos colocamos em risco nossas informações como senhas, históricos de navegação, e-mails, mensagens, dados e arquivos, simplesmente por utilizarmos um hotspot desconhecido, gratuito ou até mesmo com nomes muito convincentes ou semelhantes aos que costumamos usar.

É possível que alguém mal intencionado esteja bisbilhotando todos os pacotes que trafegam naquela rede aberta.

**Dicas valiosas para redes Wi-Fi públicas e domésticas**

**Em redes públicas**

* Evite se conectar a redes abertas;
* Utilize uma VPN confiável;
* Desative a opção de conexão automática nas redes Wi-fi públicas.
* Desative o compartilhamento de arquivos e impressoras.
* Não instale APPs que prometem quebrar senhas ou descobri-las para conectar a redes Wi-Wi protegidas.

**Em sua rede doméstica**

* Em seu roteador, configure uma senha forte, troque-a periodicamente, utilize os padrões WPA2 ou WPA3;
* Mantenha o firmware atualizado;
* Mude os padrões de fábrica como o nome da sua rede (SSID) e as credenciais de administrador do roteador;
* Desabilite o acesso remoto ao roteador para manutenção;
* Fique atento aos sites onde vai inserir informações confidenciais, confirme que utilizam conexões seguras (https)
  * Procure o cadeado na barra de endereços do navegador.

---