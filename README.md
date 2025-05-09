
# Treinamento Redes Corporativas MATVSUL

Este repositório contém todo o material gerado no curso de **Treinamento de Redes Corporativas** na MATVSUL. Aqui você encontrará scripts de configuração, guias passo‑a‑passo e documentação oficial para implantar e gerenciar sua infraestrutura de rede utilizando equipamentos Intelbras.

---

## 📂 Estrutura de Pastas

```

network-training-matvsul/
├── README.md
├── firewall
│   ├── r3005g
├── switches
│   ├── s3328
│   └── s2328
├── ap
│   └── ax3000
├── network\_plan
│   ├── ip\_addressing\_scheme.txt
│   └── provisionamento\_de\_rede\_10-0-10-0\_20.txt
├── docs
│   ├── Datasheet‑R3005G\_1.pdf
│   ├── R3005G\_Guia\_Instalacao.pdf
│   ├── R3005G\_Configuracao\_Via\_Script.pdf
│   ├── R3005G\_Manual\_Usuario.pdf
└── examples

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
- `firewall/` – contas de administrador  
- `firewall/`       – definição de VLANs e DHCP  
- `firewall/`     – balanceamento e failover de links  
- `firewall/`     – servidor OpenVPN na VLAN de gestão

### 2. Switch Layer‑3 S3328  
Comandos Comware para SVIs e DHCP  
- `switches/s3328/ – criação de VLANs e interfaces L3  
- `switches/s3328/ – configuração de pools DHCP globais

### 3. Switch Layer‑2 S2328  
Portas de acesso/trunk para câmeras, AP e gestão  
- `switches/s2328/`

### 4. AP AX3000  
Guia em Markdown para SSIDs e VLANs  
- `ap/ax3000_config.md`

### 5. Plano de Endereçamento  
Esquema de rede principal 10.0.10.0/20 e sub‑redes /24  
- `network_plan/`  
- `network_plan/`

### 6. Documentação de Referência  
PDFs oficiais e guias técnicos  
- VLAN, QoS, ACL, OpenFlow, roteamento, protocolos IP etc. em `docs/`

### 7. Exemplos Práticos  
Script completo combinando QoS, ACL e VLAN em Comware  
- `examples/comware_qos_acl_example.sh`

---

## ✔️ Passo a Passo

1. **repositório**  
   ```bash
   git clone https://github.com/SEU_USUARIO/network-training-matvsul.git
   cd network-training-matvsul
````

2. **Configure o R3005G**

   * Acesse a GUI do R3005G
   * Importe os JSONs de 

3. **Configure o Switch S3328**

   * Acesse CLI
   * Cole e execute os arquivos de 

4. **Configure o Switch S2328**

   * No CLI, aplique 

5. **Configure o AP AX3000**

   * Siga o passo‑a‑passo em 

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

