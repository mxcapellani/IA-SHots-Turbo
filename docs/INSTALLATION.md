# Instalação, ativação e atualização

## Instalação portátil
1. Extrair o ZIP mantendo a estrutura.
2. Copiar `.agents/skills/iashots-turbo-ultimate/` para a área de skills aceita pelo agente. Para descoberta por projeto, preservar esse caminho no repositório.
3. Usar o nome `iashots-turbo-ultimate` na solicitação se o host permitir seleção explícita. A forma de importação depende da aplicação.
4. Enviar uma referência real para teste. Conferir ambos os prompts e ausência de detalhes inventados.

O núcleo é autossuficiente, mas as referências devem acompanhar a instalação quando possível. Não é necessário renderizar imagens para usar o texto. Sem visão, análise visual direta fica indisponível.

## Atualização
Guardar personalizações separadamente. Substituir a pasta inteira por uma versão validada, sem misturar referências antigas. Conferir changelog e repetir casos já aprovados no host. Atualizar somente após executar o validador estrutural.

## Preparação do GitHub
Na pasta extraída, executar os comandos abaixo em ambiente GitHub CLI autenticado. O fluxo com API disponível nesta conversa é independente desses comandos.

```bash
git init
git add .
git commit -m "feat: release IAShots Turbo Ultimate v1.0.0"
git branch -M main
git remote add origin https://github.com/mxcapellani/IA-SHots-Turbo.git
git push -u origin main
```
Se o repositório já existir, conectar seu endereço real e publicar sem sobrescrever conteúdo alheio. Nunca colocar senhas ou tokens nos arquivos. A criação automática depende das permissões da ferramenta utilizada.
