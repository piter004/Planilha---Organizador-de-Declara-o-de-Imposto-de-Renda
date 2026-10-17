#  Joker App - Organizador de Declaração de Imposto de Renda (IRPF)
##  Sobre o Projeto

O **Joker App** é uma planilha de controle e organização de dados para a **Declaração de Imposto de Renda Pessoa Física (IRPF)**, desenvolvida no Microsoft Excel.

Inspirado na identidade visual estilizada do jogo **Persona 5** (paleta de cores em vermelho, preto e branco com o ícone da máscara do Joker), o projeto combina um design marcante com uma navegação intuitiva em formato de aplicativo desktop.

---

##  Interface e Navegação

A interface principal conta com botões interativos para alternar entre as abas do formulário, mantendo o estado do botão ativo destacado em vermelho:

| Botão Titular Ativo | Botão Informes Ativo | Botão Notas Ativo |

---

##  Estrutura da Planilha

A planilha está dividida em **3 abas funcionais**:

### 1.  `TÍTULAR`
Área destinada aos dados pessoais e fiscais do contribuinte:
* Nome Completo, CPF e Data de Nascimento.
* **Título de Eleitor:** Formatado estritamente como texto para evitar a exibição em notação científica (`9.87654E+11`).
* Endereço, CEP, Contatos e Respostas Fiscais (Sim/Não).

### 2.  `INFORMES` (Rendimentos Bancários)
Consolidação do patrimônio e contas em instituições financeiras:
* **Lista de Seleção (Dropdown):** Integração com lista de bancos oficiais (C6 Bank, Santander, Itaú, etc.).
* **Cálculo Automático de Patrimônio:** Totalizador no topo com a fórmula:
  ```excel
  =SOMA(C20; C10; C15)
###  3.  `NOTAS` (Entradas / Holerites)
* **Registro detalhado das receitas e entradas financeiras ao longo do ano:**

* **Tabela de lançamentos por Data, Categoria (Holerite, CNPJ, Rendimentos) e Valor.**

* Totalizador acumulado das receitas recebidas.
