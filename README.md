# Santander-Code-Girls-Projeto1

# 🚀 Desafio AWS EC2 – Documentação de Estudo

Este repositório foi criado como parte do desafio da [DIO](https://www.dio.me) para consolidar meus conhecimentos em **gerenciamento de instâncias EC2 na AWS**.  
Aqui documento todo o processo, insights e aprendizados adquiridos durante as aulas e práticas.

---

## 🎯 Objetivos do Desafio
- Aplicar os conceitos aprendidos em um ambiente prático na AWS.  
- Documentar processos técnicos de forma clara e estruturada.  
- Utilizar o GitHub como ferramenta de versionamento e compartilhamento de documentação.  

---

## 📚 Conteúdos Estudados
Durante o laboratório foram explorados os seguintes tópicos:

1. **Criação de instância EC2**
   - Escolha da região
   - Seleção do sistema operacional (Amazon Linux, Ubuntu, Windows Server etc.)
   - Tipos de instância (t2.micro, t3.micro etc.)

2. **Configuração de chaves**
   - Geração do par de chaves `.pem`
   - Conversão para `.ppk` no Windows (quando necessário)
   - Importância da segurança e backup da chave

3. **Security Groups**
   - Regras de **Inbound** (entrada) e **Outbound** (saída)  
   - Exemplo: abrir porta 22 (SSH) apenas para o meu IP  
   - Exemplo: abrir porta 80 (HTTP) para qualquer origem

4. **Conexão na instância**
   - Acesso via SSH no Linux/Mac  
   - Acesso via **PuTTY/OpenSSH** no Windows  
   - Comando usado:  
     ```bash
     ssh -i "minha-chave.pem" ec2-user@IP_DA_INSTANCIA
     ```

5. **Gerenciamento**
   - Start, Stop e Terminate da instância  
   - Diferença entre desligar (Stop) e encerrar (Terminate)  
   - Custos associados ao uso contínuo  

6. **Armazenamento**
   - Volume EBS associado à instância  
   - Persistência de dados (EBS vs instância temporária)  

---

## 🖼️ Prints e Evidências
As capturas de tela estão no repositório para registrar cada etapa:  
- Criação da instância - deixei foto da lista com as duas instancias, servidor01 e servidor02 
- Configuração do Security Group  - coloquei uma foto das especificações dela
- Conexão SSH bem-sucedida  - tem uma foto do moba mostrando o top.

---

## 💡 Insights e Aprendizados
- **Responsabilidade compartilhada**: AWS cuida da infraestrutura, eu cuido da configuração.  
- É fundamental **restringir acessos** no Security Group, nunca deixar portas abertas sem necessidade.  
- Usar instâncias **free tier (t2.micro)** ajuda a praticar sem custos adicionais.  
- Conectar via SSH pela primeira vez pode ser desafiador, mas depois vira rotina.  



## 👩‍💻 Autor
Desafio desenvolvido por **Nathalia Macedo** como parte do curso da **DIO**.  
Este repositório servirá como base de estudos para práticas futuras em **AWS**.
