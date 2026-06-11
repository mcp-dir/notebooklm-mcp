# NotebookLM

### NotebookLM para Claude, Cursor e agentes de IA

Google NotebookLM em linguagem natural: crie notebooks, adicione fontes (PDF, URL, YouTube) e faça perguntas com respostas fundamentadas + citações. NotebookLM não tem API oficial, conecte com 1 clique pela extensão do mcp.ai (captura os cookies da sua sessão Google; ficam criptografados na plataforma).

- 📊 **0 ferramentas**
- 🔒 **Somente leitura**
- 💬 **Funciona com qualquer cliente MCP**: Claude Desktop, Cursor, VS Code, Cline, Continue
- 🔑 **Login via magic-link (sem senha)**

[English version](README.en.md) · [Documentação completa](docs/) · [Skill pra agentes](skills/)

---

## Instalar em 1 clique

### Claude (Web e Desktop)

A Anthropic unificou a instalação de MCPs em `claude.ai/customize/connectors`. **O mesmo link serve pra Claude Web e Claude Desktop** (basta estar logado):

[➕ Abrir no Claude e conectar](https://claude.ai/customize/connectors?modal=add-custom-connector&mcpName=NotebookLM&mcpServerUrl=https%3A%2F%2Fapi.mcp.ai%2Fp_notebooklm)

**Manual** (se o deeplink não abrir): [claude.ai/customize/connectors](https://claude.ai/customize/connectors) → **+** → **Adicionar conector personalizado** → cole **Nome** `NotebookLM` e **URL** `https://api.mcp.ai/p_notebooklm`.

### Cursor

[➕ Instalar NotebookLM no Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=notebooklm&config=eyJ1cmwiOiJodHRwczovL2FwaS5tY3AuYWkvcF9ub3RlYm9va2xtIn0=)

### VS Code (Copilot Chat)

[➕ Instalar NotebookLM no VS Code](vscode:mcp/install?name=notebooklm&config=%7B%22type%22%3A%22http%22%2C%22url%22%3A%22https%3A%2F%2Fapi.mcp.ai%2Fp_notebooklm%22%7D)

### ChatGPT, Manus, OpenClaw e mais 40+ clientes

Funciona em qualquer cliente MCP que suporte **MCP over HTTP**. A URL do servidor é sempre:

```
https://api.mcp.ai/p_notebooklm
```

Detalhes por cliente: [INSTALL.md](INSTALL.md).

---

## Exemplos de uso

```
Liste meus notebooks do NotebookLM
Pergunte ao meu notebook: qual o resumo das fontes?
Adicione esta URL como fonte ao notebook
```

---

## 0 ferramentas disponíveis

| Tool | Descrição |
|---|---|


Detalhe de cada tool: [docs/ferramentas.md](docs/ferramentas.md)

---

## Preços

Grátis.

---

## Privacidade & LGPD

- **Somente leitura**, nenhuma ferramenta altera dados na origem.
- **Sub-processadores**: o LLM host que você escolher (Claude, ChatGPT, Cursor, agente próprio). Lista completa em [docs/privacidade-lgpd.md](docs/privacidade-lgpd.md).
- Os dados retornados pelas tools são enviados ao **LLM host que você escolher**, sub-processador fora do nosso controle. Recomendamos planos com opt-out de treinamento.

---

## Perguntas frequentes

**O servidor é open source?**
O servidor é proprietário (hosted). Este repositório é o wrapper público com manifestos, docs e skills — tudo MIT.

**Posso usar com agente próprio (não Claude/Cursor)?**
Sim — qualquer cliente que suporte MCP over HTTP. URL: `https://api.mcp.ai/p_notebooklm`.


---

## Suporte

- 📧 [notebooklm@mcp.ai](mailto:notebooklm@mcp.ai)
- 🐛 [GitHub Issues](https://github.com/mcp-dir/notebooklm-mcp/issues)
- 📄 [docs/](docs/)

---

## Licença

MIT — veja [LICENSE](LICENSE). O servidor MCP em `api.mcp.ai/p_notebooklm` é proprietário (hosted); este repositório (manifestos, docs, skills) é MIT.
