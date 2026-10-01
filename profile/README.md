<div align="center">

<img src="https://www.temperopdv.com.br/brand/tempero-icone-app.svg" alt="Tempero PDV" width="104" />

# Tempero PDV

**PDV e gestão para restaurantes, bares e cafés.** Do salão à cozinha, do caixa ao financeiro, com a equipe toda no celular
e o restaurante funcionando mesmo quando a internet cai.

[![Site](https://img.shields.io/badge/site-temperopdv.com.br-142220?style=for-the-badge)](https://www.temperopdv.com.br)
[![Planos](https://img.shields.io/badge/7_dias_grátis-nível_Pro-4f7872?style=for-the-badge)](https://www.temperopdv.com.br/planos)
[![Downloads](https://img.shields.io/badge/downloads-Windows_·_macOS_·_Linux_·_Android-ecd48d?style=for-the-badge&labelColor=142220)](https://github.com/Tempero-PDV/tempero-pdv-downloads/releases)

</div>

---

### O que o Tempero PDV faz

| No salão | Na produção | Na gestão |
|---|---|---|
| Mesas em planta 2D e 3D, comandas, conta por pessoa, gorjeta e PIX | Cozinha e bar com tela (KDS) e impressora própria por setor | Caixa, financeiro, DRE, relatórios e indicadores do dia |
| App do garçom no Android e no iPhone, cardápio digital com QR | Tempo de preparo por prato e por época do ano, alerta de alergia | Divisão dos 10% pela escala, folha da equipe e consumo |
| Reservas e clientes (CRM) | Placa ESP32 que liga a térmica no Wi-Fi, sem computador | NFC-e, impostos do Simples, pacote do contador |
| Funciona sem internet: central local e fila que sincroniza depois | Via só com os itens novos, cancelamento impresso | Rede de unidades, marca própria, API e trilha de auditoria |

### Repositórios

| Repositório | O que tem |
|---|---|
| [tempero-pdv-sistema](https://github.com/Tempero-PDV/tempero-pdv-sistema) | O sistema completo: site, painel, consoles, API, apps e firmware |
| [tempero-pdv-site](https://github.com/Tempero-PDV/tempero-pdv-site) | Site público, blog, ajuda com mais de 1.300 respostas, carreiras e SEO |
| [tempero-pdv-apps](https://github.com/Tempero-PDV/tempero-pdv-apps) | Apps de garçom, balcão, caixa, cozinheiro e barman: Android, web/PWA e desktop |
| [tempero-pdv-equipamentos](https://github.com/Tempero-PDV/tempero-pdv-equipamentos) | Impressoras térmicas, firmware ESP32, agente de impressão e Tempero OS |
| [tempero-pdv-bot-telegram](https://github.com/Tempero-PDV/tempero-pdv-bot-telegram) | Bot do dono com mais de 700 comandos, login com TOTP e automações |
| [tempero-pdv-suporte](https://github.com/Tempero-PDV/tempero-pdv-suporte) | Central de suporte e o app desktop Tempero Suporte |
| [tempero-pdv-remoto](https://github.com/Tempero-PDV/tempero-pdv-remoto) | Acesso remoto próprio (WebRTC com TURN) e o app Tempero Remoto |
| [tempero-pdv-chat](https://github.com/Tempero-PDV/tempero-pdv-chat) | Chat da equipe: Android, web e desktop |
| [tempero-pdv-tarefas](https://github.com/Tempero-PDV/tempero-pdv-tarefas) | Tarefas no padrão do Asana: projetos, sprints, horas e metas |
| [tempero-pdv-agentes](https://github.com/Tempero-PDV/tempero-pdv-agentes) | Agentes de IA com ferramentas, aprovação e o escritório 3D |
| [tempero-pdv-downloads](https://github.com/Tempero-PDV/tempero-pdv-downloads) | Instaladores públicos (a versão mais nova de cada produto) |

Os repositórios de código são privados e recebem uma cópia automática do repositório principal a cada mudança.

### Onde roda

```
 restaurante                       nuvem                                  apoio
 ───────────                       ─────                                  ─────
 celular do garçom ─┐        ┌─ Next.js 15 na Vercel (site, painel,   ┌─ N8N: avisos, resumo, backup
 computador do caixa ┼─ HTTPS ┤   consoles e API, funções em iad1)    ├─ backup cifrado (AES-256-GCM)
 tela da cozinha ────┤        ├─ Supabase: Postgres, login, arquivos   ├─ TURN do acesso remoto
 placa ESP32 ────────┘        ├─ Stripe: assinaturas                   └─ Chatwoot
   └─ central local (LAN)     └─ Upstash Redis: limites e presença
      sem internet
```

### Apps

| App | Sistemas |
|---|---|
| Tempero PDV Desktop (caixa, cozinha, bar) | Windows · macOS · Linux · Arch |
| App do salão | Android · iPhone (PWA) · qualquer navegador |
| Tempero Suporte | Windows · macOS · Linux · Arch |
| Tempero Remoto | Windows · macOS · Linux · Arch |
| Tempero Chat | Windows · macOS · Linux · Arch · Android · web |
| Placa da cozinha | ESP32 e ESP32-S3 |

### Stack

![Next.js](https://img.shields.io/badge/Next.js_15-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React_19-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white)
![Electron](https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)
![Espressif](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

### Segurança e privacidade

Segredos só no servidor · permissão por cargo em toda rota · 2FA · defesa por IP · backup diário cifrado fora da nuvem
principal · LGPD com canal para titulares e encarregado · varredura de segredos e dependências a cada push.

### Contato

[www.temperopdv.com.br](https://www.temperopdv.com.br) · [Fale com a gente](https://www.temperopdv.com.br/contato) · [Carreiras](https://www.temperopdv.com.br/carreiras)

<sub>© Estevam Souza · Tempero PDV</sub>
