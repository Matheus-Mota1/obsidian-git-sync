# Definição

International Organization for Standardization (ISO), um órgão que desenvolve padrões internacionais, criou um modelo de referência de camadas 


| Camada | PDU |
| ---------| ------|
|7. Aplicação| Dados |
|6. presentação | Dados |
|5. Sessão | Dados |
|4. Transporte | Segmento |
|3. Rede | Pacote |
|2. Link de Dados | Quadro |
|1. Física | Bits |

Da camada 7 a camada 3 são praticamente implementadas em software, por meio de protocolos no sistema operacional ou de aplicações de redes desenvolvidas pelos programadores.

A camada 1 e 2 podem ser associadas à placa de rede. A camada 2 ainda integra um pouco de software, como os drivers da placa de rede, mas a camada 1 é praticamente toda implementada em hardware.

# Possibilita acesso aos recursos de rede

[[Camada de Aplicação]]

# Traduzir, criptografar e comprimir dados

[[Camada de Apresentação]]

# Estabelecer, gerenciar e encerrar sessões.

[[Camada de Sessão]]

# Promover a entrega confiável das mensagens processo a processo e recuperação de erros

[[Camada de Transporte]]

# Transferir pacotes de origem no destino; fornecer ligação entre redes.

[[Camada de Rede]]

# Organizar bits e quadros fornecer entrega nó a nó.

[[Camada de Enlace]]

# Transmitir bits através de um meio físico, prover especificações mecânicas e elétricas.

[[Camada Física]]





por:

  
* Bibiliografia *  
  
• RFC 1123 - [https://tools.ietf.org/html/rfc1123](https://tools.ietf.org/html/rfc1123)  
• Stevens,R. TCP/IP illustrated, Volume 1. Ed. Addison Wesley, 2000.  
• Siyan, K. S.; Parker, T. TCP/IP Unleashed. Ed. SAMS Publishing, 2002.  
• Forouzan, B.A. TCP/IP Protocol Suite, 4° edição Ed.McGraw-Hill, 2020  
• Murhammer; Atakan; Bretz; Pugh; Suzuki; Wood. TCP/IP Tutorial e Técnico - IBM Books. Makron Books

Comunicação e encapsulamente

Comunicação horizontal
Uma camada só consegue conversar com ela mesma, ou seja a camada 2 do destinatário só consegue se comunicar com a camada 2 do destinatário esse comunicação ocorre de forma virtual. Essas informações denominadas **cabeçalhos**.

Cada camada adicionara um novo cabeçalho ao dado que será enviado, e esse processo e chamado de **encapsulamento**

Esse procedimento acontece, repetidamente, até alcançar a camada 1 e a informação ser transmitida ao destino, onde ocorrerá o processo inverso. A informação subira, desencapsulando as informações, da camada 1 até o usuário do serviço.
Ao encapsular é criado o PDU

# Protocolo
É a definição deste procedimento. É o conjunto de normas para a comunicação entre dois equipamentos. Neste exemplo, você utilizou a escrita no idioma português para enviar um recado para outra pessoa que também sabe ler em português, ou seja, vocês falam o mesmo protocolo.
O protocolo é a implementação do serviço que a camada deve executar.
# Interface
