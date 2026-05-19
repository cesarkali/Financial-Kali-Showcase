<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=slice&color=ff0000&height=200&section=header&text=Financial%20Kali&fontSize=80&fontAlignY=35&animation=twinkling&desc=SaaS%20de%20Gestão%20Financeira%20com%20IA%20Preditiva&descAlignY=55&descAlign=50&fontColor=ffffff&reversal=true"/>
</div>

<div align="center">
  <a href="https://caliberda.com.br/kali" target="_blank">
    <img src="https://img.shields.io/badge/Acessar_Plataforma-ff0000?style=for-the-badge&logo=vercel&logoColor=black" alt="Acessar Plataforma">
  </a>
</div>

<br>

> 🔒 **Nota Executiva de Arquitetura:** O código-fonte deste SaaS é **privado** por envolver propriedade intelectual, integrações comerciais proprietárias de IA e arquitetura Multi-Tenant de dados sensíveis. Este repositório atua como uma vitrine arquitetural e de engenharia de produto. 

---

## 💎 Visão do Produto

**Financial Kali v3.0** é um ecossistema B2B/B2C de gestão financeira e patrimonial de alta performance. Projetado com uma estética "Obsidian Dark" voltada para redução de fadiga visual (Frictionless UX), o sistema entrega visibilidade total, conciliação em massa e privacidade absoluta sobre o fluxo de caixa.

A plataforma opera de forma híbrida e ininterrupta através de um **Web App (React 19)** e um **App Android Nativo (React Native)**, garantindo sincronização em tempo real.

---

## 🚀 Funcionalidades Core (Product Highlights)

### 🤖 Finn IA Preditiva (Native Voice & Vision)
O núcleo de inteligência do sistema foi desenhado para processamento ultrarrápido sem toque na tela:
* **Finn Voice:** Integração ponta-a-ponta com Groq Whisper-large-v3 para transcrição e categorização instantânea via comando de voz.
* **Finn Vision:** Sistema de OCR e filtro de foco que rejeita automaticamente anexos sem relevância financeira.
* **Contexto Isolado:** Histórico de inferência individualizado por sessão, impossibilitando vazamento de contexto entre conversas.

### 🏢 Arquitetura Multi-Tenant (Multi-Empresa)
Projetado para usuários que operam múltiplos negócios simultaneamente:
* **Isolamento de Banco de Dados:** Contas Pessoais, Empresariais e de Projetos rodam em clusters totalmente segregados.
* **Identidade Dinâmica:** O sistema adapta o UI e renderiza logos (via base64) de acordo com a empresa selecionada ou o domínio da conta bancária.
* **Replicação Estrutural:** Transferência de categorias e regras de negócio entre bases com um único clique.

### 🔒 Segurança & Stealth Ops
* **Modo Sigilo (Stealth):** Ocultação em um clique de todos os valores e gráficos sensíveis para operação em ambientes públicos.
* **Google Identity Sync:** Autenticação avançada e gestão de sessão com Firebase Auth.
* **Cleanup Recursivo:** Engenharia de banco de dados que garante exclusão em cascata (definitiva) ao encerrar uma conta, atendendo aos mais altos padrões de LGPD.

---

## 🛠️ Stack Tecnológica & Engenharia

A arquitetura foi escolhida para garantir **Tempo de Resposta < 200ms**, escalabilidade em nuvem e fluidez nativa mobile.

| Camada | Tecnologia Principal | Descrição Técnica |
| :--- | :--- | :--- |
| **Front-end Web** | React 19 + Vite 8 | UI componentizada, Tailwind CSS e Lucide Icons. |
| **Mobile Nativo** | React Native + Expo | SDK 54, UI 100% nativa sem WebViews, animações de 60fps via Animated API. |
| **Back-end & DB** | Firebase Firestore | NoSQL Serverless com listeners em tempo real e regras de segurança estruturais. |
| **Inteligência Artificial** | Groq + Gemini | Llama 3.3 70B e Gemini 1.5 Flash operando via Resilient Key Rotation (alta disponibilidade). |
| **CI/CD & DevOps** | GitHub Actions + EAS | Pipelines automatizados com injeção de changelog no banco de dados e builds OTA (Over-The-Air) para Android. |

---

<div align="center">
  <p class="text-zinc-500">
    <i>Desenvolvido por Júlio Caliberda.</i><br>
    <i>Arquiteturas Resolutivas para Problemas Complexos.</i>
  </p>
</div>
