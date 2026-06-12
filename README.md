# 🧸 Taskids - Gerenciamento de Tarefas para Crianças

![Taskids](https://img.shields.io/badge/version-1.0.0-blue.svg) ![License](https://img.shields.io/badge/license-MIT-green.svg)

## 📖 Sobre o Projeto

**Taskids** é uma aplicação web projetada para ajudar pais e responsáveis a gerenciar tarefas e deveres das crianças de forma lúdica e educativa. O sistema incentiva o cumprimento de responsabilidades diárias através de um sistema de recompensas (mesada) que pode ser configurado pelos pais.

Baseado em boas práticas de educação infantil, o Taskids transforma tarefas cotidianas em missões que geram recompensas, ensinando desde cedo sobre responsabilidade, organização e consequências (positivas e negativas).

---

## 🎯 Público-alvo

| Usuário | Função |
|---------|--------|
| 👧 **Crianças** | Visualizar tarefas do dia, marcar como concluídas, acompanhar saldo acumulado |
| 👨‍👩‍👧 **Pais/Admin** | Criar/editar/excluir tarefas, definir valores, configurar periodicidade da mesada, acompanhar desempenho |

---

## ✨ Funcionalidades Principais

### Para Crianças
- ✅ Visualizar lista de tarefas do dia
- ✅ Marcar tarefas como **concluída** ou **não concluída**
- ✅ Acompanhar saldo atual (mesada acumulada)
- ✅ Interface simples, colorida e intuitiva
- ✅ Apenas acesso aos marcadores (sem edição de tarefas)

### Para Pais (Admin)
- ➕ Criar, editar e excluir tarefas personalizadas
- 💰 Definir valor por tarefa (ex: R$ 0,50 por "Escovar os dentes")
- 📅 Configurar periodicidade da mesada: **semanal** ou **mensal**
- 🔄 Definir regras de remuneração:
  - Tarefa **concluída** → acrescenta o valor
  - Tarefa **não concluída** → desconta o valor
- 👀 Acompanhar histórico de cumprimento por criança
- 📊 Visualizar relatório de desempenho

---

## 📋 Exemplos de Tarefas (baseado nas imagens)

### Regras e Deveres
| Tarefa | Valor sugerido |
|--------|----------------|
| Dormir no horário | R$ 0,50 |
| Tomar banho | R$ 0,50 |
| Fazer a lição de casa | R$ 1,00 |
| Colocar a roupa suja no cesto | R$ 0,25 |
| Cuidar dos brinquedos e pertences | R$ 0,50 |
| Ajudar nas tarefas de casa | R$ 0,75 |
| Obedecer ao papai e mamãe | R$ 1,00 |

### Hábitos Diários
| Tarefa | Valor sugerido |
|--------|----------------|
| Escovar os dentes | R$ 0,25 |
| Lavar as mãos | R$ 0,25 |
| Comer fruta | R$ 0,50 |
| Acordar no horário | R$ 0,50 |
| Ir para a escola | R$ 0,50 |
| Hora da leitura | R$ 0,75 |

### Comportamento Social
| Tarefa | Valor sugerido |
|--------|----------------|
| Ser amável e educado | R$ 0,50 |
| Dividir os brinquedos com os amigos | R$ 0,50 |
| Não gritar e nem chorar sem motivo | R$ 0,25 |
| Não falar palavrão | R$ 0,25 |
| Não brigar | R$ 0,50 |
| Não fazer birras | R$ 0,50 |

### Palavras Mágicas (bônus)
| Palavra | Bônus |
|---------|-------|
| Oi / Olá | +R$ 0,10 |
| Obrigado | +R$ 0,10 |
| Por favor | +R$ 0,10 |
| Com licença | +R$ 0,10 |
| Desculpe | +R$ 0,10 |
| Bom dia / Boa tarde / Boa noite | +R$ 0,10 |
| Tchau | +R$ 0,10 |

---

## 🧮 Exemplo de Cálculo da Mesada

### Configuração dos Pais
- **Periodicidade:** Semanal
- **Dia de pagamento:** Domingo

### Cenário da Criança (Arthur)

| Dia | Tarefas Concluídas | Tarefas Não Concluídas | Saldo do dia |
|-----|-------------------|------------------------|---------------|
| Segunda | 5 tarefas (+R$ 2,50) | 1 tarefa (-R$ 0,50) | +R$ 2,00 |
| Terça | 6 tarefas (+R$ 3,00) | 0 tarefas | +R$ 3,00 |
| Quarta | 4 tarefas (+R$ 2,00) | 2 tarefas (-R$ 1,00) | +R$ 1,00 |
| Quinta | 7 tarefas (+R$ 3,50) | 0 tarefas | +R$ 3,50 |
| Sexta | 5 tarefas (+R$ 2,50) | 1 tarefa (-R$ 0,50) | +R$ 2,00 |
| Sábado | 3 tarefas (+R$ 1,50) | 3 tarefas (-R$ 1,50) | R$ 0,00 |
| Domingo | Pagamento semanal | | **R$ 11,50** |

**Total da mesada na semana: R$ 11,50** 🎉

---

## 🎨 Interface (Inspiração)

...



---

## 🛠️ Tecnologias Utilizadas

| Camada | Tecnologia |
|--------|------------|
| **Frontend** | React + TypeScript |
| **Backend** | Node.js + Express |
| **Banco de Dados** | PostgreSQL / MongoDB |
| **Autenticação** | JWT (separando perfil criança/admin) |
| **Estilos** | CSS Modules / TailwindCSS |

---

## 📁 Estrutura do Projeto

...


---

## 🚀 Como Executar o Projeto

### Pré-requisitos
- Node.js (v18+)
- npm ou yarn
- PostgreSQL ou MongoDB

### Backend

cd backend
npm install
npm run dev


cd frontend
npm install
npm start


### 📝 Regras de Negócio

Regra	Descrição
✅ Conclusão	Tarefa concluída → soma o valor à mesada
❌ Não conclusão	Tarefa não concluída → subtrai o valor da mesada
📆 Periodicidade	Pai configura: semanal ou mensal
🔒 Permissões	Criança vê apenas tarefas e marcadores
👑 Admin	Pai tem acesso total (CRUD + configurações)

🎯 Próximas Funcionalidades (Roadmap)
Notificações (lembrete de tarefas)

Ranking entre irmãos

Metas extras e conquistas

Relatório mensal em PDF

Aplicativo mobile (React Native)

Suporte a múltiplas crianças por pai

🤝 Contribuição
Projeto em desenvolvimento. Sugestões são bem-vindas!

📄 Licença
MIT © Hugoleosilva