# Controle de Refeição — GONAR Engenharia

Sistema **offline** para controle de **refeições** (cafés e almoços) e **frequência** de funcionários em obras de engenharia civil. Tudo roda em um único arquivo HTML — sem instalação, sem servidor, sem internet — e exporta planilhas Excel já formatadas para enviar ao financeiro.

> Feito para o dia a dia de obra: rápido de lançar, fácil de exportar.

---

## ✨ Funcionalidades

- **Múltiplas obras** — cada obra guarda seus próprios períodos, equipe e preços.
- **Módulo de Refeições**
  - Períodos por intervalo de datas (gere uma quinzena ou um mês inteiro automaticamente).
  - Lançamento rápido: célula em branco, `Enter`/`↓` desce uma linha, e arraste o ponto para preencher **para cima ou para baixo** (como no Excel).
  - Totais automáticos (cafés, almoços, R$ café, R$ almoço e **Total a pagar**).
  - Exportação `.xlsx` formatada (bordas, dia da semana por extenso, valores em R$, logo no topo).
- **Módulo de Frequência**
  - Períodos por data (quinzenal ou mensal), com dias e dias da semana automáticos.
  - Equipe agrupada em Administração / Produção / Terceirizados.
  - Marcação de presença em um clique: `P`, `F`, `A`, `NP`, `FE`, `DE`.
  - Subtotais por grupo, resumo por função e assinatura no rodapé.
  - Exportação `.xlsx` formatada.
- **Logo da empresa** embutida (aparece no app e nas planilhas).
- **Backup / Restauração** dos dados em arquivo `.json`.
- **Interface premium** em tema escuro, responsiva (funciona no celular).

---

## 🚀 Como usar

1. Baixe o arquivo `index.html`.
2. Dê **dois cliques** — ele abre no navegador (Chrome, Edge, Firefox).
3. Pronto. Funciona **sem internet** e salva os dados no próprio navegador da máquina.

> Dica: clique com o botão direito em `index.html` → "Enviar para" → "Área de trabalho (criar atalho)" para abrir sempre rápido.

---

## 💾 Sobre os dados e backup

- Os dados ficam salvos **localmente no navegador** daquele computador (localStorage).
- Para levar os dados para outro PC ou guardar uma cópia de segurança, use **Backup** (gera um `.json`) e **Restaurar** no outro computador.
- Limpar os dados do navegador apaga os lançamentos — faça backup com frequência.

---

## 🛠️ Tecnologias

- HTML, CSS e JavaScript puros (arquivo único, alta performance).
- [ExcelJS](https://github.com/exceljs/exceljs) embutido para gerar os arquivos `.xlsx` formatados.
- Sem dependências externas em tempo de execução — 100% offline.

---

## 🌐 Publicar na web (opcional, GitHub Pages)

Se quiser acessar pelo navegador via link:

1. Crie um repositório no GitHub e suba estes arquivos.
2. No repositório: **Settings → Pages**.
3. Em **Source**, escolha a branch `main` e a pasta `/ (root)` e salve.
4. Em alguns minutos o sistema fica disponível em
   `https://SEU-USUARIO.github.io/controle-de-refeicao/`.

---

## 📦 Estrutura do projeto

```
controle-de-refeicao/
├── index.html      # o sistema completo (app + biblioteca embutida)
├── README.md       # este arquivo
├── LICENSE         # licença de uso
└── .gitignore      # arquivos ignorados pelo Git
```

---

## 📄 Licença

Distribuído sob a licença MIT. Veja o arquivo [LICENSE](LICENSE).

---

# Controle de Refeição — GONAR Engenharia (English)

**Offline** system for tracking employee **meals** (coffee/lunch) and **attendance** on civil engineering job sites. Runs entirely from a single HTML file — no install, no server, no internet — and exports formatted Excel spreadsheets ready to send to accounting.

## ✨ Features

Multiple job sites, each with its own periods, team, and prices. **Meals module:** date-range periods (auto-generate a fortnight or full month), spreadsheet-style fast entry (Enter/arrow to move down, drag-fill up or down), automatic totals, formatted `.xlsx` export. **Attendance module:** fortnightly/monthly periods with automatic weekdays, team grouped by Admin/Production/Contractors, one-click status marking (`P/F/A/NP/FE/DE`), group subtotals, formatted `.xlsx` export. Plus an embedded company logo, JSON backup/restore, and a responsive dark-theme UI.

## 🚀 Usage

Download `index.html` and double-click it — opens in any browser, works fully offline, and saves data in that machine's browser storage.

## 💾 Data & backup

Data is stored locally (`localStorage`). Use **Backup** to export a `.json` file and **Restore** to bring it into another computer — clearing browser data erases entries, so back up regularly.

## 🛠️ Tech stack

Plain HTML/CSS/JS (single file) with [ExcelJS](https://github.com/exceljs/exceljs) bundled in for `.xlsx` generation — no runtime dependencies, 100% offline.

## 📄 License

MIT — see [LICENSE](LICENSE).
