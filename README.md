<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=slice&color=0:1a0000,100:ff0000&height=200&section=header&text=Financial%20Kali&fontSize=72&fontAlignY=35&desc=Gest%C3%A3o%20financeira%20com%20IA%2C%20na%20web%20e%20no%20Android&descSize=18&descAlignY=58&fontColor=ffffff&reversal=true" alt="Financial Kali"/>

  <a href="https://www.caliberda.com.br/kali"><img src="https://img.shields.io/badge/Acessar_a_plataforma-ff0000?style=for-the-badge&logo=vercel&logoColor=white" alt="Acessar a plataforma"></a>

  ![Versão](https://img.shields.io/badge/vers%C3%A3o-4.1.0-ff0000?style=flat-square)
  ![Plataformas](https://img.shields.io/badge/plataformas-Web%20%C2%B7%20Android-1f1f1f?style=flat-square)
  ![React](https://img.shields.io/badge/React-19-1f1f1f?style=flat-square&logo=react)
  ![React Native](https://img.shields.io/badge/React%20Native-0.81%20%C2%B7%20Expo%2054-1f1f1f?style=flat-square&logo=expo)
  ![Firebase](https://img.shields.io/badge/Firebase-Firestore%20%C2%B7%20Auth-1f1f1f?style=flat-square&logo=firebase)
</div>

> 🔒 **Código privado.** O Financial Kali lida com dados financeiros de pessoas e empresas, então o código-fonte não é público. Este repositório é a vitrine do produto: o que ele faz, como foi construído e as decisões de engenharia por trás.

---

## 💎 O produto

O **Financial Kali** é um sistema de gestão financeira pessoal e empresarial com um assistente de IA, o **Finn**, que entende voz, texto e imagens. Funciona no navegador e num **app Android nativo**, com os dados sincronizados em tempo real entre os dois.

O visual "Obsidian Dark" foi pensado para uso diário prolongado: fundo escuro, números em fonte monoespaçada para leitura financeira e animações discretas.

## 🚀 O que ele faz

### 🤖 Finn, o assistente de IA
- **Voz:** fale o lançamento ("gastei 45 reais no mercado ontem") e ele é transcrito e categorizado.
- **Imagens:** envie a foto de um comprovante ou nota; anexos sem relação com finanças são recusados.
- **Conversas isoladas:** cada conversa tem o próprio histórico, sem misturar sessões nem bases.
- **Alta disponibilidade:** várias chaves de API se revezam, e outro provedor assume se um falhar.

### 🏢 Várias bases, um login
- Contas pessoais, de empresas e de projetos em **bases separadas**, cada uma com a própria identidade visual (logotipo e cores).
- Escolha da base no login para quem administra mais de um negócio.
- Categorias e regras copiadas de uma base para outra com um clique.

### 📊 Lançamentos e análise
- Histórico em três visões: **a pagar**, **a receber** e **pago**.
- **Baixa em lote:** liquide vários lançamentos pendentes de uma vez.
- **Parcelamentos** editáveis parcela a parcela ou na série inteira.
- Painel com **6 indicadores do mês** (gastos, receitas, saldo, taxa de poupança, lançamentos e ticket médio), cada um comparado com o mês anterior.
- Análises de fluxo de caixa, tendência por categoria e evolução do patrimônio, além de metas e orçamento com alertas.

### 🔒 Privacidade
- **Modo sigilo:** esconde todos os valores e gráficos com um clique, para usar em público.
- Login com Google (Firebase Auth) e regras de segurança no banco por usuário.
- **Exclusão completa:** ao encerrar a conta, todos os dados são apagados em cascata, em linha com a LGPD.
- Nenhuma chave no código: tudo por variáveis de ambiente e secrets de build.

---

## 🛠️ Como foi construído

| Camada | Tecnologia | Detalhes |
| :--- | :--- | :--- |
| **Web** | React 19 + Vite 8 + Tailwind CSS | Interface componentizada, ícones Lucide, gráficos interativos |
| **Android** | React Native 0.81 + Expo SDK 54 | UI 100% nativa (sem WebView), NativeWind, animações no thread nativo |
| **Dados e login** | Firebase Firestore + Auth | Sincronização em tempo real com listeners, regras de segurança no servidor |
| **IA** | Groq + Google Gemini | Whisper large-v3 (voz), Llama 3.3 70B (texto), Llama 4 Scout (imagens); Gemini como reserva |
| **Entrega** | GitHub Actions + Vercel | Cada versão publica a web e grava as notas de versão no próprio banco, para o app mostrar as novidades |

## 📱 Plataformas

| Onde | Como |
|---|---|
| **Web** | [caliberda.com.br/kali](https://www.caliberda.com.br/kali) |
| **Android** | App nativo distribuído por APK, com atualização integrada |

---

<div align="center">
  <sub>Feito por <a href="https://github.com/cesarkali">Júlio Caliberda</a> · <a href="https://portifolio.caliberda.com.br">portfólio</a></sub>
</div>
