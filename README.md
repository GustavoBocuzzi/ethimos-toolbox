# Ethimos Toolbox

Utilitários internos para Mesa RF e Mesa RV — gerador de tabela Oracle Symphony e e-mails de operação.

## Ferramentas

- **Tabela Oracle Symphony** — monta ordens (Ativo, C/V, Qtd, Preço, Conta, Validade) e copia no formato de tabela compatível com o Symphony
- **E-mail de Operação** — gera assunto + corpo para RV, RF Aplicação, RF Resgate, Swap e COE

## Estrutura

```
ethimos-toolbox/
├── index.html          # aplicação completa (single file, sem dependências)
└── .github/
    └── workflows/
        └── deploy.yml  # CI/CD para Azure Static Web Apps
```

## Deploy

Hospedado no Azure Static Web Apps. Push na branch `main` dispara deploy automático.

## Desenvolvimento local

Abrir `index.html` direto no navegador. Para que o botão Copiar funcione corretamente (ClipboardItem com text/html), servir via HTTP local:

```bash
npx serve .
```
