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
