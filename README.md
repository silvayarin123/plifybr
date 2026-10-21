# Plify — landing page completa (imagens restauradas)

## Publicação no GitHub e na Vercel

1. Extraia o ZIP.
2. Envie o conteúdo da pasta extraída para a raiz de um repositório GitHub: `index.html`, `vercel.json`, `README.md` e `assets/`.
3. Na Vercel, importe o repositório e escolha **Framework Preset: Other**, sem Build Command ou Output Directory personalizada.
4. Publique e force o recarregamento da página para evitar cache antigo.

### Como as imagens funcionam
O `index.html` inclui **todas as imagens, GIF e vídeo em base64** para funcionar mesmo que a pasta `assets/` não seja disponibilizada. `assets/` contém cópias independentes para facilitar ajustes futuros. Não altere o começo `data:image/` ou `data:video/` dos elementos.

Não há regras de redirecionamento que capturem imagens; `vercel.json` contém apenas a configuração de projeto estático.
