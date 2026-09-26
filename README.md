# Alinhafood Print Agent — instaladores

Este repositório guarda **só os instaladores** do Alinhafood Print Agent, o
programa que imprime as notinhas do [Alinhafood](https://alinhafood.com.br) nas
impressoras térmicas da loja. O código-fonte não fica aqui.

Os arquivos ficam em **[Releases](../../releases)**, um por versão:

| Sistema | Arquivo |
|---|---|
| Windows | `AlinhafoodPrintAgent-X.Y.Z-windows-Setup.exe` |
| macOS (Apple Silicon) | `AlinhafoodPrintAgent-X.Y.Z-mac-arm64.dmg` |
| macOS (Intel) | `AlinhafoodPrintAgent-X.Y.Z-mac-x64.dmg` |

## Para a loja

Instale pelo link do painel do Alinhafood, em **Impressora → Agente de
Impressão**. A partir da versão 1.11.0 o agente se atualiza sozinho: ele baixa
a versão nova daqui e confere o arquivo antes de instalar.

## Para quem publica

- **Nunca troque o arquivo de uma versão já publicada.** O painel guarda o
  SHA-256 de cada instalador; arquivo diferente com o mesmo nome faz todas as
  lojas baixarem e recusarem. Corrigiu algo? Versão nova.
- A tag é `vX.Y.Z` e os arquivos mantêm o nome que o build gerou.
- Publicar aqui não libera nada para as lojas. Quem decide quem recebe cada
  versão é a lista `AGENT_RELEASES` no painel; o roteiro completo está no
  CLAUDE.md do repositório do agente (seção "Atualização automática").
