<div align="center">

# Olá, sou o Iago Beserra 👋

Desenvolvedor focado em **backend, segurança defensiva e automação**.
Construo desde serviços Windows de baixo nível até plataformas web completas.

[![Portfolio](https://img.shields.io/badge/Portfolio-1f9d55?style=for-the-badge&logo=googlechrome&logoColor=white)](https://iag0bezz.github.io/iag0bezz/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-1f9d55?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/iago-beserra-71747317a/)
[![Gmail](https://img.shields.io/badge/Gmail-1f9d55?style=for-the-badge&logo=gmail&logoColor=white)](mailto:iago.beserra1@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-1f9d55?style=for-the-badge&logo=github&logoColor=white)](https://github.com/iag0bezz)
[![Curriculo](https://img.shields.io/badge/Curriculo-1f9d55?style=for-the-badge&logo=readdotcv&logoColor=white)](https://iag0bezz.github.io/iag0bezz/curriculo-iago-beserra.pdf)

![Followers](https://img.shields.io/github/followers/iag0bezz?label=followers&style=for-the-badge&color=1f9d55&labelColor=161a18)

</div>

## Projetos em destaque

### [AntiGrabber](https://github.com/iag0bezz/Anti-Grabber)

![C#](https://img.shields.io/github/languages/top/iag0bezz/Anti-Grabber?style=flat-square&color=1f9d55&label=C%23)
![License](https://img.shields.io/github/license/iag0bezz/Anti-Grabber?style=flat-square&color=1f9d55)
![Stars](https://img.shields.io/github/stars/iag0bezz/Anti-Grabber?style=flat-square&color=1f9d55)

Serviço Windows de segurança defensiva contra **grabbers**, malware que rouba
token de sessão do Discord, credenciais da Steam e dados de outros apps. A
detecção é 100% baseada em metadado e comportamento: qual processo abriu qual
conexão, para qual domínio, usando o [WinDivert](https://reqrypt.org/windivert.html),
sem MITM e sem telemetria. Roda 100% offline, sem login, sem conta e sem nuvem.

Stack: **C# / .NET 8**, serviço Windows (`AntiGrabberService`) mais tray nativo
(host WinForms com **WebView2**, renderizando a UI em HTML/Alpine.js embutido,
sem Electron nem runtime Node em produção) e notificações toast nativas do
Windows. Instalador único via Inno Setup, com releases automáticos pelo
GitHub Actions a cada tag.

### Rexie Auth

![Node.js](https://img.shields.io/badge/Node.js-1f9d55?style=flat-square)
![Status](https://img.shields.io/badge/repo-privado-eceeed?style=flat-square&color=5f6864)

Plataforma completa de venda e licenciamento de scripts para servidores
FiveM. Monorepo Node.js com três apps (`apps/api`, `apps/bot`, `apps/web`),
banco MariaDB e deploy via Docker e PM2.

Funcionalidades: loja com catálogo de produtos e pacotes, carrinho, cupom de
desconto e checkout via Pix (gateway Efí); central de documentação com
busca por produto; avaliações e changelog de cada produto; licenciamento com
reset de HWID e parcelamento; painel admin completo (produtos, pedidos,
cupons, avaliações, pacotes, clientes, licenças, backup e logs); campanhas de
broadcast para clientes no Discord; e um bot Discord com comandos próprios
para criar, listar, consultar e gerenciar licença direto no servidor. A API
expõe validação, heartbeat e checagem de atualização para o script consumir
em tempo de execução, além de jobs recorrentes para expiração de pedido,
retenção de log, backup, licença perto de vencer e lembrete de parcela.

### Skylla, SaaS de gestão para restaurantes

![TypeScript](https://img.shields.io/badge/TypeScript-1f9d55?style=flat-square)
![Status](https://img.shields.io/badge/repo-privado-eceeed?style=flat-square&color=5f6864)

Plataforma multi-tenant para gestão de restaurante, do pedido ao financeiro.
Monorepo com API (**Fastify 5 + Prisma + PostgreSQL**) e app web
(**Next.js 15 + React 19**). Cobre autenticação (JWT + RBAC), produtos com
upload de imagem (MinIO/S3), pedidos com baixa automática de estoque e
financeiro, estoque com ficha técnica e conversão de unidades, compras com
recebimento parcial e rateio de frete, financeiro com CMV e fluxo de caixa,
inventário físico, auditoria e um módulo de inteligência que gera previsão de
reabastecimento e insights, com regras de negócio isoladas da camada HTTP.

## Stack

<div>
  <img align="center" alt="C#" height="32" width="32" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg">
  <img align="center" alt=".NET" height="32" width="32" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/dotnetcore/dotnetcore-original.svg">
  <img align="center" alt="TypeScript" height="32" width="32" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-plain.svg">
  <img align="center" alt="JavaScript" height="32" width="32" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
  <img align="center" alt="Node.js" height="32" width="32" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original.svg">
  <img align="center" alt="React" height="32" width="32" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg">
  <img align="center" alt="Next.js" height="32" width="32" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nextjs/nextjs-original.svg">
  <img align="center" alt="Docker" height="32" width="32" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original.svg">
  <img align="center" alt="PostgreSQL" height="32" width="32" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original.svg">
  <img align="center" alt="MySQL" height="32" width="32" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original.svg">
</div>

<sub>Backend: C#/.NET, Node.js/TypeScript, Fastify, Prisma. Frontend: React, Next.js. Infra: Docker, WebView2, WinDivert.</sub>
