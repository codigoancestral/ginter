## Primeira Vez
#### Introdução

A integração entre sistemas, por meio da tecnologia “WebService”, garante a integridade, inviolabilidade e segurança dos processos judiciais, inclusive quanto ao sigilo processual, quando houver. O intercâmbio de dados é independente de implementações existentes em cada órgão ou instituições públicas ou privadas, podendo ser acessado por pessoas físicas, jurídicas ou entidades.

O Modelo Nacional de Interoperabilidade (MNI) representa o padrão para troca de informações processuais e estabelece as bases para o intercâmbio de informações de processos judiciais e assemelhados entre os diversos órgãos de administração da Justiça no âmbito do Poder Judiciário. O MNI foi implementado e é mantido pelo Conselho Nacional de Justiça.

Aos interessados em utilizar o MNI do PJe, cabe realizar as seguintes etapas:

Implementar as operações detalhadas do MNI em seus respectivos sistemas;
Solicitar ao TSE a criação dos vários perfis de usuários no PJe;
Consumir os serviços do webservice da instalação do PJe.

#### Primeiro passo: Criar os Usuários

O primeiro passo para realizar a integração entre os sistemas é entender o papel dos diversos usuários a serem criados no PJe e reunir os dados necessários para que se possa criá-los no ambiente de testes daquela aplicação.

Basicamente será necessário criar três perfis de usuários:

a) Usuário MNI (somente um usuário por instituição externa);

b) Usuário Procurador/Gestor (um ou vários);

c) Usuário Servidor de Cartório (dois usuários, um na capital e um no interior).

A criação desses usuários é realizada pelo Tribunal Superior Eleitoral utilizando-se os dados fornecidos pela instituição externa.

O papel de cada usuário e os dados necessários para a criação deles são os seguintes:

**a) Usuário de Interoperabilidade MNI**

Este é o usuário utilizado para a efetiva interoperabilidade técnica entre os sistemas da instituição externa e o PJe da Justiça Eleitoral.

No Pje (lado da Justiça Eleitoral na integração), o usuário de interoperabilidade MNI é criado com o perfil de Procurador/Gestor, perfil esse necessário para realizar-se a maioria das operações implementadas pelo protocolo MNI.

Para criar o usuário de interoperabilidade MNI, necessita-se de um CPF válido de Servidor/Procurador/Promotor/Policial da instituição externa. Este CPF será utilizado pela equipe de desenvolvimento de sistemas da instituição externa para ser inserido no código fonte do sistema que irá interoperar com o Pje (lado da instituição externa na integração).

A principal particularidade que deve-se ter em mente acerca do usuário de interoperabilidade MNI é que sua senha será definida pela equipe de desenvolvimento da instituição externa e portanto obviamente essa será de conhecimento da mesma, que a utilizará no código-fonte do sistema que irá interoperar com o PJe.

Em função disso recomendamos que esse CPF não seja de pessoa que irá utilizar o PJe para a prática de atos processuais.

Os dados necessários para criar o usuário de interoperabilidade MNI são:

* CPF válido de Servidor/Procurador/Promotor/Policial da instituição externa (somente um);
* E-mail (recomenda-se que esse e-mail seja de pessoa ou lista de discussão ligada a área de desenvolvimento de sistemas da instituição externa, pois é para esse email que o PJe envia o link para definição e redefinição de senha).

**b) Usuário com perfil de Procurador/Gestor**

O usuário Procurador/Gestor atua nos processos distribuídos para a sua Procuradoria. Pode-se ter um ou vários usuários com esse perfil no Pje. A quantidade de usuários a ser criada fica a critério da instituição externa.

Observação Importante: Os CPFs dos usuários Procuradores/Gestores devem ser diferentes do CPF do usuário MNI.

Os dados necessários para criar o usuário de interoperabilidade MNI são:

* CPF válido de Servidor/Procurador/Promotor/Policial da instituição externa;
* E-mail

**Observação:** Existindo usuários da instituição externa com o perfil de Procurador/Gestor já criados no Pje, não é necessário fazer esse procedimento novamente.

**c) Usuário com perfil de Servidor de Cartório**

Usuário lotado numa Zona Eleitoral que cria e atua nos processos da sua ZE. Serão criados até dois usuários com o perfil de Servidor de Cartório por instituição externa.

A Zona Eleitoral na qual o usuário Servidor de Cartório será lotado deve ser previamente escolhida pela instituição externa e informada ao TSE.

Pode ser qualquer Zona Eleitoral da capital ou do interior. Ex.: 015ª ZONA ELEITORAL DO RIO DE JANEIRO RJ.

**Observação:** Os CPFs dos usuários com perfil de Servidor de Cartório devem ser diferentes dos CPFs do usuário MNI e dos usuários com perfil de Procuradores/Gestores.

Os dados necessários para criar o usuário Servidor de Cartório são:

* CPF válido de Servidor/Procurador/Promotor/Policial da instituição externa;
* E-mail
* Número e nome da Zona Eleitoral na qual deseja-se lotar o usuário (a escolha da instituição externa).

**Resumo da Ópera**

**Criar usuário MNI**

* CPF válido de Servidor/Procurador/Promotor/Policial da instituição externa (somente um CPF);
* E-mail (recomenda-se que esse e-mail seja de pessoa ou lista de discussão ligada a área de desenvolvimento de sistemas da instituição externa, pois é para esse email que o PJe envia o link para definição e redefinição de senha).

**Criar usuário Procurador/Gestor**

* CPF válido de Servidor/Procurador/Promotor/Policial da instituição externa;
* E-mail.

**Criar usuário Servidor de Cartório**

* CPF válido de Servidor/Procurador/Promotor/Policial da instituição externa;
* Email;
* Número e nome da Zona Eleitoral na qual deseja-se lotar o usuário (a escolha da instituição externa).

#### Criando os Usuários
#### Criando os Usuários no Ambiente PJe de Treinamento (EAD)

Criando os Usuários no Ambiente PJe de Treinamento (EAD)
Para criar usuário em quaisquer dos ambientes de treinamento EAD, deve-se tão somente solicitar a criação dos usuários abrindo um chamado técnico no Service Desk do TSE.

Pode-se utilizar os seguintes canais de atendimento:

* Central de Atendimento do TSE: enviar e-mail para 8800@tse.ju.br
* Catálogo de Serviços: acessar o endereço [http://servicos.tse.jus.br/](http://servicos.tse.jus.br/)
* Opção: Soluções Judiciais
    * Serviço: PJE - Interoperabilidade com Sistemas Externos
    * Ação: Esclarecer Dúvidas

No corpo do e-mail ou no campo Descrição, informar os dados necessários para a criação dos usuários da instituição externa no PJe, de acordo com os campos a seguir:

* Solicitante: Nome da instituição externa
* Corpo do email ou campo descrição: informações detalhadas da solicitação
    * URL do PJe: informar a URL do sistema;
    * Tipo da Solicitação: Criação de Usuário
    * Dados de Cada Usuário:
        * CPF válido do usuário;
        * Email do usuário;
        * Perfil do usuário;
        * Nome e número do Zana Eleitoral (SOMENTE se o perfil for Servidor de Cartório).

#### Criando os Usuários no Ambiente PJe de Produção

Por motivos óbvios, a criação de usuários nos ambientes de produção do PJe requer um nível maior de segurança, controle e rastreabilidade. Em virtude disso, o cadastro de novos usuários nos ambientes de produção (1g, 2g e 3g), realiza-se seguindo o seguinte procedimento:

* Verificar se na própria instituição já tenham usuários cadastrados com o perfil de Procurador/Gestor, pois com esse perfil é possível o cadastro de novos usuários no Pje;
* Caso não existam usuários com o perfil mencionado no item anterior, encaminhar ofício a Presidência do TSE, com vistas a Assessoria do Processo Eletrônico (ASPJE), solicitando o cadastro dos novos usuários no PJe de Produção;
* Informar a instância desejada;
* Informar a URL do sistema PJe no qual deseja-se cadastrar os novos usuários;
* Para cada usuário, informar:
    * CPF válido;
    * Email;
    * Perfil desejado;
    * Nome e número do Zana Eleitoral (SOMENTE se o perfil for Servidor de Cartório).

#### Acessando o PJe

**a) Acesso manual**

O acesso ao PJe dá-se através de login e senha ou certificado digital A3 com token USB;

O acesso manual ao PJe, via certificado digital A3 com token USB, não exige senha previamente cadastrada no sistema, exige-se apenas a senha do certificado digital do usuário.

**b) Acesso via MNI**

As operações a serem realizadas no PJe utilizando-se o protocolo MNI, via sistema da instituição externa, realizam-se APENAS através de login e senha (autenticação sistema → sistema). A senha a ser inserida no código-fonte do sistema da instituição externa deve ter sido previamente cadastrada no sistema PJe;

**c) Definição e/ou alteração de senha**

Quando uma senha está prestes a expirar, já expirou ou deseja-se alterá-la, deve-se redefinir a senha por meio do botão “Esqueci minha senha” na tela de login do PJe. Após essa solicitação, o PJe encaminha para o e-mail do usuário cadastrado, um link para a definição / redefinição de senha.

## Dia a Dia da Interoperabilidade
#### Panorama do Suporte

Atualmente o TSE atende pedidos de integração, suporte técnico, negocial ou gerencial de uma gama de instituições externas: Ministérios Públicos Federal e Estaduais de todo o Brasil, Tribunais Regionais Federais e Justiças Comuns, Polícias Civis, Polícia Federal, Procuradorias Regionais, Procuradorias da Fazenda, Advocacia Geral da União, Supremo Tribunal Federal.

O PJe é composto por um conjunto de tecnologias
 interdependentes e nas quais atuam equipes de diversos setores das áreas de tecnologia da informação e negocial do TSE, o que sempre demanda esforço investigativo conjunto na solução das questões técnicas e negociais afetas ao PJe.

Dessa forma esperamos contar com a paciência, a boa vontade e a compreensão de todos na busca de soluções para cada instituição externa.

#### Abertura de Chamados de Suporte (Modelo Padrão)

Afim de facilitar o entendimento da solicitação de suporte e sua consequente solução por parte da equipe técnica, negocial ou gerencial do TSE, o Modelo de Abertura de Chamado de Suporte deverá seguido pelas instituições externas, quando solicitarem suporte para questões afetas a interoperabilidade entre os sistemas.

**Modelo de Abertura de Chamado de Suporte**

* Solicitante: Nome da Instituição
* Corpo do email: informações detalhadas da solicitação
    * URL do PJe: Endereço do sistema
    * URL do Webservice Intercomunicação: Endereço do webservice
    * Natureza da Solicitação: [Gerencial, Técnica, Negocial]
    * Tipo da Solicitação: [Erro, Dúvida, Sugestão de Melhoria]
    * Descrição da Solicitação: Detalhamento da solicitação

* Anexar a(s) requisições e respostas XML(s) utilizadas(s) pelo sistema da instituição externa para auxiliar nas investigações.

* Anexar documentos e/ou imagens da tela contendo detalhes visuais da solicitação. Print da tela cheia.

Pode-se utilizar os seguintes canais de atendimento para registrar um chamado para o Suporte do PJe:

* Central de Atendimento do TSE: enviar e-mail para 8800@tse.ju.br ou;

* Catálogo de Serviços: acessar o endereço [http://servicos.tse.jus.br/](http://servicos.tse.jus.br/)
    * Opção: Soluções Judiciais
    * Serviço: PJE - Interoperabilidade com Sistemas Externos
    * Escolher uma ação: Erro/Falha, Esclarecer Dúvidas, Indisponível, Lentidão

Uma vez registrado o chamado no Service Desk, esse será designado para a área capacitada a resolver a solicitação: Gerencial, Infraestrutura, Desenvolvimento, Banco de Dados, Negocial etc.

#### Resposta do Usuário ao Questionamento do Suporte do PJe

Por vezes, o Suporte do PJe necessita solicitar ao usuário do MNI, informações, documentos ou arquivos relevantes que auxiliem nas linhas de investigação de um chamado, podendo vir a auxiliar em sua solução.

O Suporte do PJe faz então um questionamento via sistema de gerenciamento de chamados e um email com tal questionamento é enviado ao usuário, contendo esse email um link para resposta.

Nem sempre o usuário consegue responder o questionamento ou enviar arquivos pelo link e nesse caso o usuário deverá abrir um novo chamado, utilizando-se dos mesmos canais mencionados no item anterior, informando o número do chamado o qual originou o questionamento e anexando as informações, documentos ou arquvivos solicitados.

#### Documentação do MNI

O MNI é um protocolo de comunicação desenvolvido e mantido pelo CNJ, cuja documentação por eles confeccionada, pode ser encontrada no endereço [http://www.pje.jus.br/wiki/index.php/Tutorial_MNI](http://www.pje.jus.br/wiki/index.php/Tutorial_MNI).

**Observação:** É a única documentação sobre o MNI disponibilizada pelo CNJ para consulta.

#### Como Criar Expedientes

Em linhas gerais os procedimentos necessários para criar expedientes no PJe são:

* Logar no PJe utilizando um usuário com o perfil de Servidor de Cartório;
* Usar a tarefa “Preparar Ato de Comunicação” para criar e enviar expedientes para o Ministério Público;
* O documento MNI - Enviar Expediente Para MPE.pdf é um guia geral para criação de expedientes. Apesar de ser um guia confeccionado visando o ambiente 3g e o perfil de usuário “Secretário Judiciário”, ele pode ser utilizado como um guia para o ambiente 1g devendo o usuário logado ter o perfil de Servidor de Cartório;

#### Como Preparar Documentos Para o Peticionamento via MNI

Na operação do webservice de intercomunicação entregarManifestaçãoProcessual() as vezes é necessário enviar documentos, principalmente PDFs, durante o peticionamento de processos. Os procedimentos necessários para preparar tais documentos, suas respectivas assinaturas e certificados digitais são:

* Converter os documentos para a codificação Base64, a qual é um método para codificação de dados para transferência na Internet. É utilizado frequentemente para transmitir dados binários por meios de transmissões que lidam apenas com texto, como por exemplo para enviar arquivos anexos por e-mail;
* Assinar os documentos convertidos para a codificacao Base64 utilizando um algoritmo de hash SHA256withRSA;
* Para assinatura dos documentos em Base64, utilizar um certificado com uma cadeia de certificado A1 ou A3 da ICP Brasil;
* A cadeia de certificado deve estar por padrão no formato PEM;
* Cada documento a ser peticionado deve conter sua assinatura individual;
* A operação pode conter tantos documentos quanto forem necessários;
* O arquivo MNI - entregarManifestaçãoProcessual – DocumentoAssinado.xml contém exemplo de documento convertido para a Base64 e assinado digitalmente com o algoritmo hash SHA256withRSA. O formato XML desse arquivo deve ser seguido a risca, devendo-se reproduzir fielmente a estrutura, a nomenclatura e o nível das tags, sob pena de não conseguir-se peticionar o processo com sucesso.

#### Tipos de Eleição

Na Justiça Eleitoral pode haver a ocorrência dos seguintes tipos de eleições, cujo código é utilizado na operação MNI entregarManifestaçãoProcessual(), por meio da tag JETipoEleição:

1. Eleições Gerais
2. Eleições Municipais
3. Eleições Complementares
4. Referendo
5. Plebiscito

#### Sigilo Processual

Consideram-se sigilosos, os processos:

1. Que, por lei, tramitem em segredo de justiça;

2. Que, em razão de decisão fundamentada da autoridade judicial competente, devam tramitar em segredo de justiça.

#### Níveis de Sigilo Processual
#### Zona Eleitoral (níveis 1, 3 e 5)

**Nível 1 (Segredo de Justiça)**

Visualização restrita aos serventuários da Zona Eleitoral, ao juiz eleitoral, ao polo ativo e seus representantes e aos membros do Ministério Público, como fiscal da lei. Nesse nível, tanto o serventuário que possui perfil de “servidor” quanto o serventuário que possui perfil de “servidor processamento” conseguirão visualizar o processo sigiloso. A expressão “representantes” contempla tanto os advogados quanto os defensores e/ou procuradores.

**Resumo Nível 1:**

* Juiz eleitoral;
* Servidor e servidor de processamento;
* Polo ativo e seus representantes (advogados, defensores, procuradores);
* Membros do Ministério Público, como fiscal da lei.

**Nível 3 (Sigilo Médio)**

Visualização restrita aos serventuários da Zona Eleitoral que possuem perfil de “servidor”, ao juiz eleitoral, ao polo ativo e seus representantes. Mais uma vez, a expressão “representantes” contempla tanto os advogados quanto os defensores e/ou procuradores.

**Resumo Nível 3:**

* Juiz eleitoral;
* Servidor;
* Polo ativo e seus representantes (advogados, defensores, procuradores);

**Observação:** No nível 3, caso necessário, o magistrado poderá atribuir visualização no processo ao polo passivo e aos membros do Ministério Público.

**Nível 5 (Sigilo Absoluto)**

Visualização restrita ao magistrado, polo ativo e seus representantes.

**Resumo Nível 5:**

* Juiz eleitoral;
* Polo ativo e seus representantes (advogados, defensores, procuradores);

**Observação:** No nível 5, caso necessário, o magistrado poderá atribuir visualização no processo ao polo passivo e aos membros do Ministério Público.

#### Tribunais Regionais Eleitorais e Tribunal Superior Eleitoral (níveis 1, 3, 4 e 5)

**Nível 1 (Segredo de Justiça)**

Visualização restrita aos serventuários da Zona Eleitoral, ao juiz eleitoral, ao polo ativo e seus representantes e aos membros do Ministério Público, como fiscal da lei. Nesse nível, tanto o serventuário que possui perfil de “servidor” quanto o serventuário que possui perfil de “servidor processamento” conseguirão visualizar o processo sigiloso. A expressão “representantes” contempla tanto os advogados quanto os defensores e/ou procuradores.

**Resumo Nível 1:**

* Juiz eleitoral;
* Servidor e servidor de processamento;
* Polo ativo e seus representantes (advogados, defensores, procuradores);
* Membros do Ministério Público, como fiscal da lei.

**Nível 3 (Sigilo Médio)**

Visualização restrita aos serventuários da Zona Eleitoral que possuem perfil de “servidor”, ao juiz eleitoral, ao polo ativo e seus representantes. Mais uma vez, a expressão “representantes” contempla tanto os advogados quanto os defensores e/ou procuradores.

**Resumo Nível 3:**

* Juiz eleitoral;
* Servidor;
* Polo ativo e seus representantes (advogados, defensores, procuradores);

**Observação:** No nível 3, caso necessário, o magistrado poderá atribuir visualização no processo ao polo passivo e aos membros do Ministério Público.

**Nível 4 (Sigilo Intenso)**

Visualização restrita ao Magistrado, Secretário Judiciário, ao Secretário da Corregedoria, aos Assessores-Chefes dos Gabinetes e ao Assessor-Chefe de Plenário.

**Resumo Nível 4:**

* Magistrado;
* Secretário Judiciário;
* Secretário da Corregedoria
* Assessores-Chefes dos Gabinetes
* Assessor-Chefe de Plenário

**Nível 5 (Sigilo Absoluto)**

Visualização restrita ao magistrado, polo ativo e seus representantes.

**Resumo Nível 5:**

* Juiz eleitoral;
* Polo ativo e seus representantes (advogados, defensores, procuradores);

**Observação:** No nível 5, caso necessário, o magistrado poderá atribuir visualização no processo a servidores, ao polo passivo e aos membros do Ministério Público.

#### Recomendações

Para fins de testes de interoperabilidade, recomendamos o uso da ferramenta SoapUI para a realização de requisições XML. A ferramenta é gratuita.

## Anexos

#### <li>Exemplos de Requisições XML - Intercomunicação</li>

| Destinatário | Link |
| :---: | :---: |
| TODOS | [Exemplos de Requisições XML - Intercomunicação](\anexos\Intercomunicacao - Exemplos.zip) |

#### <li>Exemplos de Requisições XML - ConsultaPJe</li>

| Destinatário | Link |
| :---: | :---: |
| TODOS | [Exemplos de Requisições XML - ConsultaPJe](\anexos\ConsultaPJe - Exemplos.zip) |

#### <li>Exemplo de Requisição XML - Documento Assinado Para Entrega Avulsa</li>

| Destinatário | Link |
| :---: | :---: |
| TODOS | [Exemplo de Requisição XML - Documentos Assinados](\anexos\entregarManifestaçãoProcessual – DocumentoAssinado.xml) |

#### <li>Guia Enviar Expediente Para MPE.pdf</li>

| Destinatário | Link |
| :---: | :---: |
| TODOS | [Guia Enviar Expediente Para MPE.pdf](\anexos\Guia Enviar Expediente Para MPE.pdf) |

#### <li>Endereços dos Ambientes do PJe 1g, 2g e 3g – Produção</li>
**1º grau (Zonas Eleitorais)**

| 1º grau | Endereço |
| :---: | :---: |
| ZE | [https://pje1g.tse.jus.br/pje/login.seam](https://pje1g.tse.jus.br/pje/login.seam) |

**2º grau (Tribunais Regionais Eleitorais)**

| 2º grau | Endereço |
| :---: | :---: |
|TRE-AC | [https://pje.tre-ac.jus.br/pje/login.seam](https://pje.tre-ac.jus.br/pje/login.seam) | 
|TRE-AL | [https://pje.tre-al.jus.br/pje/login.seam](https://pje.tre-al.jus.br/pje/login.seam) |
|TRE-AM | [https://pje.tre-am.jus.br/pje/login.seam](https://pje.tre-am.jus.br/pje/login.seam) |
|TRE-AP | [https://pje.tre-ap.jus.br/pje/login.seam](https://pje.tre-ap.jus.br/pje/login.seam) |
|TRE-BA | [https://pje.tre-ba.jus.br/pje/login.seam](https://pje.tre-ba.jus.br/pje/login.seam) |
|TRE-CE | [https://pje.tre-ce.jus.br/pje/login.seam](https://pje.tre-ce.jus.br/pje/login.seam) |
|TRE-DF | [https://pje.tre-df.jus.br/pje/login.seam](https://pje.tre-df.jus.br/pje/login.seam) |
|TRE-ES | [https://pje.tre-es.jus.br/pje/login.seam](https://pje.tre-es.jus.br/pje/login.seam) |
|TRE-GO | [https://pje.tre-go.jus.br/pje/login.seam](https://pje.tre-go.jus.br/pje/login.seam) |
|TRE-MA | [https://pje.tre-ma.jus.br/pje/login.seam](https://pje.tre-ma.jus.br/pje/login.seam) |
|TRE-MG | [https://pje.tre-mg.jus.br/pje/login.seam](https://pje.tre-mg.jus.br/pje/login.seam) |
|TRE-MS | [https://pje.tre-ms.jus.br/pje/login.seam](https://pje.tre-ms.jus.br/pje/login.seam) |
|TRE-MT | [https://pje.tre-mt.jus.br/pje/login.seam](https://pje.tre-mt.jus.br/pje/login.seam) |
|TRE-PA | [https://pje.tre-pa.jus.br/pje/login.seam](https://pje.tre-pa.jus.br/pje/login.seam) |
|TRE-PB | [https://pje.tre-pb.jus.br/pje/login.seam](https://pje.tre-pb.jus.br/pje/login.seam) |
|TRE-PE | [https://pje.tre-pe.jus.br/pje/login.seam](https://pje.tre-pe.jus.br/pje/login.seam) |
|TRE-PI | [https://pje.tre-pi.jus.br/pje/login.seam](https://pje.tre-pi.jus.br/pje/login.seam) |
|TRE-PR | [https://pje.tre-pr.jus.br/pje/login.seam](https://pje.tre-pr.jus.br/pje/login.seam) |
|TRE-RJ | [https://pje.tre-rj.jus.br/pje/login.seam](https://pje.tre-rj.jus.br/pje/login.seam) |
|TRE-RN | [https://pje.tre-rn.jus.br/pje/login.seam](https://pje.tre-rn.jus.br/pje/login.seam) |
|TRE-RO | [https://pje.tre-ro.jus.br/pje/login.seam](https://pje.tre-ro.jus.br/pje/login.seam) |
|TRE-RR | [https://pje.tre-rr.jus.br/pje/login.seam](https://pje.tre-rr.jus.br/pje/login.seam) |
|TRE-RS | [https://pje.tre-rs.jus.br/pje/login.seam](https://pje.tre-rs.jus.br/pje/login.seam) |
|TRE-SC | [https://pje.tre-sc.jus.br/pje/login.seam](https://pje.tre-sc.jus.br/pje/login.seam) |
|TRE-SE | [https://pje.tre-se.jus.br/pje/login.seam](https://pje.tre-se.jus.br/pje/login.seam) |
|TRE-SP | [https://pje.tre-sp.jus.br/pje/login.seam](https://pje.tre-sp.jus.br/pje/login.seam) |
|TRE-TO | [https://pje.tre-to.jus.br/pje/login.seam](https://pje.tre-to.jus.br/pje/login.seam) |

**3º grau (TSE)**

| 3º grau | Endereço |
| :---: | :---: |
| TSE | [https://pje.tse.jus.br/pje/login.seam](https://pje.tse.jus.br/pje/login.seam) |

#### <li>Endereços dos Webservices Intercomunicação – Produção</li>

**1º grau (Zonas Eleitorais)**

| 1º grau | Endereço |
| :---: | :---: |
| ZE | [https://pje1g.tse.jus.br/pje/intercomunicacao?wsdl](https://pje1g.tse.jus.br/pje/intercomunicacao?wsdl) |

**2º grau (Tribunais Regionais Eleitorais)**

| 2º grau | Endereço |
| :---: | :---: |
|TRE-AC | [https://pje.tre-ac.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-ac.jus.br/pje/intercomunicacao?wsdl) |
|TRE-AL | [https://pje.tre-al.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-al.jus.br/pje/intercomunicacao?wsdl) |
|TRE-AM | [https://pje.tre-am.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-am.jus.br/pje/intercomunicacao?wsdl) |
|TRE-AP | [https://pje.tre-ap.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-ap.jus.br/pje/intercomunicacao?wsdl) |
|TRE-BA | [https://pje.tre-ba.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-ba.jus.br/pje/intercomunicacao?wsdl) |
|TRE-CE | [https://pje.tre-ce.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-ce.jus.br/pje/intercomunicacao?wsdl) |
|TRE-DF | [https://pje.tre-df.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-df.jus.br/pje/intercomunicacao?wsdl) |
|TRE-ES | [https://pje.tre-es.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-es.jus.br/pje/intercomunicacao?wsdl) |
|TRE-GO | [https://pje.tre-go.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-go.jus.br/pje/intercomunicacao?wsdl) |
|TRE-MA | [https://pje.tre-ma.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-ma.jus.br/pje/intercomunicacao?wsdl) |
|TRE-MG | [https://pje.tre-mg.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-mg.jus.br/pje/intercomunicacao?wsdl) |
|TRE-MS | [https://pje.tre-ms.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-ms.jus.br/pje/intercomunicacao?wsdl) |
|TRE-MT | [https://pje.tre-mt.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-mt.jus.br/pje/intercomunicacao?wsdl) |
|TRE-PA | [https://pje.tre-pa.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-pa.jus.br/pje/intercomunicacao?wsdl) |
|TRE-PB | [https://pje.tre-pb.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-pb.jus.br/pje/intercomunicacao?wsdl) |
|TRE-PE | [https://pje.tre-pe.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-pe.jus.br/pje/intercomunicacao?wsdl) |
|TRE-PI | [https://pje.tre-pi.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-pi.jus.br/pje/intercomunicacao?wsdl) |
|TRE-PR | [https://pje.tre-pr.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-pr.jus.br/pje/intercomunicacao?wsdl) |
|TRE-RJ | [https://pje.tre-rj.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-rj.jus.br/pje/intercomunicacao?wsdl) |
|TRE-RN | [https://pje.tre-rn.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-rn.jus.br/pje/intercomunicacao?wsdl) |
|TRE-RO | [https://pje.tre-ro.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-ro.jus.br/pje/intercomunicacao?wsdl) |
|TRE-RR | [https://pje.tre-rr.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-rr.jus.br/pje/intercomunicacao?wsdl) |
|TRE-RS | [https://pje.tre-rs.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-rs.jus.br/pje/intercomunicacao?wsdl) |
|TRE-SC | [https://pje.tre-sc.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-sc.jus.br/pje/intercomunicacao?wsdl) |
|TRE-SE | [https://pje.tre-se.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-se.jus.br/pje/intercomunicacao?wsdl) |
|TRE-SP | [https://pje.tre-sp.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-sp.jus.br/pje/intercomunicacao?wsdl) |
|TRE-TO | [https://pje.tre-to.jus.br/pje/intercomunicacao?wsdl](https://pje.tre-to.jus.br/pje/intercomunicacao?wsdl) |

**3º grau (TSE)**

| 3º grau | Endereço |
| :---: | :---: |
| TSE | [https://pje.tse.jus.br/pje/intercomunicacao?wsdl](https://pje.tse.jus.br/pje/intercomunicacao?wsdl) |

#### <li>Endereços dos Webservices ConsultaPJe – Produção</li>

**1º grau (Zonas Eleitorais)**

| 1º grau | Endereço |
| :---: | :---: |
| ZE | [https://pje1g.tse.jus.br/pje/ConsultaPJe?wsdl](https://pje1g.tse.jus.br/pje/ConsultaPJe?wsdl) |

**2º grau (Tribunais Regionais Eleitorais)**

| 2º grau | Endereço |
| :---: | :---: |
|TRE-AC | [https://pje.tre-ac.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-ac.jus.br/pje/ConsultaPJe?wsdl) | 
|TRE-AL | [https://pje.tre-al.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-al.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-AM | [https://pje.tre-am.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-am.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-AP | [https://pje.tre-ap.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-ap.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-BA | [https://pje.tre-ba.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-ba.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-CE | [https://pje.tre-ce.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-ce.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-DF | [https://pje.tre-df.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-df.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-ES | [https://pje.tre-es.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-es.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-GO | [https://pje.tre-go.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-go.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-MA | [https://pje.tre-ma.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-ma.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-MG | [https://pje.tre-mg.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-mg.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-MS | [https://pje.tre-ms.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-ms.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-MT | [https://pje.tre-mt.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-mt.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-PA | [https://pje.tre-pa.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-pa.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-PB | [https://pje.tre-pb.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-pb.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-PE | [https://pje.tre-pe.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-pe.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-PI | [https://pje.tre-pi.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-pi.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-PR | [https://pje.tre-pr.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-pr.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-RJ | [https://pje.tre-rj.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-rj.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-RN | [https://pje.tre-rn.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-rn.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-RO | [https://pje.tre-ro.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-ro.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-RR | [https://pje.tre-rr.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-rr.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-RS | [https://pje.tre-rs.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-rs.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-SC | [https://pje.tre-sc.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-sc.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-SE | [https://pje.tre-se.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-se.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-SP | [https://pje.tre-sp.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-sp.jus.br/pje/ConsultaPJe?wsdl) |
|TRE-TO | [https://pje.tre-to.jus.br/pje/ConsultaPJe?wsdl](https://pje.tre-to.jus.br/pje/ConsultaPJe?wsdl) |

**3º grau (TSE)**

| 3º grau | Endereço |
| :---: | :---: |
| TSE | [https://pje.tse.jus.br/pje/ConsultaPJe?wsdl](https://pje.tse.jus.br/pje/ConsultaPJe?wsdl) |

#### <li>Endereços do Ambiente e Webservices PJe 1g – EAD</li>

**Endereço do Ambiente**

| 1º grau | Endereço |
| :---: | :---: |
| ZE | [https://pje1g-ead.tse.jus.br/pje/login.seam](https://pje1g-ead.tse.jus.br/pje/login.seam) |

**Endereço do Webservice Intercomunicação**

| 1º grau | Endereço |
| :---: | :---: |
| ZE | [https://pje1g-ead.tse.jus.br/pje/intercomunicacao?wsdl](https://pje1g-ead.tse.jus.br/pje/intercomunicacao?wsdl) |

**Endereço do Webservice ConsultaPJe**

| 1º grau | Endereço |
| :---: | :---: |
| ZE | [https://pje1g-ead.tse.jus.br/pje/ConsultaPJe?wsdl](https://pje1g-ead.tse.jus.br/pje/ConsultaPJe?wsdl) |

#### <li>Endereços do Ambiente e Webservices PJe 2g – EAD</li>

**Endereço do Ambiente**

| 2º grau | Endereço |
| :---: | :---: |
| TRE | [https://pje2g-ead.tse.jus.br/pje/login.seam](https://pje2g-ead.tse.jus.br/pje/login.seam) |

**Endereço do Webservice Intercomunicação**

| 2º grau | Endereço |
| :---: | :---: |
| TRE | [https://pje2g-ead.tse.jus.br/pje/intercomunicacao?wsdl](https://pje2g-ead.tse.jus.br/pje/intercomunicacao?wsdl) |

**Endereço do Webservice ConsultaPJe**

| 2º grau | Endereço |
| :---: | :---: |
| TRE | [https://pje2g-ead.tse.jus.br/pje/ConsultaPJe?wsdl](https://pje2g-ead.tse.jus.br/pje/ConsultaPJe?wsdl) |

#### <li>Endereços do Ambiente e Webservices PJe 3g – EAD</li>

**Endereço do Ambiente**

| 3º grau | Endereço |
| :---: | :---: |
| TSE | [https://pje3g-ead.tse.jus.br/pje/login.seam](https://pje3g-ead.tse.jus.br/pje/login.seam) |

**Endereço do Webservice Intercomunicação**

| 3º grau | Endereço |
| :---: | :---: |
| TSE | [https://pje3g-ead.tse.jus.br/pje/intercomunicacao?wsdl](https://pje3g-ead.tse.jus.br/pje/intercomunicacao?wsdl) |

**Endereço do Webservice ConsultaPJe**

| 3º grau | Endereço |
| :---: | :---: |
| TSE | [https://pje3g-ead.tse.jus.br/pje/ConsultaPJe?wsdl](https://pje3g-ead.tse.jus.br/pje/ConsultaPJe?wsdl) |

