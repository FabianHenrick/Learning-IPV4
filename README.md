# Learning-IPV4
<h1>Aqui Começãm meus estudos de Endereçamento IPV4</h1>

IP, ou Protocolo de Internet (Internet Protocol), é um conjunto de regras que governam o formato dos dados enviados via internet ou rede local. Ele é responsável por endereçar, encaminhar e rotear pacotes de dados,
permitindo que computadores e dispositivos se comuniquem entre si.

Há dois tipos principais de endereços IP:
<li>
 IPv4 (Internet Protocol version 4): Utiliza endereços de 32 bits, geralmente representados por quatro números decimais separados por pontos (por exemplo, 192.168.0.1). Com o crescimento da internet, o número de endereços IPv4 disponíveis está se esgotando.

<li> IPv6 (Internet Protocol version 6): Utiliza endereços de 128 bits, representados por oito grupos de quatro dígitos hexadecimais separados por dois pontos (por exemplo, 2001:0db8:85a3:0000:0000:8a2e:0370:7334).
O IPv6 foi desenvolvido para resolver a limitação de endereços do IPv4 e para melhorar certos aspectos do protocolo.


Os endereços IP são fundamentais para a comunicação na internet, permitindo que dados sejam enviados e recebidos corretamente entre dispositivos.

Os endereços IPv4 são divididos em diferentes classes para facilitar a atribuição e roteamento de endereços IP. Essas classes são definidas pela IANA (Internet Assigned Numbers Authority) e são baseadas nos primeiros bits do endereço IP. Existem cinco classes principais: A, B, C, D e E. Aqui está uma descrição de cada uma:

<h3>Classe A:</h3>

Intervalo: 0.0.0.0 a 127.255.255.255
Primeiro Octeto: 0 a 127
Número de Redes: 128
Número de Hosts por Rede: 16.777.216 - 2 (dois endereços são reservados)
Uso: Grandes redes com muitos hosts (empresas muito grandes, redes governamentais)

<h3>Classe B:</h3>

Intervalo: 128.0.0.0 a 191.255.255.255
Primeiro Octeto: 128 a 191
Número de Redes: 16.384
Número de Hosts por Rede: 65.536 - 2
Uso: Redes de tamanho médio (universidades, grandes empresas)

<h3>Classe C:</h3>

Intervalo: 192.0.0.0 a 223.255.255.255
Primeiro Octeto: 192 a 223
Número de Redes: 2.097.152
Número de Hosts por Rede: 256 - 2
Uso: Pequenas redes (pequenas empresas, redes residenciais)

Classe D:

Intervalo: 224.0.0.0 a 239.255.255.255
Primeiro Octeto: 224 a 239
Uso: Multicast (envio de dados para múltiplos destinos simultaneamente)

<h3>Classe E:</h3>

Intervalo: 240.0.0.0 a 255.255.255.255
Primeiro Octeto: 240 a 255
Uso: Reservada para uso futuro e para testes
Os endereços de classes A, B e C são utilizados para a alocação de redes e hosts na internet. As classes D e E têm propósitos específicos e não são usadas para endereçamento regular de hosts.

métodos de comunicação usados na rede para enviar dados de um ou mais remetentes para um ou mais receptores. Cada método tem características específicas:

Unicast:

Definição: Comunicação de um para um.
Descrição: Dados são enviados de um único remetente para um único receptor específico. Este é o método mais comum de transmissão na rede.
Exemplo: Um computador enviando um e-mail para outro computador.
Broadcast:

Definição: Comunicação de um para todos.
Descrição: Dados são enviados de um único remetente para todos os dispositivos na rede. Usado principalmente em redes locais (LANs).
Exemplo: Um roteador enviando uma mensagem ARP (Address Resolution Protocol) para todos os dispositivos em uma rede local.
Multicast:

Definição: Comunicação de um para muitos.
Descrição: Dados são enviados de um único remetente para um grupo específico de receptores que se inscreveram para receber os dados. Mais eficiente do que o broadcast quando se trata de enviar dados para múltiplos receptores.
Exemplo: Transmissão de vídeo em streaming para um grupo de assinantes.
Anycast:

Definição: Comunicação de um para qualquer um.
Descrição: Dados são enviados de um único remetente para o receptor mais próximo ou melhor em um grupo de possíveis receptores. Este método é usado para otimizar a entrega de dados e melhorar a redundância.
Exemplo: Consultas DNS (Domain Name System), onde a solicitação é enviada para o servidor DNS mais próximo disponível.
Comparação Visual

Unicast:
lua
Remetente -----> Receptor

Broadcast:
lua
Remetente -----> Todos os dispositivos na rede

Multicast:
lua
Remetente -----> Grupo de dispositivos específicos

Anycast:
bash
Remetente -----> Receptor mais próximo em um grupo de dispositivos
Cada método tem seus próprios casos de uso e é escolhido com base nas necessidades da aplicação e na eficiência desejada da comunicação na rede.
