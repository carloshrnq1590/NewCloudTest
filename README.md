Desafio Prático Google Cloud Platform (GCP)


📌 Objetivo


Este desafio tem como objetivo testar seus conhecimentos práticos na GCP, incluindo criação de infraestrutura, deploy de aplicações e automação.

Cada tarefa contém instruções específicas e o que você precisa enviar para análise.

📜 Requisitos

Ter uma conta na Google Cloud Platform.
Ter o gcloud CLI instalado e autenticado.
Opcional: Docker e Terraform instalados.


🚀 Desafio 1 - Criando Infraestrutura na GCP

✅ Tarefa 1: Criar uma VM Compute Engine

Criar uma VM chamada minha-vm com as seguintes configurações:

Ubuntu 22.04 LTS.

Tipo de máquina: e2-micro (dentro do Free Tier).

Disco de 10GB SSD padrão.

Uma tag de firewall personalizada (minha-vm).

📩 O que enviar para análise?

Captura de tela da VM rodando no Console GCP.

Saída do comando:

gcloud compute instances describe minha-vm

![image](https://github.com/user-attachments/assets/0fa9737e-1a70-40d9-8f19-c64b8b27d838)






✅ Tarefa 2: Configurar uma VPC Personalizada

Criar uma VPC customizada chamada minha-vpc.

Criar duas sub-redes:

publica-subrede: CIDR 10.0.1.0/24
privada-subrede: CIDR 10.0.2.0/24

Criar uma regra de firewall para permitir conexões HTTP (porta 80) apenas na publica-subrede.

📩 O que enviar para análise?

Captura de tela da configuração da VPC e das sub-redes.

Saída do comando:

gcloud compute networks subnets list --filter="network: minha-vpc"


![Sem título](https://github.com/user-attachments/assets/4bba247b-1c0d-46e1-b640-c8bf65d62de7)

