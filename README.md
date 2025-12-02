# 🌐 Guia Alternativo de Redes e Git

## 🖧 1. Redes: visão geral

### 🔗 1.1 Como uma rede pode ser montada
As redes podem ser organizadas de vários jeitos. Em casas, normalmente tudo conversa com um único roteador. Em empresas, é comum usar caminhos redundantes para evitar quedas.

### 📡 1.2 Tipos de rede por alcance
- **📱 PAN:** dispositivos próximos (Bluetooth, smartwatch).  
- **🏠 LAN:** redes domésticas ou de escritório.  
- **🏙️ MAN:** redes que cobrem regiões urbanas.  
- **🌍 WAN:** longas distâncias, incluindo a Internet.

### 🔒 1.3 Redes internas e externas
- **🌐 Internet:** aberta ao público.  
- **🏢 Intranet:** rede privada dentro de organizações.  
- **🔑 Extranet:** acesso restrito para pessoas externas autorizadas.

---

## ⚙️ 2. Desempenho e controle de tráfego

### ⏱️ 2.1 Latência
Latência é o tempo que leva para um pacote ir e voltar. Menos latência = melhor experiência em jogos, chamadas e streaming.

### 🎚️ 2.2 QoS (Quality of Service)
QoS permite definir prioridades. Assim, chamadas de vídeo e VoIP não travam quando a rede está ocupada.

---

## 📡 3. Protocolos essenciais

### 🔁 3.1 TCP x UDP
- **📦 TCP:** garante entrega e ordem dos dados.  
- **🚀 UDP:** mais rápido e leve, sem garantias.

### 🔐 3.2 HTTP x HTTPS
- **HTTP:** dados enviados sem proteção.  
- **HTTPS:** usa TLS para criptografar.

### 🌍 3.3 DNS
Sistema que traduz nomes como `google.com` em endereços IP. Sem o DNS, seria necessário memorizar números.

---

## 📶 4. Wi-Fi e segurança wireless

### 🛡️ 4.1 Padrões de segurança
- **❌ WEP:** inseguro.  
- **✔️ WPA / WPA2:** seguros e usados amplamente.  
- **🔒 WPA3:** padrão mais recente, recomendado.

---

## 🧩 5. Endereços IP

### 🔢 5.1 IPv4
Formato tradicional (ex.: `192.168.0.1`). Como o número de endereços acabou, o NAT virou padrão em redes domésticas.

### 🆕 5.2 IPv6
Mais moderno, muito mais espaço de endereços e melhorias em segurança.

---

## 🛡️ 6. Segurança da informação

### 🔑 6.1 Criptografia
- **⚡ Simétrica:** mesma chave para tudo.  
- **🔐 Assimétrica:** par de chaves (pública/privada).

### 🧾 6.2 TLS e certificados
O TLS mantém a conexão segura e usa certificados digitais para validar servidores.

### ⚠️ 6.3 Ameaças comuns
- DDoS  
- Malware  
- Engenharia social  
- Exploração de vulnerabilidades  
Boas práticas incluem firewalls, IDS/IPS, atualizações e treinamento.

---

## 🚀 7. Tecnologias modernas

- **☁️ Cloud:** infraestrutura flexível e escalável.  
- **🌎 CDN:** servidores distribuídos para entregar conteúdo mais rápido.  
- **🛣️ VPN:** túnel seguro mesmo em redes públicas.  
- **📟 IoT:** dispositivos simples que exigem protocolos leves e segurança reforçada.

---

# 🧰 Git e Controle de Versão

## 📁 8. Fundamentos do Git

### 📂 8.1 Áreas internas
- **📝 Working Directory:** onde você edita.  
- **📤 Staging Area:** preparação para commit.  
- **📦 .git:** armazenamento do histórico.

### 🧱 8.2 Commits e hashes
Cada commit é identificado por um hash único criado a partir do conteúdo e metadados.

---

## 🌿 9. Branches

### 🍃 9.1 O que é uma branch
Uma branch é só um ponteiro que aponta para o último commit daquela linha.

### 🔄 9.2 Como ela avança
Ao criar um novo commit, a branch automaticamente aponta para ele.

---

## 🔀 10. Merge e conflitos

### ⚡ 10.1 Tipos de merge
- **➡️ Fast-forward:** avança sem criar commit extra.  
- **🔧 Merge normal:** cria um commit de união.

### ❗ 10.2 Conflitos
Quando duas alterações mexem na mesma parte do arquivo, o Git exige que você resolva manualmente.

---

## 🌍 11. Remotos e colaboração

### 🔗 11.1 Adicionando remote
