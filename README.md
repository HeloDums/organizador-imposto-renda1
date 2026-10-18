# 🧾 Organizador de Declaração de Imposto de Renda (Excel)

Planilha em Excel que centraliza e organiza as informações necessárias para a declaração anual de Imposto de Renda (IRPF). Foi construída com **menu de navegação**, **validações de dados**, **fórmulas automáticas** e **links rápidos**, para que o preenchimento seja prático, padronizado e livre de erros de digitação.

> Projeto desenvolvido como desafio da DIO: *Criando um Organizador de Declaração de Imposto de Renda*.

---

## 🎯 Objetivo

Reunir em um único arquivo tudo o que costuma ser necessário na hora de declarar: dados pessoais, rendimentos, despesas dedutíveis, bens e direitos, dívidas e documentos. Assim, quando chega a época da declaração, as informações já estão organizadas e conferidas.

## 🗂️ Estrutura da planilha

| Aba | Para que serve |
|---|---|
| **Menu** | Página inicial com navegação por hiperlinks, links rápidos (Receita Federal, e-CAC, gov.br) e instruções de uso |
| **Resumo** | Painel com totais calculados automaticamente (rendimentos, despesas, patrimônio, progresso do checklist) |
| **Dados Pessoais** | Cadastro do contribuinte e dos dependentes |
| **Rendimentos** | Lançamento das fontes pagadoras, valores brutos e IR retido |
| **Despesas** | Despesas dedutíveis (saúde, educação, previdência etc.) com controle de comprovantes |
| **Bens e Direitos** | Imóveis, veículos, contas e investimentos, com variação entre os anos |
| **Dívidas** | Financiamentos, empréstimos e ônus |
| **Checklist** | Lista de documentos com status (Pendente / Em andamento / Entregue) |
| **Listas** | Listas de apoio que alimentam os menus suspensos |

## ⚙️ Recursos utilizados

- **Validação de dados**
  - Listas suspensas (tipo de rendimento, categoria de despesa, grupo de bem, UF, estado civil, status etc.)
  - Validação de **CPF/CNPJ** (somente números, 11 ou 14 dígitos)
  - Validação de **datas**, **valores monetários** (não negativos), **ano-calendário** e **e-mail**
  - Mensagens de entrada e de erro personalizadas
- **Navegação com `HYPERLINK`**: botões do menu levam para cada aba e todas as abas têm o botão "Voltar ao Menu"
- **Fórmulas**: `SOMA`, `SOMASE`, `CONT.SE`, `CONT.VALORES`, `SE`, `SEERRO`, `MÍNIMO` e referências entre abas
- **Formatação condicional**: status do checklist coloridos e destaque para despesas sem comprovante
- **Organização visual**: células de entrada em amarelo (texto azul), células calculadas em cinza, painéis congelados e cores por aba

## 🚀 Como usar

1. Abra o arquivo `Organizador_IR.xlsx` no Excel.
2. Comece pela aba **Menu** e vá em **Dados Pessoais**.
3. Preencha apenas as **células amarelas** (texto azul). As cinzas são fórmulas.
4. A **linha 6** de cada aba é um **exemplo**: substitua ou apague.
5. Acompanhe os totais na aba **Resumo** e o andamento na aba **Checklist**.
6. Confira os parâmetros de limites (educação e dependentes) na aba **Resumo**, pois são valores de referência que mudam conforme o ano.

## 📸 Capturas de tela

![Menu](images/menu.png)
![Resumo](images/resumo.png)

## 🧠 Aprendizados

- Como estruturar uma planilha como um pequeno "sistema", separando entradas, cálculos e listas de apoio
- Uso de validação de dados para garantir a qualidade das informações na origem
- Criação de navegação interna com `HYPERLINK`
- Documentação técnica em Markdown e publicação no GitHub

## ⚠️ Aviso

Esta é uma ferramenta de **organização pessoal**. Ela não substitui o programa oficial da Receita Federal nem orientação de um contador. Os valores de limites e deduções são referências e devem ser conferidos nas regras vigentes de cada ano.

## 📁 Arquivos do repositório

```
├── README.md
├── Organizador_IR.xlsx
└── images/
    ├── menu.png
    └── resumo.png
```
