# Projeto QA: Sistema de Conciliação de Cartões

Este projeto demonstra a estruturação completa de um fluxo de QA para conciliação financeira, com foco em integridade de dados e conformidade com LGPD.

## 🛠️ Ferramentas Utilizadas
* **Google Sheets**: Planejamento e Matriz de Casos de Teste. [Acesse a Planilha aqui](https://google.com)
* **Jira Service Management**: Gestão de incidentes e documentação técnica.
* **GitHub**: Portfólio e histórico de documentação.

---

## 🐞 Detalhamento das Falhas Identificadas

### 1. Divergência de Nomenclatura - Bandeira Elo (QCT-1)
O sistema não reconhece a bandeira devido a máscaras de texto incompatíveis.
**Evidências:**
![Planilha Elo](planilha-elo.jpeg) ![Sistema Elo](sistema-elo.jpeg) ![Jira QCT-1](jira-qct1.png)

### 2. Falso Positivo - Mastercard vs Visa (QCT-4)
O sistema valida como "OK" transações com bandeiras divergentes entre operadora e sistema.
**Evidências:**
![Planilha Master](planilha-master.jpeg) ![Sistema Master](sistema-master.jpeg) ![Jira QCT-4](jira-qct4.png)

### 3. Falso Positivo - Crédito vs Débito na Cielo (QCT-5)
Falha crítica onde o sistema não diferencia a modalidade de pagamento, aceitando dados divergentes.
**Evidências:**
![Planilha Cielo](planilha-cielo.jpeg) ![Sistema Cielo](sistema-cielo.jpeg) ![Jira QCT-5](jira-qct5.png)

---
*Nota: Todos os dados sensíveis foram protegidos (tarjas vermelhas/pretas) para garantir a segurança da informação.*

