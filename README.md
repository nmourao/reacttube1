# ReactTube

Reações personalizadas em vídeo para YouTube com IA, gravação e upload direto para sua conta.

---

## 🚀 Deploy com Vercel

1. Acesse [https://vercel.com](https://vercel.com) e crie uma conta.
2. Clique em **"New Project"** e conecte seu GitHub.
3. Faça upload deste projeto como um repositório.
4. Certifique-se de que `index.html` está na raiz.
5. Vercel detectará automaticamente como **Static Site**.
6. Clique em **Deploy** e pronto!

---

## 🧠 Configurar OAuth com Google

1. Acesse https://console.cloud.google.com/
2. Crie um novo projeto.
3. Vá em **APIs & Services > Credentials**
4. Clique em **Create Credentials > OAuth 2.0 Client ID**
5. Escolha tipo: **Web Application**
6. Adicione **URIs de redirecionamento autorizados**, como:
   - `http://localhost:3000`
   - `https://SEU-USUARIO.vercel.app`

7. Copie seu `client_id` e edite em `index.html`:

```js
const clientId = 'SEU_CLIENT_ID_AQUI';
```

---

## 📁 Estrutura

```
reacttube-deploy/
├── index.html
├── models/         # Modelos face-api.js
└── README.md
```

Pronto! Agora você tem um app de reações com IA + upload direto pro YouTube! 🎥✨
