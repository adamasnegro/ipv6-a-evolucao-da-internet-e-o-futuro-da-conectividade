# 🌐 IPv6 — A Evolução da Internet e o Futuro da Conectividade

> **Da limitação do IPv4 à nova geração do protocolo de Internet**

A Internet cresceu de maneira extraordinária desde sua criação. Milhões de computadores inicialmente conectados por redes acadêmicas e militares deram lugar a bilhões de dispositivos, smartphones, servidores, sensores, sistemas corporativos, serviços em nuvem, dispositivos IoT e infraestruturas críticas.

Por trás de toda essa comunicação existe um elemento fundamental:

**o endereço IP.**

Durante décadas, o **IPv4 — Internet Protocol version 4** foi responsável por identificar e permitir a comunicação entre dispositivos na Internet.

Porém, o crescimento da Internet revelou uma limitação estrutural:

> **O espaço de endereçamento do IPv4 não foi projetado para a escala da Internet moderna.**

Foi nesse contexto que surgiu o **IPv6 — Internet Protocol version 6**, projetado como sucessor do IPv4 e preparado para uma Internet com uma quantidade muito maior de dispositivos conectados.

---

# 📚 1. O que é um endereço IP?

Um endereço IP é um identificador utilizado na camada de rede para permitir que dispositivos sejam localizados e que pacotes sejam encaminhados entre redes.

De forma simplificada:

```text
Dispositivo
     ↓
Endereço IP
     ↓
Rede
     ↓
Roteadores
     ↓
Destino
```

Quando acessamos um site, utilizamos um aplicativo, fazemos uma chamada de vídeo ou acessamos um servidor remoto, pacotes precisam ser encaminhados através de diversas redes.

O protocolo IP fornece uma parte fundamental dessa comunicação.

---

# 🕰️ 2. O nascimento do IPv4

O IPv4 foi especificado originalmente na **RFC 791**, publicada em 1981.

Naquele período, a Internet possuía uma dimensão completamente diferente da atual.

Computadores eram muito menos numerosos, dispositivos móveis praticamente não existiam e conceitos como:

* smartphones;
* Internet das Coisas;
* computação em nuvem;
* streaming em larga escala;
* redes 5G;
* cidades inteligentes;
* bilhões de sensores;

ainda não faziam parte da realidade cotidiana.

O IPv4 utiliza endereços de:

```text
32 bits
```

Isso permite aproximadamente:

```text
2³²

≈ 4,3 bilhões de endereços
```

Um endereço IPv4 possui o formato:

```text
192.168.1.10
```

Dividido em quatro octetos.

---

# ⚠️ 3. O problema do IPv4

À primeira vista, mais de 4 bilhões de endereços parece uma quantidade enorme.

Porém, o crescimento da Internet mostrou que esse espaço não seria suficiente.

O problema não foi apenas a quantidade de pessoas.

Foi a explosão na quantidade de dispositivos.

Hoje podemos ter:

* computadores;
* notebooks;
* smartphones;
* tablets;
* servidores;
* impressoras;
* câmeras;
* roteadores;
* televisores;
* veículos;
* sensores;
* dispositivos industriais;
* equipamentos médicos;
* dispositivos IoT;
* máquinas virtuais;
* containers;
* serviços em nuvem.

Cada vez mais dispositivos precisam participar de redes IP.

---

# 🔥 4. O esgotamento dos endereços IPv4

O problema tornou-se tão significativo que organizações responsáveis pela administração dos recursos da Internet passaram a adotar políticas específicas para lidar com a escassez de endereços IPv4.

Uma das soluções mais conhecidas foi o:

## NAT — Network Address Translation

Com NAT, vários dispositivos de uma rede privada podem compartilhar um endereço IPv4 público.

Exemplo:

```text
                 INTERNET
                    │
              IPv4 Público
              200.10.20.30
                    │
                 ROTEADOR
                    │
          ┌─────────┼─────────┐
          │         │         │
       192.168.1.10  .20      .30
        PC          Notebook   IoT
```

O NAT ajudou a prolongar a vida do IPv4.

Porém, ele também introduziu complexidade.

---

# 🧩 5. Consequências da dependência do NAT

O NAT resolveu parte do problema de disponibilidade de endereços, mas criou uma arquitetura em que muitos dispositivos deixam de possuir conectividade global direta.

Isso pode complicar:

* aplicações ponto a ponto;
* VoIP;
* jogos online;
* servidores internos;
* algumas aplicações IoT;
* troubleshooting;
* protocolos que carregam endereços;
* criação de conexões de entrada;
* arquiteturas distribuídas.

O NAT não deve ser considerado simplesmente "ruim".

Ele é uma tecnologia extremamente importante no mundo IPv4.

Porém:

> **NAT é principalmente uma técnica de conservação de endereços, não uma substituição para um espaço de endereçamento globalmente escalável.**

---

# 🚀 6. Por que o IPv6 foi criado?

O IPv6 foi desenvolvido como sucessor do IPv4.

A proposta não era simplesmente criar "mais endereços".

O objetivo era desenvolver uma nova geração do protocolo IP capaz de oferecer:

* espaço de endereçamento muito maior;
* hierarquia de endereçamento mais escalável;
* autoconfiguração;
* multicast aprimorado;
* anycast;
* cabeçalho simplificado;
* suporte mais estruturado para extensões;
* arquitetura adequada ao crescimento da Internet.

A especificação atual do IPv6 está documentada na **RFC 8200**, publicada pela IETF em 2017.

---

# 🌎 7. IPv4 x IPv6

| Característica      | IPv4               | IPv6                         |
| ------------------- | ------------------ | ---------------------------- |
| Tamanho do endereço | 32 bits            | 128 bits                     |
| Endereços teóricos  | ≈ 4,3 bilhões      | ≈ 3,4 × 10³⁸                 |
| Notação             | Decimal            | Hexadecimal                  |
| Exemplo             | 192.168.1.10       | 2001:db8::10                 |
| Broadcast           | Sim                | Não                          |
| Multicast           | Sim                | Sim                          |
| Anycast             | Não originalmente  | Sim                          |
| Autoconfiguração    | Limitada           | Mais integrada               |
| NAT                 | Muito utilizado    | Não necessário para escassez |
| Fragmentação        | Roteadores e hosts | Origem                       |
| Cabeçalho           | Mais complexo      | Simplificado                 |
| Escalabilidade      | Limitada           | Extremamente maior           |

O IPv6 aumenta o tamanho do endereço de **32 para 128 bits**.

---

# 🔢 8. A diferença de escala

IPv4:

```text
2³²
≈ 4.294.967.296 endereços
```

IPv6:

```text
2¹²⁸
≈ 340 undecilhões
```

Ou aproximadamente:

```text
3,4 × 10³⁸
```

Essa diferença muda completamente a escala possível para o endereçamento da Internet.

O objetivo não é simplesmente entregar "um IP para cada pessoa".

É permitir uma arquitetura capaz de suportar uma quantidade gigantesca de redes, dispositivos, serviços e infraestruturas.

---

# 🧬 9. Como é um endereço IPv6?

IPv6 utiliza hexadecimal.

Exemplo:

```text
2001:0db8:85a3:0000:0000:8a2e:0370:7334
```

Pode ser abreviado utilizando regras específicas:

```text
2001:db8:85a3::8a2e:370:7334
```

Outro exemplo:

```text
2001:db8::1
```

A notação pode parecer complexa inicialmente.

Para quem trabalha com redes, porém, ela se torna natural com a prática.

---

# 🏗️ 10. Estrutura de endereçamento IPv6

O IPv6 permite uma estrutura hierárquica muito mais ampla.

Um endereço pode representar:

```text
Prefixo global
      ↓
     Rede
      ↓
   Sub-rede
      ↓
Interface
```

Isso permite que organizações criem hierarquias de endereçamento mais estruturadas.

Um exemplo conceitual:

```text
2001:db8:1234::/48
```

Dentro desse bloco podem existir diversas sub-redes:

```text
2001:db8:1234:0001::/64
2001:db8:1234:0002::/64
2001:db8:1234:0003::/64
2001:db8:1234:0004::/64
```

---

# ⚙️ 11. Autoconfiguração

Uma das características importantes do IPv6 é o suporte à autoconfiguração.

Um dispositivo pode obter informações de rede utilizando mecanismos como:

```text
SLAAC
```

### SLAAC

**Stateless Address Autoconfiguration**

Permite que hosts configurem automaticamente seus endereços IPv6 utilizando informações anunciadas pela rede.

Isso reduz a necessidade de configuração manual em determinados cenários.

Também é possível utilizar:

```text
DHCPv6
```

dependendo da arquitetura adotada.

---

# 🛣️ 12. IPv6 e roteamento

O crescimento da Internet exige não apenas muitos endereços, mas também uma arquitetura eficiente para organização das rotas.

O IPv6 foi projetado considerando:

* hierarquia;
* agregação de rotas;
* escalabilidade;
* crescimento de redes;
* múltiplos níveis de endereçamento.

Isso é fundamental para grandes provedores, data centers, redes corporativas e infraestrutura global.

---

# 🔄 13. A transição do IPv4 para o IPv6

A substituição do IPv4 não poderia acontecer de um dia para o outro.

A Internet é uma infraestrutura gigantesca e distribuída.

Existem:

* provedores;
* empresas;
* universidades;
* governos;
* data centers;
* dispositivos antigos;
* sistemas legados;
* aplicações;
* equipamentos de rede;
* serviços que ainda dependem de IPv4.

Por isso, a transição ocorre de maneira gradual.

---

# 🔀 14. Dual Stack

Uma das principais estratégias de transição é o:

## Dual Stack

O dispositivo utiliza simultaneamente:

```text
IPv4
+
IPv6
```

Exemplo:

```text
Servidor
 ├── IPv4: 203.0.113.10
 └── IPv6: 2001:db8::10
```

Isso permite que clientes IPv4 continuem funcionando enquanto clientes IPv6 também podem utilizar a infraestrutura.

---

# 🌉 15. Túneis IPv6

Outra estratégia consiste em transportar IPv6 através de uma infraestrutura IPv4.

Conceitualmente:

```text
IPv6
  ↓
Encapsulamento
  ↓
IPv4
  ↓
Rede IPv4
  ↓
Desencapsulamento
  ↓
IPv6
```

Tecnologias de tunelamento foram importantes durante diferentes fases da transição.

Entretanto, com o avanço da implantação nativa do IPv6, o objetivo é reduzir a dependência dessas técnicas.

---

# 🔁 16. Tradução entre IPv4 e IPv6

Também existem mecanismos de tradução.

Exemplos:

```text
NAT64
DNS64
```

Eles permitem que determinados clientes IPv6 alcancem serviços que ainda utilizam IPv4.

Isso é especialmente importante durante o período em que os dois protocolos coexistem.

---

# 🔐 17. IPv6 e segurança

Um erro comum é afirmar:

> "IPv6 é seguro por natureza."

Isso não é correto.

IPv6 não elimina:

* malware;
* phishing;
* DDoS;
* exploração de vulnerabilidades;
* ataques de aplicação;
* roubo de credenciais;
* ataques Man-in-the-Middle;
* interceptação de tráfego;
* configuração insegura.

A própria RFC 8200 destaca que IPv6 possui questões de segurança semelhantes às existentes no IPv4 e que mecanismos como TLS e SSH continuam importantes para proteger aplicações.

---

# 🛡️ 18. IPv6 não substitui uma arquitetura de segurança

Uma rede IPv6 precisa continuar utilizando controles como:

```text
Firewall
IDS
IPS
SIEM
EDR
IAM
MFA
Segmentação
Monitoramento
Criptografia
Políticas de acesso
Hardening
Logs
```

IPv6 deve ser tratado como parte da arquitetura de segurança.

Não como uma solução de segurança isolada.

---

# 🔎 19. IPv6 e reconhecimento de rede

Existe uma diferença interessante para profissionais de segurança.

O espaço de endereçamento IPv6 é gigantesco.

Isso torna muito menos prática a ideia de simplesmente fazer uma varredura sequencial de todo o espaço IPv6.

Por outro lado, isso não significa que IPv6 seja "invisível".

Atacantes podem utilizar:

* DNS;
* registros públicos;
* logs;
* informações de roteamento;
* serviços expostos;
* certificados;
* mecanismos de descoberta;
* endereços conhecidos;
* engenharia social.

Portanto:

> **IPv6 muda a superfície de ataque, mas não elimina a necessidade de segurança.**

---

# 🌐 20. IPv6 e Internet das Coisas

Um dos grandes motivos para o IPv6 ser estratégico é o crescimento da:

## Internet of Things — IoT

Imagine uma empresa com:

```text
10.000 sensores
```

Uma cidade inteligente com:

```text
1.000.000+ dispositivos
```

Uma indústria com:

```text
sensores
robôs
câmeras
controladores
atuadores
máquinas
```

A quantidade de dispositivos conectados tende a crescer continuamente.

O enorme espaço de endereçamento do IPv6 torna o protocolo especialmente adequado para esse cenário.

---

# 📡 21. IPv6 e 5G

IPv6 também possui forte relação com as redes móveis modernas.

Arquiteturas de:

* 4G;
* 5G;
* IoT;
* edge computing;
* redes privadas;

precisam lidar com enormes quantidades de dispositivos e sessões.

O IPv6 fornece uma base de endereçamento muito mais escalável para essas arquiteturas.

---

# ☁️ 22. IPv6 e Cloud Computing

A computação em nuvem também aumenta a necessidade de endereçamento.

Ambientes modernos podem possuir:

```text
Máquinas virtuais
Containers
Load Balancers
Microserviços
APIs
Bancos de dados
Clusters
Kubernetes
Serviços distribuídos
```

Em grandes ambientes, o número de endpoints pode crescer rapidamente.

IPv6 permite trabalhar com uma quantidade de endereços muito maior e pode simplificar determinadas arquiteturas que anteriormente dependiam fortemente de NAT.

---

# 🏢 23. IPv6 nas empresas

A adoção do IPv6 não deve ser vista somente como responsabilidade dos provedores de Internet.

Empresas também precisam preparar:

```text
Firewalls
Switches
Roteadores
Servidores
Sistemas operacionais
Aplicações
DNS
Monitoramento
VPN
Políticas de segurança
```

Uma infraestrutura corporativa moderna precisa compreender os dois protocolos durante o período de coexistência.

---

# 📊 24. O que as estatísticas do Google mostram?

O Google mantém uma página pública de estatísticas de adoção do IPv6.

A metodologia mede continuamente a disponibilidade de conectividade IPv6 entre usuários do Google e apresenta a porcentagem de usuários que acessam os serviços Google através de IPv6.

Isso torna os dados particularmente interessantes porque não estamos falando apenas de:

> "quantos equipamentos suportam IPv6?"

Estamos observando:

> **quantos usuários efetivamente conseguem acessar serviços através de IPv6.**

---

# 📈 25. Um marco histórico: IPv6 ultrapassando 50%

Um dos acontecimentos mais importantes da evolução recente ocorreu em 2026.

Segundo os dados publicados pelo Google e analisados pela Internet Society, o acesso nativo IPv6 ultrapassou 50% pela primeira vez em **28 de março de 2026**, chegando a **50,10%** naquele momento.

Isso significa que, naquele ponto da medição, mais da metade do acesso observado aos serviços Google ocorreu através de IPv6.

É um marco simbólico extremamente importante.

Durante anos, IPv6 foi considerado:

```text
"O futuro da Internet."
```

Hoje, essa afirmação precisa ser atualizada:

```text
IPv6 não é apenas o futuro.

IPv6 já faz parte do presente da Internet.
```

---

# 🌍 26. A adoção não acontece igualmente em todos os países

As estatísticas por país mostram que a implantação do IPv6 ocorre de maneira desigual.

Existem países e operadores com níveis muito elevados de adoção, enquanto outras regiões ainda possuem forte dependência do IPv4.

O próprio Google classifica as regiões considerando tanto a implantação quanto a experiência de conectividade IPv6.

Isso demonstra algo importante:

> **Adotar IPv6 não significa simplesmente ativar o protocolo.**

Também é necessário garantir:

* estabilidade;
* roteamento;
* desempenho;
* compatibilidade;
* segurança;
* monitoramento;
* qualidade da experiência do usuário.

---

# 🇧🇷 27. O cenário brasileiro

O Brasil possui uma participação significativa na implantação do IPv6.

A expansão do IPv6 brasileiro está relacionada principalmente ao crescimento das redes de banda larga, redes móveis e políticas de modernização da infraestrutura de Internet.

Para profissionais brasileiros de redes e segurança, isso significa que IPv6 deixou de ser apenas um assunto acadêmico.

Ele faz parte da realidade profissional.

---

# 🔐 28. IPv6 para profissionais de Cybersecurity

Para quem trabalha com:

```text
Cybersecurity
Network Security
SOC
Blue Team
Red Team
Pentest
Cloud Security
Infrastructure
Network Engineering
```

aprender IPv6 tornou-se cada vez mais importante.

Um profissional que conhece apenas IPv4 pode não compreender completamente uma infraestrutura moderna.

Durante uma análise de segurança, por exemplo, é necessário considerar:

```text
IPv4
IPv6
DNS
Routing
Firewall
ACL
VPN
ICMPv6
DHCPv6
SLAAC
Neighbor Discovery
```

Ignorar IPv6 pode significar ignorar parte da superfície real de uma rede.

---

# 🧠 29. IPv6 e ICMPv6

Outro ponto importante é o:

## ICMPv6

No IPv6, ICMPv6 possui papel fundamental no funcionamento do protocolo.

Ele participa de mecanismos como:

* Neighbor Discovery;
* Router Solicitation;
* Router Advertisement;
* Neighbor Solicitation;
* Neighbor Advertisement;
* Path MTU Discovery.

Por isso, bloquear ICMPv6 de maneira indiscriminada pode causar problemas de conectividade.

Isso exige uma abordagem de segurança mais cuidadosa.

---

# 🔍 30. IPv6 e Neighbor Discovery

No IPv4, uma função semelhante à descoberta de vizinhos é realizada pelo ARP.

No IPv6, temos:

```text
Neighbor Discovery Protocol
```

baseado em ICMPv6.

Ele permite que dispositivos descubram informações sobre vizinhos e roteadores.

Isso cria também uma área importante para segurança de redes.

---

# 🧱 31. IPv6 e Firewall

Uma rede corporativa não deve simplesmente habilitar IPv6 e assumir que está protegida.

É necessário verificar:

```text
Firewall IPv4
        +
Firewall IPv6
```

Também devem ser revisados:

* ACLs;
* regras de entrada;
* regras de saída;
* VPN;
* IDS/IPS;
* monitoramento;
* logging;
* segmentação;
* políticas de acesso.

Um dos erros clássicos de segurança é proteger muito bem IPv4 enquanto deixa IPv6 com controles inadequados.

---

# ⚔️ 32. IPv6 e ataques

IPv6 possui suas próprias possibilidades de ataque.

Exemplos de áreas que precisam de atenção:

```text
ICMPv6
Neighbor Discovery
Router Advertisement
DHCPv6
IPv6 Extension Headers
Rogue Router
Spoofing
DoS/DDoS
Misconfiguration
Firewall bypass
Dual Stack attacks
```

Isso reforça uma conclusão importante:

> **A implantação do IPv6 precisa ocorrer junto com uma estratégia de segurança.**

---

# 🔄 33. O grande desafio: Dual Stack

Durante a transição, muitas empresas possuem:

```text
IPv4 + IPv6
```

Isso significa que a superfície de configuração aumenta.

Um administrador pode configurar corretamente:

```text
IPv4 Firewall
```

mas esquecer:

```text
IPv6 Firewall
```

Ou proteger:

```text
IPv4 DNS
```

e esquecer:

```text
IPv6 DNS
```

Por isso, ambientes Dual Stack exigem atenção especial.

---

# 📋 34. Checklist profissional para implantação IPv6

Uma empresa que pretende implementar IPv6 deve avaliar:

```text
[ ] Inventário de equipamentos
[ ] Compatibilidade de switches
[ ] Compatibilidade de roteadores
[ ] Firewalls
[ ] Servidores
[ ] Sistemas operacionais
[ ] Aplicações
[ ] DNS
[ ] DHCPv6
[ ] SLAAC
[ ] Monitoramento
[ ] Logs
[ ] IDS/IPS
[ ] VPN
[ ] Políticas de segurança
[ ] Treinamento da equipe
[ ] Plano de endereçamento
[ ] Plano de roteamento
[ ] Testes
[ ] Documentação
[ ] Plano de contingência
```

---

# 📚 35. IPv6 não é apenas uma atualização

É importante entender que IPv6 não deve ser tratado como:

```text
IPv4 versão 2
```

Ele representa uma evolução arquitetural.

Existem mudanças em:

* endereçamento;
* descoberta de vizinhos;
* roteamento;
* autoconfiguração;
* cabeçalho;
* fragmentação;
* multicast;
* anycast;
* gerenciamento;
* segurança operacional.

Por isso, aprender IPv6 exige compreender seus próprios conceitos.

---

# 🧭 36. A evolução da Internet em perspectiva

Podemos resumir essa evolução:

```text
Internet inicial
       ↓
IPv4
       ↓
Crescimento da Internet
       ↓
Escassez de endereços
       ↓
NAT + técnicas de conservação
       ↓
Desenvolvimento do IPv6
       ↓
Dual Stack
       ↓
Expansão do IPv6
       ↓
IoT + Cloud + 5G
       ↓
IPv6 como infraestrutura dominante
```

---

# 🚀 37. O futuro

A Internet continuará crescendo.

Novos dispositivos serão conectados.

Novos serviços serão criados.

A computação continuará migrando para:

```text
Cloud
Edge
IoT
5G
6G
Automação
IA
Smart Cities
Indústria 4.0
```

Todas essas tecnologias dependem de conectividade.

E conectividade depende de endereçamento.

Nesse cenário, o IPv6 deixa de ser apenas uma alternativa ao IPv4.

Ele se torna uma infraestrutura estratégica para o crescimento da Internet.

---

# 🎯 38. Por que aprender IPv6?

Para profissionais de tecnologia, aprender IPv6 significa estar preparado para trabalhar com uma Internet que já está em processo de transformação.

Conhecer IPv6 é importante para:

### 🌐 Redes

Compreender endereçamento, roteamento e conectividade moderna.

### 🔐 Cybersecurity

Identificar e proteger superfícies de ataque IPv6.

### ☁️ Cloud

Trabalhar com arquiteturas modernas de infraestrutura.

### 📡 Telecom

Compreender redes móveis e infraestrutura de larga escala.

### 🤖 IoT

Projetar redes para grandes quantidades de dispositivos.

### 🖥️ Infraestrutura

Administrar servidores e equipamentos modernos.

### 🛡️ Pentest

Identificar ativos e serviços IPv6 durante avaliações de segurança.

---

# 💡 39. Uma mudança de mentalidade

Durante muito tempo, aprender redes significava principalmente aprender:

```text
IPv4
Subnetting
NAT
DHCP
ARP
```

Esses conhecimentos continuam sendo fundamentais.

Porém, o profissional de redes moderno precisa ampliar essa visão:

```text
IPv4
+
IPv6
+
DNS
+
Routing
+
Security
+
Cloud
+
Automation
+
Monitoring
```

O conhecimento de IPv4 não desaparece.

Ele passa a coexistir com IPv6 durante uma longa fase de transição.

---

# 🧩 40. Conclusão

O IPv4 foi fundamental para a construção da Internet moderna.

Sem ele, a expansão global da Internet provavelmente teria ocorrido de maneira muito diferente.

Mas a Internet mudou.

A quantidade de dispositivos cresceu.

As aplicações evoluíram.

As redes móveis cresceram.

A computação em nuvem se tornou dominante.

A Internet das Coisas expandiu.

A necessidade de conectividade aumentou.

E a arquitetura de endereçamento precisou evoluir.

O IPv6 surgiu justamente nesse contexto.

Com:

```text
128 bits
```

de endereçamento, autoconfiguração, novas possibilidades de hierarquia, multicast, anycast e uma arquitetura projetada para uma escala muito maior, o IPv6 representa uma das principais evoluções técnicas da Internet.

E os dados atuais mostram que essa evolução já está acontecendo.

O marco de mais de **50% de acesso nativo IPv6 observado pelo Google em 2026** demonstra que IPv6 deixou definitivamente de ser apenas um projeto para o futuro.

---

# 🌐 IPv6 não é o futuro.

## IPv6 é a Internet evoluindo.

A transição ainda está acontecendo.

IPv4 continuará presente por muitos anos.

Mas compreender IPv6 hoje significa estar preparado para as redes que já estão sendo construídas.

---

# 📌 Principais conceitos estudados

```text
IPv4
IPv6
Endereçamento IP
32 bits
128 bits
NAT
SLAAC
DHCPv6
ICMPv6
Neighbor Discovery
Multicast
Anycast
Dual Stack
Túneis IPv6
NAT64
DNS64
Roteamento
Firewall
Segurança de Redes
IoT
5G
Cloud Computing
Cybersecurity
```

---

# 📚 Referências

* Google IPv6 Statistics
* IETF — RFC 8200
* Internet Society — IPv6 Deployment
* IANA — IPv6 Address Space

---

# 🔗 Fontes

**Google — IPv6 Statistics:**
https://www.google.com/intl/en/ipv6/statistics.html

**IETF — RFC 8200 — IPv6 Specification:**
https://www.rfc-editor.org/rfc/rfc8200/

**IANA — IPv6 Address Space:**
https://www.iana.org/assignments/ipv6-address-space

---

# 💻 Área de interesse

**Redes de Computadores | IPv6 | Cybersecurity | Linux | Cloud Computing | Infraestrutura | Segurança da Informação**

---

# 🚀 Aprender redes é entender como a Internet funciona.

# 🔐 Aprender IPv6 é entender para onde ela está indo.
