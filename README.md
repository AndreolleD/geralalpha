# Guia Alternativo de Redes e Git

## 1. Redes: visão geral

### 1.1 Como uma rede pode ser montada
Existem vários desenhos possíveis para conectar dispositivos. Em redes domésticas, quase sempre tudo se liga a um único roteador. Já em ambientes maiores, é comum usar múltiplos caminhos para evitar que uma falha derrube tudo.

### 1.2 Tipos de rede por alcance
- **PAN:** dispositivos muito próximos, como smartwatch e celular.  
- **LAN:** redes locais, típicas de casas e escritórios.  
- **MAN:** cobertura maior, geralmente usada por provedores de cidade.  
- **WAN:** longas distâncias, como a comunicação entre países.

### 1.3 Redes internas e externas
- **Internet:** acessível a qualquer pessoa.  
- **Intranet:** usada internamente em empresas.  
- **Extranet:** parecida com a intranet, mas com acessos externos controlados.

---

## 2. Desempenho e controle de tráfego

### 2.1 Latência
A latência é o tempo que os dados levam para ir e voltar. Quanto menor, melhor para jogos, chamadas e vídeos.

### 2.2 QoS (Quality of Service)
Quando uma rede tem muito tráfego, o QoS ajuda a decidir o que é mais importante. Assim você consegue priorizar, por exemplo, a chamada de vídeo em vez de um download.

---

## 3. Protocolos essenciais

### 3.1 TCP e UDP
- **TCP:** garante entrega, ordem dos pacotes e confiabilidade.  
- **UDP:** não garante nada, mas é rápido e eficiente quando pequenas perdas não prejudicam (streaming, jogos, VoIP).

### 3.2 HTTP e HTTPS
- **HTTP:** comunicação sem criptografia.  
- **HTTPS:** usa TLS para garantir que os dados não sejam lidos no caminho.

### 3.3 DNS
O DNS faz a tradução entre nomes e endereços IP. Sem ele, precisaríamos decorar números como `142.250.78.14` em vez de `google.com`.

---

## 4. Wi-Fi e segurança wireless

### 4.1 Padrões de segurança
- **WEP:** ultrapassado e vulnerável.  
- **WPA / WPA2:** padrões modernos e mais seguros.  
- **WPA3:** versão atual com melhorias de criptografia.

---

## 5. Endereços IP

### 5.1 IPv4
Usa números separados por pontos (ex.: 192.168.0.1). Como o estoque de endereços acabou, se usa muito NAT para reaproveitar IPs.

### 5.2 IPv6
Tem muito mais espaço de endereços, dispensa NAT e já inclui recursos modernos de segurança.

---

## 6. Segurança da informação

### 6.1 Criptografia
- **Simétrica:** mesma chave para cifrar e decifrar.  
- **Assimétrica:** usa par de chaves (pública e privada).

### 6.2 TLS e certificados
O TLS garante que a conexão entre cliente e servidor seja protegida. A autenticação é feita por certificados emitidos por autoridades confiáveis.

### 6.3 Ataques comuns
- DDoS  
- Malware  
- Engenharia social  
- Exploração de falhas  
Boas práticas incluem firewalls, IDS/IPS, atualizações e conscientização de usuários.

---

## 7. Tecnologias modernas em rede
- **Cloud:** infraestrutura elástica e distribuída.  
- **CDN:** entrega conteúdo de forma rápida usando servidores mais próximos do usuário.  
- **VPN:** cria túneis seguros sobre redes abertas.  
- **IoT:** dispositivos simples que exigem protocolos leves e cuidados extras de segurança.

---

# Parte 2 — Git e Controle de Versão

## 8. Fundamentos do Git

### 8.1 Estrutura interna
O Git usa três áreas:
- **Working Directory:** onde você altera arquivos.  
- **Staging Area:** fila do que vai entrar no próximo commit.  
- **Repository (.git):** histórico e metadados.

### 8.2 Commits e hashes
Cada commit gera um hash único baseado no conteúdo e nas informações do commit. Mudar qualquer detalhe gera outro hash.

---

## 9. Branches

### 9.1 O que é uma branch
Uma branch é basicamente um ponteiro que aponta para o último commit daquela linha de trabalho.

### 9.2 Movimentação do ponteiro
Sempre que você cria um novo commit, a branch avança para esse commit automaticamente.

---

## 10. Merge e resolução de conflitos

### 10.1 Tipos de merge
- **Fast-forward:** quando a branch de destino pode simplesmente avançar sem criar commit extra.  
- **Merge com commit:** criado quando há divergência entre históricos.

### 10.2 Conflitos
Quando duas mudanças afetam a mesma parte do arquivo, o Git pede que você resolva manualmente.

---

## 11. Remotos e colaboração

### 11.1 Repositórios remotos
Você conecta seu projeto a um servidor externo com:
