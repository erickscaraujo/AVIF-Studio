# 🖼️ AVIF Studio

![Versão](https://img.shields.io/badge/versão-1.0.0-blue)
![Windows](https://img.shields.io/badge/Windows-10%2F11%2064--bit-0078D4?logo=windows&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-1.70%2B-orange?logo=rust&logoColor=white)
![Licença](https://img.shields.io/badge/licença-MIT-green)
![Offline](https://img.shields.io/badge/100%25-offline-success)
![Idioma](https://img.shields.io/badge/idioma-pt--BR-yellowgreen)

**Conversor profissional de imagens em lote para AVIF — rápido, seguro e 100% offline.**

Desenvolvido por **Erick de S.C. Araújo.**

O AVIF Studio converte imagens individuais ou milhares de arquivos de uma só vez para o formato `.avif`, com compressão eficiente, interface moderna em português do Brasil, estatísticas em tempo real e distribuição portátil + instalador para Windows 10 e 11 (64-bit).

---

## ✨ Destaques

- 🗂️ **Lote de verdade** — varredura recursiva, drag-and-drop de arquivos e pastas, milhares de imagens sem travar a interface.
- ⚡ **Paralelo por padrão** — metade dos threads lógicos (`máx(1, lógicos/2)`), com modos econômico/equilibrado/máximo/personalizado.
- 🎚️ **Controle AVIF** — qualidade 0–100, velocidade 1–10, modo sem-perdas explícito, preservação de transparência.
- 📊 **Estatísticas ao vivo** — convertidas, economia absoluta/percentual (inclusive negativa), médias, ETA.
- 🛡️ **Seguro** — gravação transacional validada, originais preservados por padrão, erros isolados por arquivo.
- 📦 **Offline e portátil** — zero DLLs externas, zero instalação, zero rede.

## 📥 Instalação

| Opção | Arquivo | Descrição |
|---|---|---|
| Instalador | `AVIF-Studio-Setup-1.0.0.exe` | Inno Setup 6. Suporta `/SILENT` e `/VERYSILENT`. |

## 🚀 Uso rápido

1. Adicione imagens, selecione pastas ou **arraste arquivos/pastas** para a janela.
2. Ajuste qualidade, velocidade e destino no painel lateral.
3. Clique em **▶ Iniciar conversão** — acompanhe progresso, estatísticas e erros.
4. Use **🔁 Tentar falhas** para repetir só o que falhou.

## 🗂️ Formatos

| Extensão | Status |
|---|---|
| `.jpg` `.jpeg` `.jfif` | ✅ Suportado (JPEG) |
| `.png` | ✅ Suportado (alfa preservado) |
| `.tif` `.tiff` | ✅ Suportado (1ª página) |
| `.webp` | ✅ Suportado (alfa preservado) |
| `.heic` `.jng` `.jp2` `.ps` `.raw` | ⛔ Reconhecido, erro específico por arquivo (sem decodificador incluído — ver `docs/DECISOES.md`) |

A extensão nunca é prova de validade: o conteúdo é verificado na decodificação.

Pacote portátil + checksums: `scripts/build-release.ps1`.
Instalador: compile `installer/avif-studio.iss` com o Inno Setup 6.

Detalhes de arquitetura e decisões em [`docs/DECISOES.md`](docs/DECISOES.md).

## 🗺️ Roteiro

- [ ] Decodificação HEIC (libheif) e JPEG 2000 como suplemento opcional.
- [ ] Preservação seletiva de EXIF/ICC/XMP.
- [ ] Pré-visualização lado a lado com estimativa de tamanho.
- [ ] Associação opcional de extensões no instalador.

## 📄 Licença

MIT — ver [`LICENSE`](LICENSE). Avisos de terceiros em [`THIRD_PARTY_NOTICES.md`](THIRD_PARTY_NOTICES.md) e `resources/licenses/`.

---

<p align="center"><b>AVIF Studio</b> — Conversor profissional de imagens.<br>Desenvolvido por <b>Erick de S.C. Araújo.</b></p>
