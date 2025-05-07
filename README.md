
# Treinamento Redes Corporativas MATVSUL

Este repositório contém todo o material gerado no curso de **Treinamento de Redes Corporativas** na MATVSUL. Aqui você encontrará scripts de configuração, guias passo‑a‑passo e documentação oficial para implantar e gerenciar sua infraestrutura de rede utilizando equipamentos Intelbras.

---

## 📂 Estrutura de Pastas

```

network-training-matvsul/
├── README.md
├── firewall
│   ├── r3005g\_user\_accounts.json
│   ├── r3005g\_vlans.json
│   ├── r3005g\_multwan.json
│   └── r3005g\_openvpn.json
├── switches
│   ├── s3328
│   │   ├── vlans\_and\_svis.txt
│   │   └── dhcp\_pools.txt
│   └── s2328
│       └── port\_settings.txt
├── ap
│   └── ax3000\_config.md
├── network\_plan
│   ├── ip\_addressing\_scheme.txt
│   └── provisionamento\_de\_rede\_10-0-10-0\_20.txt
├── docs
│   ├── Datasheet‑R3005G\_1.pdf
│   ├── R3005G\_Guia\_Instalacao.pdf
│   ├── R3005G\_Configuracao\_Via\_Script.pdf
│   ├── R3005G\_Manual\_Usuario.pdf
│   ├── 02\_Configuracoes\_tecnologias\_virtuais.pdf
│   ├── 03\_Configurando\_interfaces\_Ethernet.pdf
│   ├── 04\_Protocolo\_IP\_Servicos.pdf
│   ├── 05\_Roteamento\_Unicast.pdf
│   ├── 07\_ACL\_QoS.pdf
│   └── 12\_OpenFlow\.pdf
└── examples
└── comware\_qos\_acl\_example.sh

````

---

## 🔖 Sobre o Curso

- **Objetivo**: Capacitar profissionais na implantação e gerenciamento de redes corporativas com foco em segurança, VLANs, DHCP, QoS, ACLs, balanceamento de links e VPN.
- **Público‑alvo**: Administradores de rede, engenheiros de infraestrutura e estudantes de TI.
- **Carga horária**: 16 horas (2 dias presenciais).

---

## 🚀 Conteúdo

### 1. Firewall R3005G  
Arquivos JSON importáveis via interface Web → **Configuração → Importar**  
- `firewall/r3005g_user_accounts.json` – contas de administrador  
- `firewall/r3005g_vlans.json`       – definição de VLANs e DHCP  
- `firewall/r3005g_multwan.json`     – balanceamento e failover de links  
- `firewall/r3005g_openvpn.json`     – servidor OpenVPN na VLAN de gestão

### 2. Switch Layer‑3 S3328  
Comandos Comware para SVIs e DHCP  
- `switches/s3328/vlans_and_svis.txt` – criação de VLANs e interfaces L3  
- `switches/s3328/dhcp_pools.txt`      – configuração de pools DHCP globais

### 3. Switch Layer‑2 S2328  
Portas de acesso/trunk para câmeras, AP e gestão  
- `switches/s2328/port_settings.txt`

### 4. AP AX3000  
Guia em Markdown para SSIDs e VLANs  
- `ap/ax3000_config.md`

### 5. Plano de Endereçamento  
Esquema de rede principal 10.0.10.0/20 e sub‑redes /24  
- `network_plan/ip_addressing_scheme.txt`  
- `network_plan/provisionamento_de_rede_10-0-10-0_20.txt`

### 6. Documentação de Referência  
PDFs oficiais e guias técnicos  
- VLAN, QoS, ACL, OpenFlow, roteamento, protocolos IP etc. em `docs/`

### 7. Exemplos Práticos  
Script completo combinando QoS, ACL e VLAN em Comware  
- `examples/comware_qos_acl_example.sh`

---

## ✔️ Passo a Passo

1. **Clone este repositório**  
   ```bash
   git clone https://github.com/SEU_USUARIO/network-training-matvsul.git
   cd network-training-matvsul
````

2. **Configure o R3005G**

   * Acesse a GUI do R3005G
   * Importe os JSONs de `firewall/`

3. **Configure o Switch S3328**

   * Acesse CLI
   * Cole e execute os arquivos de `switches/s3328/`

4. **Configure o Switch S2328**

   * No CLI, aplique `switches/s2328/port_settings.txt`

5. **Configure o AP AX3000**

   * Siga o passo‑a‑passo em `ap/ax3000_config.md`

6. **Verifique e teste**

   * Acesse VLAN de gestão (10.0.99.0/24)
   * Teste DHCP em cada VLAN
   * Valide acesso VPN e balanceamento de links
   * Confira captive portal para visitantes

---

## 🤝 Contribuições

Contribuições são bem‑vindas! Para colaborar:

1. Abra uma **Issue** descrevendo bugs ou sugestões.
2. Faça um **Fork** e crie uma **Branch** para sua feature/fix.
3. Envie um **Pull Request** detalhando alterações.

---

Curso Treinamento Redes Corporativas • Maio/2025

