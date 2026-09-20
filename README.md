<p align="center">
  <img src="assets/logo.png" alt="Marca Pessoal" width="180">
</p>

<h1 align="center">Empacotamento Debian</h1>

<p align="center">
  <a href="https://www.debian.org/"><img src="https://img.shields.io/badge/Debian-D70A53?style=for-the-badge&logo=debian&logoColor=white" alt="Debian"></a>
  <a href="https://www.kernel.org/"><img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux"></a>
  <a href="https://www.gnu.org/software/bash/"><img src="https://img.shields.io/badge/Shell_Script-121011?style=for-the-badge&logo=gnu-bash&logoColor=white" alt="Shell Script"></a>
</p>

# Empacotamento Debian 

[![Debian](https://img.shields.io/badge/Debian-D70A53?style=for-the-badge&logo=debian&logoColor=white)](https://www.debian.org/)
[![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://www.kernel.org/)
[![Shell Script](https://img.shields.io/badge/Shell_Script-121011?style=for-the-badge&logo=gnu-bash&logoColor=white)](https://www.gnu.org/software/bash/)

Repositório dedicado ao estudo, desenvolvimento e manutenção de pacotes no ecossistema **Debian**. Este espaço é utilizado para realização de testes de empacotamento, resolução de bugs, análise de dependências e documentação de fluxos de trabalho segundo as diretrizes das políticas Debian (*Debian Policy Manual*).

---

##  Objetivos do Repositório

-  **Empacotamento de Software:** Criação e manutenção de arquivos e receitas de build (`debian/control`, `debian/rules`, `debian/copyright`, etc.).
-  **Correção de Bugs:** Diagnóstico, depuração e aplicação de *patches* em pacotes existentes.
-  **Laboratório de Testes:** Ambientes isolados para compilação e verificação de integridade de pacotes (`pbuilder`, `sbuild`, `lintian`).
-  **Documentação:** Anotações técnicas e guias práticos sobre ferramentas e boas práticas da comunidade Debian.

---

##  Ferramentas e Tecnologias

As principais ferramentas utilizadas nos fluxos deste repositório incluem:

| Ferramenta | Finalidade |
| :--- | :--- |
| `dpkg-dev` / `debuild` | Ferramentas essenciais para compilação e construção do pacote |
| `dh-make` / `debhelper` | Automação e padronização dos scripts de compilação |
| `lintian` | Análise estática e verificação de conformidade com as regras do Debian |
| `quilt` | Gerenciamento de *patches* no código-fonte original (*upstream*) |
| `pbuilder` / `sbuild` | Compilação em ambientes limpos de chroot |

---

##  Estrutura do Repositório

```text
.
├── packages/           # Diretório contendo os fontes e arquivos de empacotamento
├── tests/              # Scripts e rotinas de validação automatizada
├── docs/               # Guias, anotações de estudo e referências técnicas
└── README.md           # Documentação principal do repositório
