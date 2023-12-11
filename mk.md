<table>
  <tr>
    <td rowspan="4"><img src="./assets/ifma.jpg" alt="IFMA Logo" style="width:300px;"></td>
    <td>Instituto Federal de Educação, Ciência e Tecnologia do Maranhão</td>
  </tr>
  <tr>
    <td>Disciplina: Redes de Computadores I</td>
  </tr>
  <tr>
    <td>Professor: <a href="https://github.com/agenteph">Paulo Henrique Barbosa</a></td>
  </tr>
  <tr>
    <td>Aluno: Israel Jorge de Sousa</td>
  </tr>
</table>

# Introdução

Esta Wiki apresenta o projeto de simulação de rede desenvolvido para disciplina de Redes de Computadores I. O principal objetivo deste projeto é proporcionar uma experiência prática abrangente na configuração e administração de uma rede de computadores. O ambiente de simulação será construído utilizando a ferramenta Cisco Packet Tracer, que oferece a oportunidade de aplicar de maneira concreta os conhecimentos adquiridos ao longo da disciplina de Redes de Computadores I.

### Cenário proposto - 1 parte

Na Empresa EHNOS, o proprietário expressou o desejo de conectar todos os computadores da empresa em uma rede com acesso à internet. Para solucionar esse desafio, você foi contratado como responsável pela tecnologia para organizar e montar toda a rede.

O proprietário informou que são 25 computadores e solicitou a você a lista de requisitos para montar a rede, o layout completo da estrutura e uma rede eficiente para a transferência de grandes volumes de arquivos.

#### Notas Importantes:

- **A rede deverá ter endereços LAN das três classes:**

  - Rede 1 (Classe A) - 10 computadores.
  - Rede 2 (Classe B) - 10 computadores.
  - Rede 3 (Classe C) - 5 computadores.

- **Interligar cada rede com 2 HUB's e 3 Switch's;**

  - 2 HUBs e 3 Switch's para interligar as redes.

- **Realizar os testes de Ping entre todos os computadores.**

## Equipamentos utilizados

- 25 computadores com o sistema operacional Windows com portas de rede Gigabit Ethernet.
- 2 Hubs com 4 com portas de rede Gigabit Ethernet.
- 3 Switch's Multi-Layer com portas de rede Gigabit Ethernet.
- 1 Roteador com 3 placas de rede Gigabit Ethernet.

<img src="./assets/equipamentos-1.png" alt="Equipamentos" >

Todos os equipamentos foram modificados para possuírem portas de rede Gigabit Ethernet pois o cliente quer uma rede eficiente para a transferência de grandes volumes de arquivos.

## Organização dos Dispositivos

A estrutura da rede foi projetada seguindo o modelo de topologia estrela, no qual os Switch's desempenharam o papel centralizador para cada grupo de classe. Os dispositivos foram organizados e conectados diretamente por meio de cabos.

<img src="./assets/organizacao-rede-1.png" alt="Organização" >

#### Configuração da Rede 1

Os computadores da Rede 1 foram configurados para rede 10.100.101.0/24 com Ip's de Classe A de 10.100.101.2 a 10.100.101.11

<div style="display: flex; justify-items: center; align-items: center; flex-direction: column;" >
  <img src="./assets/rede-1.png" width="500" style="display: block;  margin: 0 auto;" alt="Organização" >
  <img src="./assets/cf-A.png" width="600" style="display: block;  margin: 0 auto;" alt="Organização" >
</div>

#### Configuração da Rede 2

Os computadores da Rede 2 foram configurados para rede 172.16.0.0/24 com Ip's de Classe A de 172.16.0.2 a 172.16.0.11

<div style="display: flex; justify-items: center; align-items: center; flex-direction: column;" >
  <img src="./assets/rede-2.png" width="500" style="display: block;  margin: 0 auto;" alt="Organização" >
  <img src="./assets/cf-b.png" width="600" style="display: block;  margin: 0 auto;" alt="Organização" >
</div>

#### Configuração da Rede 3

Os computadores da Rede 3 foram configurados para rede 192.168.2.0/24 com Ip's de Classe A de 192.168.2.2 a 192.168.2.6

<div style="display: flex; justify-items: center; align-items: center; flex-direction: column;" >
  <img src="./assets/rede-3.png" width="500" style="display: block;  margin: 0 auto;" alt="Organização" >
  <img src="./assets/cf-c.png" width="600" style="display: block;  margin: 0 auto;" alt="Organização" >
</div>

#### Conectando as três Redes

Para interligar as três redes foi empregado um roteador para interligar as três redes, desempenhando o papel de gateway. Cada rede estabelece conexão com o roteador através de uma porta, conforme a seguinte configuração:

<div style="display: flex; justify-items: center; flex-direction: column;" >
 <ul>
 <li style="margin-bottom:30px;">
  Rede 1 (Classe A)
   <img src="./assets/r1.png" width="600" style="display: block;" alt="Organização" >
 </li>

 <li style="margin-bottom:30px;">
  Rede 2 (Classe B)
    <img src="./assets/r2.png" width="600" style="display: block;" alt="Organização" >
 </li>

 <li>
  Rede 3 (Classe C)
    <img src="./assets/r3.png" width="600" style="display: block;" alt="Organização" >
 </li>
 
 </ul>
</div>

## Testes de Ping

Nesta etapa vamos utilizar a ferramenta que é usada para testar a conectividade entre dois dispositivos em uma rede, como computadores ou servidores.

### Entre os Computadores na Rede 1 (Classe A):

- **Na mesma Rede**
<div>
  <img src="./assets/t-A-1.png" width="500" height="700"  alt="Organização" >
  <img src="./assets/t-A-2.png" width="500" height="700" alt="Organização" >
   <img src="./assets/t-A-3.png"width="500" height="200"  alt="Organização" >
</div>

- **Com a Rede de Classe B**
<div>
  <img src="./assets/t-A-4.png" width="500" height="700"  alt="Organização" >
</div>

- **Com a Rede de Classe C**
<div>
  <img src="./assets/t-A-5.png" width="500" height="700"  alt="Organização" >
</div>

#### Entre os Computadores na Rede 2 (Classe B):

- **Na mesma Rede**
<div>
  <img src="./assets/t-B-1.png" width="500" height="700"  alt="Organização" >
  <img src="./assets/t-B-2.png" width="500" height="700" alt="Organização" >
   <img src="./assets/t-B-3.png"width="500" height="200"  alt="Organização" >
</div>

- **Com a Rede de Classe A**
<div>
  <img src="./assets/t-B-4.png" width="500" height="700"  alt="Organização" >
</div>

- **Com a Rede de Classe C**
<div>
  <img src="./assets/t-B-5.png" width="500" height="700"  alt="Organização" >
</div>

#### Entre os Computadores na Rede 3 (Classe C):

- **Na mesma Rede**
<div>
  <img src="./assets/t-C-1.png" width="500" height="700"  alt="Organização" >
</div>

- **Com a Rede de Classe A**
<div>
  <img src="./assets/t-C-4.png" width="500" height="700"  alt="Organização" >
</div>

- **Com a Rede de Classe B**
<div>
  <img src="./assets/t-C-5.png" width="500" height="700"  alt="Organização" >
</div>

Após a realização abrangente dos testes utilizando o comando "ping" entre os computadores nas redes designadas, os resultados fornecem uma visão esclarecedora do estado de conectividade. Notavelmente, constatamos que todos os testes efetuados dentro de uma mesma rede (Classe A, Classe B e Classe C) apresentaram sucesso, com 100% dos pacotes sendo recebidos.

No entanto, ao realizar os testes entre computadores de redes distintas, observamos uma consistente perda de 1 pacote. Este padrão sugere que pode haver um desafio específico na comunicação inter-redes, possivelmente atribuível a configurações de roteamento ou outros fatores de infraestrutura.

## Testes de no modo simulação do Packet Tracer

<img src="./assets/s-1_1.gif" style="margin-bottom:30px;"   alt="Organização" >
<br />
<img src="./assets/s-1_2.gif"   alt="Organização" >

## Conclusão do Cenário Proposto:

Após a configuração e implementação da rede para a Empresa EHNOS, os testes de ping realizados ofereceram insights cruciais sobre a conectividade e desempenho. No âmbito das redes internas (Classe A, B e C), os resultados demonstraram uma comunicação robusta, evidenciada pelo recebimento de 100% dos pacotes, indicando uma sólida configuração intra-rede.

No entanto, ao realizar os testes entre computadores de redes distintas, foi observada uma perda consistente de 1 pacote. Esse comportamento aponta para possíveis desafios na interconexão das redes, como configurações de roteamento ou políticas de segurança entre as classes de redes.
