# O que é DNS?
*DNS significa "Domain Name Server" ou "Sistema de Nomes de Domínio", em português. É uma parte fundamental da infraestrutura da Internet e atua como um sistema de tradução de nomes de domínio em endereços IP (Internet Protocol).*

## Por que o uso de domínio?
*Os nomes de domínio, como "google.com", "facebook.com" e "wikipedia.org", são mais fáceis de serem lembrados e compreendidos pelas pessoas do que os endereços IP, que são uma série de números, como "172.217.21.174" (endereço IP do Google). O DNS é responsável por fazer o mapeamento entre esses nomes de domínio legíveis por humanos e os endereços IP associados a eles, assim como uma lista telefônica, traduzindo nomes para números.*
## Como o DNS funciona na prática?
*Quando você digita um nome de domínio em seu navegador para acessar um site, o computador precisa descobrir o endereço IP correspondente para se conectar ao servidor que hospeda o site. O processo funciona da seguinte maneira:*

- **1 - O navegador envia uma solicitação para o servidor DNS do seu provedor de internet ou para um servidor DNS configurado em sua rede local.**

- **2 - O servidor DNS verifica se tem o endereço IP correspondente ao nome de domínio na sua cache (memória temporária). Se estiver lá, ele retorna o endereço IP ao navegador, e o navegador pode se conectar diretamente ao servidor do site.**

- **3 - Se o servidor DNS não tiver a informação em sua cache, ele encaminha a solicitação para outros servidores DNS mais autoritativos, que possuem informações atualizadas sobre os domínios e seus endereços IP.**

- **4 - A solicitação é encaminhada de servidor para servidor até que o servidor DNS responsável pelo domínio específico seja encontrado.**

- **5 - O servidor DNS autoritativo retorna o endereço IP ao servidor que fez a solicitação, e então esse endereço IP é passado de volta ao navegador.**

- **6 - O navegador pode, finalmente, se conectar ao servidor do site usando o endereço IP fornecido pelo servidor DNS.**

*Todo esse processo acontece em questão de milissegundos, permitindo que os usuários acessem sites rapidamente por meio de nomes de domínio familiares, sem a necessidade de memorizar os complexos endereços IP. O DNS é uma peça essencial da arquitetura da Internet e facilita muito a navegação e a comunicação na web.*