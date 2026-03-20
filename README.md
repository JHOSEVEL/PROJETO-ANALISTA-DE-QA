
# 🧪 Projeto de Portfólio QA OrangeHRM (Nível Basico)

## 📌 Visão Geral do Projeto

Este projeto demonstra um processo completo de QA aplicado a uma página de login real:

🔗 [https://opensource-demo.orangehrmlive.com/web/index.php/auth/login](https://opensource-demo.orangehrmlive.com/web/index.php/auth/login)

O objetivo é apresentar:

* Habilidades de teste manual
* Design de casos de teste
* Relatório de bugs (ficticios)

---

## 🎯 Escopo

Funcionalidade testada:

* Funcionalidade de Login

Fora do escopo:

* Recursos do Dashboard
* Gerenciamento de usuários

---

## 🧠 Estratégia de Teste

### Tipos de Teste Abrangidos

* Teste Funcional
* Teste Negativo
* Teste de UI/UX
* Teste de Segurança (básico)

---

## 🧪 Casos de Teste Manuais

### ✅ Cenários Positivos

| ID   | Descrição        | Passos                  | Resultado Esperado       |
| ---- | ------------------ | ---------------------- | --------------------- |
| TC01 | Login válido        | Inserir Admin/admin123   | Redirecionar para o dashboard |
| TC02 | Login após logout | Login → Logout → Login | Sucesso               |

### ❌ Cenários Negativos

| ID   | Descrição      | Resultado Esperado         |
| ---- | ---------------- | ----------------------- |
| TC03 | Usuário inválido | Mensagem de erro           |
| TC04 | Senha inválida | Mensagem de erro           |
| TC05 | Campos vazios     | Mensagem de validação      |
| TC06 | Apenas espaços      | Não deve permitir        |
| TC07 | Injeção SQL    | Não deve autenticar |

### ⚠️ Casos de Borda (Edge Cases)

* Nome de usuário com 1 caractere
* Nome de usuário com 255 caracteres
* Senha vazia
* Copiar/colar entradas

### 🎨 Testes de UI/UX

* Mascaramento de senha
* Habilitar/desabilitar botão
* Layout responsivo
* Clareza da mensagem de erro

### 🔐 Testes de Segurança

#### Injeção SQL

```
' OR 1=1 --
````

## 🐞 Exemplo de Relatório de Bug

**Título:** Login aceita espaços em branco

**Passos para Reproduzir:**

1. Abrir a página de login
2. Inserir "   " como nome de usuário
3. Inserir qualquer senha
4. Clicar em login

**Resultado Esperado:** Erro de validação

**Resultado Atual:** Tentativa de autenticação ocorre

**Severidade:** Média
**Prioridade:** Alta

---

## 🤖 Automação de Testes

### 🛠 Pilha de Tecnologia (Tech Stack)

* Python
  Dicionario com 5 exemplo de usuario e senha usando selenium

---

## 📊 Teste Orientado a Dados (users.csv)

```
username,password,expected
Admin,admin123,success
admin,wrong,fail
,admin123,fail
```

---

## 💼 Valor para o Portfólio

Este projeto demonstra:

* Fluxo de trabalho de QA real
* Habilidades de automação
* Pensamento analítico
* Consciência de segurança

---

## 👨‍💻 Autor

Josevel Alves Silva
Analista de Dados e Analista de QA Aspirante

---

## ⭐ Como se Destacar

* Adicionar capturas de tela da execução dos testes
* Gravar vídeo de demonstração
* Compartilhar no LinkedIn

---

## 📌 Licença

Este projeto é apenas para fins educacionais e de portfólio.
