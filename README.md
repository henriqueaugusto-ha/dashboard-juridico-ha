# ⚖️ Dashboard Jurídico — H.A. Advocacia

Dashboard visual de gestão da **Central do Cliente** do escritório H.A. Advocacia Especializada em Trânsito.

🔗 **Visualize ao vivo:** [dashboard.henriqueaugusto.adv.br](https://dashboard.henriqueaugusto.adv.br/)

---

## 📊 O que o dashboard mostra

- **6 abas navegáveis**: Administrativo, Judicial, Prazos Abertos, Prazos Atrasados, Produzidos vs A Produzir, Visão Geral Mensal
- **Espécies de ação detalhadas** (Lei Seca, Sem Capacete, Manobra Perigosa, Anulatória PSDD, Transf. Pontos, Mandado de Segurança, etc.)
- **Barras empilhadas por etapa** processual (DP → JARI → CETRAN → Vitória para administrativos; Confecção → Protocolo → Liminar → Sentença → Cumprimento para judiciais)
- **Filtro por espécie** com clique nos cards
- **Botão de exportação CSV/XLSX**
- **Responsivo** (mobile-friendly 320px+)

---

## 🛠️ Como funciona

- Site **estático** (single-file HTML, ~90 KB)
- **Funciona offline** após carregar
- **Dados embutidos** no momento da geração (snapshot do ClickUp)
- **Sem dependências externas** (sem CDN, sem APIs em runtime)
- **Hospedado em GitHub Pages** com domínio personalizado

---

## 🔄 Atualizações

O dashboard é atualizado **sob demanda** pelo Dr. Henrique Augusto, executando o agente Claude que:

1. Lê todas as listas da Central do Cliente no ClickUp via MCP
2. Cruza com a Planilha 3 (Processos Judiciais)
3. Aplica as regras de normalização (espécies, órgãos, etapas)
4. Regenera o `index.html` com os dados atualizados
5. Faz commit neste repositório
6. GitHub Pages publica automaticamente (~1 min)

---

## 📁 Estrutura

```
dashboard-juridico-ha/
├── index.html           ← Dashboard (arquivo único, ~90 KB)
├── CNAME                ← Configuração do domínio personalizado
└── README.md            ← Este arquivo
```

---

## 🔐 Privacidade

O dashboard contém **nomes de clientes** e **espécies de ação contratadas**. Apesar de o repositório ser público para usar GitHub Pages gratuito, recomenda-se:

- **Não divulgar a URL** publicamente (compartilhar apenas com equipe interna)
- Considerar migrar para repositório **privado** (requer GitHub Pro — US$ 4/mês)
- Não inclui CPF, RG, telefones, valores, endereços ou dados sensíveis

---

## 📝 Histórico de Versões

| Versão | Data | Mudanças |
|---|---|---|
| v1 | Maio/2026 | Dashboard inicial — 2 abas (ADM + Judicial) |
| v2 | 14/05/2026 | 6 abas + apuração Dez/25→Mai/26 |
| v3 | 14/05/2026 | + Espécies de ação (cards + barras empilhadas) + filtros + domínio personalizado |

---

## 📞 Contato

Dr. Henrique Augusto Félix Linhares
H.A. Advocacia Especializada em Trânsito
[henriqueaugusto.adv.br](https://henriqueaugusto.adv.br/)
