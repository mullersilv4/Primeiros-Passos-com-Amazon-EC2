# Primeiros-Passos-com-Amazon-EC2
Este projeto demonstra como lançar instâncias **Amazon EC2** em diferentes **Availability Zones** (AZs) dentro da mesma região da AWS, garantindo maior resiliência para aplicações.


## 🎯 Objetivo
- Implantar um sistema de estabilização em duas instâncias EC2 em zonas de disponibilidade separadas.  
- Configurar um script simples de dados do usuário (*user data*) para exibir os detalhes da instância em um navegador.  

---

## 🛠️ Serviços AWS Utilizados
- **Amazon EC2** → Máquinas virtuais em nuvem.  
- **Amazon EBS** → Volumes de armazenamento persistente associados às instâncias.  
- **VPC/Subnets** → Estrutura de rede para separar as Availability Zones.  

---

## 🚀 Etapas Realizadas
1. Criação de uma **instância EC2** na **Availability Zone A**.  
2. Associação de um volume **Amazon EBS** à instância.  
3. Configuração de script via **user data** para inicializar e exibir informações no navegador.  
4. Criação de uma **segunda instância EC2** na **Availability Zone B** para redundância.  
5. Associação de um volume **Amazon EBS** à segunda instância.  
6. Teste de acesso às instâncias via navegador para validar a configuração.  

---

## 📊 Resultado
- O sistema de estabilização foi distribuído entre **duas zonas de disponibilidade**, garantindo maior tolerância a falhas.  
- Cada instância EC2 ficou acessível individualmente, exibindo seus dados de inicialização.  

---

## 🔧 Próximos Passos (Evoluções Futuras)
- Criar um **Elastic Load Balancer (ELB)** para distribuir o tráfego entre as instâncias.  
- Utilizar **Auto Scaling Groups** para ajustar a quantidade de instâncias de acordo com a demanda.  
- Integrar **CloudWatch** para monitoramento e alarmes de disponibilidade.  

---

## 📷 Diagrama da Arquitetura
[📷 Ver Diagrama da Arquitetura]([./imagens/diagrama-ec2.png](https://github.com/mullersilv4/Primeiros-Passos-com-Amazon-EC2/issues/1))
