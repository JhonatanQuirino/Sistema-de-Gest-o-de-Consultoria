# 📅 Google Calendar para Google Sheets — Sistema de Gestão de Consultoria

Este projeto integra **Google Calendar** com **Google Sheets** via **Google Apps Script**, com o objetivo de automatizar o controle de tempo de consultorias, geração de relatórios por projeto e por setor.

---

## ⚙️ Funcionalidades

- ✅ Importar eventos do calendário do ano atual
- 📋 Organizar dados em uma aba `Detalhado` com:
  - Data
  - Hora Início / Fim
  - Duração (h)
  - Projeto (OS)
  - Descrição

- 📊 Gerar resumo por Projeto (OS), agrupando:
  - Datas trabalhadas
  - Descrições únicas
  - Total de horas

- 📈 Gerar relatório mensal de horas consumidas por setor

---

## 🧩 Scripts

| Arquivo | Função |
|--------|--------|
| `importarEventosAgenda.gs` | Importa todos os eventos da agenda para a aba `Detalhado` |
| `gerarResumoConsultoria.gs` | Gera a aba `Resumido` com agrupamento por OS |
| `gerarRelatorioPorSetorMensal.gs` | Gera a aba `Relatório por Setor` com total de horas por mês e setor |

---

## 🛠️ Como Usar

1. Crie uma planilha no Google Sheets com as abas:
   - `Detalhado` (com cabeçalho: Data, Hora Início, Hora Fim, Duração (h), Projeto (OS), Descrição)
2. No Google Apps Script da planilha, crie 3 arquivos `.gs` e cole os respectivos códigos de `scripts/`
3. Substitua a `calendarId` pela ID do seu Google Calendar
4. Execute o script `importarEventosAgenda` para popular os dados
5. Rode os demais scripts para gerar os relatórios

---

## 📎 Exemplo visual

![Exemplo da planilha](assets/exemplo-planilha.png)

---

## 🧠 Aprendizados

- Integração de APIs do Google Workspace
- Agrupamento e deduplicação de dados via JavaScript
- Automação de relatórios gerenciais com Apps Script

---

## 📌 Licença

MIT — sinta-se livre para usar, adaptar e compartilhar!

---

## 🙋‍♂️ Autor

Desenvolvido por [Jhonatan Quirino](https://www.linkedin.com/in/jhonatanquirino/) 🚀
