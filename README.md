# 🚀 Modelo institucional municipal

> Modelo de portal institucional estático para prefeituras. Reúne serviços, notícias, informações públicas e canais de atendimento em uma interface que pode ser adaptada para diferentes municípios.

![Status](https://img.shields.io/badge/status-em_desenvolvimento-green.svg)
![Version](https://img.shields.io/badge/version-1.0.0-orange.svg)
![License](https://img.shields.io/badge/license-n%C3%A3o_especificada-lightgrey.svg)

---

## 📌 Índice

- [Visão Geral](#-visão-geral)
- [Tecnologias](#-tecnologias)
- [Como Executar](#-como-executar)
- [Como Contribuir](#-como-contribuir)
- [Licença](#-licença)

---

## 💡 Visão Geral

O projeto oferece uma base reutilizável para apresentar informações e serviços municipais em um só lugar. As páginas são geradas como arquivos estáticos pelo Astro, sem enviar um framework JavaScript ao navegador; o menu móvel usa apenas um pequeno script.

- ✨ **Serviços municipais:** atalhos para serviços mais acessados e uma página dedicada.
- 📰 **Informação pública:** áreas para notícias, transparência, informações da prefeitura e contato.
- 🎨 **Personalização:** configure identidade visual e dados do município sem alterar o layout compartilhado.
- 📱 **Interface responsiva:** navegação adaptada para dispositivos móveis e telas maiores.

> O município, contatos, serviços e notícias que acompanham o projeto são exemplos. Substitua-os por informações oficiais antes da publicação.

---

## 🛠️ Tecnologias

![Astro](https://img.shields.io/badge/Astro-BC52EE?style=for-the-badge&logo=astro&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-663399?style=for-the-badge&logo=css&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)

---

## 🚀 Como Executar

### Pré-requisitos

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/) 22.23.4 ou superior
- npm

### 🔧 Passo a passo

```bash
# 1. Clone o repositório
git clone https://github.com/elielreinan/modelo-institucional.git

# 2. Acesse a pasta do projeto
cd modelo-institucional

# 3. Instale as dependências
npm ci

# 4. Inicie o servidor de desenvolvimento
npm run dev
```

Para validar e gerar a versão estática:

```bash
npm run build
npm run preview
```

O build gera os arquivos em `dist/`. Publique essa pasta em uma hospedagem estática e configure o provedor para usar `404.html` nas rotas inexistentes.

### Personalizar para outro município

- Edite `src/config/client.ts` para configurar nome, contatos, endereço, brasão, imagem e cores.
- Atualize `src/data.ts` com os serviços e notícias oficiais.
- Conecte os atalhos de transparência e serviços aos portais oficiais antes de publicar.
- As páginas públicas ficam em `src/pages/`; o layout compartilhado e os componentes reutilizáveis ficam em `src/layouts/` e `src/components/`.
- Ajuste `astro.config.mjs` se for publicar em outro domínio ou caminho base.

---

## 🤝 Como Contribuir

Contribuições são bem-vindas. Abra uma issue para relatar problemas ou sugerir melhorias e envie um pull request com alterações focadas. Antes de propor conteúdo municipal, confirme que os dados e links são oficiais.

---

## 📄 Licença

Este repositório não declara uma licença de uso. Consulte o responsável pelo projeto antes de reutilizar ou distribuir o código.
