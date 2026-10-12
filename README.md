# Bia Studio

App (uma página, sem servidor) para gerar os vídeos de moda da Bia Souza no pod, a partir do celular.
Ele conversa direto com o repositório privado `soudedeco/bia-ai-studio` pela API do GitHub.

**Este repositório não guarda nenhum segredo nem foto.** A chave de acesso fica só no navegador de quem usa;
fotos, jobs e vídeos ficam no repositório privado.

## Telas

- **Looks**: sobe fotos do rolo da câmera para `assets/fashion/<look>/` e recorta detalhes em 9:16.
- **Criar**: escolhe qualidade, textura, upscale, interpolação, referências de detalhe e monta os takes (foto inicial, final opcional, duração, movimento). Avisa os erros conhecidos (foto final que congela, distância longa entre fotos, giros que inventam costas).
- **Execuções**: acompanha a fila, assiste e baixa cada take, manda takes para a edição e refaz um take em qualidade máxima.
- **Edição**: marca início e fim de cada trecho, faz a prévia e monta o filme final (workflow `Moda - montar edicao`, sem GPU).

## Chave de acesso

GitHub → Settings → Developer settings → Fine-grained tokens → acesso só ao `bia-ai-studio`,
com **Contents: Read and write** e **Actions: Read and write**.
