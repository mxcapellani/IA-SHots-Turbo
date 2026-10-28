# Auditoria funcional — 1.0.0

## Fonte e classificação
Fonte: descrição funcional fornecida pelo usuário, preservada em [SOURCE_SPECIFICATION.md](SOURCE_SPECIFICATION.md). Não houve acesso ao GPT original, configurações privadas, imagens de teste ou conversas exemplares.

“Verificada documentalmente” significa presença explícita na fonte e implementação no núcleo; não significa comportamento medido. “Inferida” significa decisão necessária de implementação. “Não verificada” requer execução real.

| Dimensão | Capacidade | Classificação | Evidência ou teste |
|---|---|---|---|
| Finalidade | Reconstrução de fotografia em prompts | Verificada documentalmente | Fonte §§1–3; T01–T06 |
| Especialização | Composição, iluminação, óptica, materiais | Verificada documentalmente | Fonte §3; T07–T10 |
| Entrada | Imagem direta | Verificada documentalmente; execução não verificada | T01, T02 |
| Entrada | Link de imagem | Condicional; não verificada em execução | T03, T04 |
| Saída | Dois prompts PT/EN completos | Verificada documentalmente | T01–T10, T17 |
| Estrutura | Sujeito, ação, ambiente, estilo, técnica, qualidade | Verificada documentalmente | T01, T06 |
| Apresentação | Profissional, objetiva, sem emojis | Verificada documentalmente | T01–T20 |
| Falta de entrada | Pedir referência antes de analisar | Verificada documentalmente | T02, T19 |
| Técnica | Estimativas sem EXIF inventado | Verificada documentalmente | T07 |
| Contexto | Reutilizar âncoras em revisão | Inferida da função de refinamento | T11, T18 |
| Ultimate | Dez camadas e fidelidade máxima | Definida; eficácia não verificada | T08, T09 |
| Ultimate | Cinematográfico, editorial, comercial, técnico | Definida; eficácia não verificada | T12–T15 |
| Ultimate | Negativo e adaptação | Condicional; não verificada | T16 |
| Ferramentas | Visão e acesso externo | Dependem do host | T03, T04, T19 |
| Geração | Imagem resultante | Não verificada; não automática | T20 |
| Arquivos/dados | Análise genérica de documentos e dados | Não estabelecida | Não adicionar ao escopo |
| Iniciadores | Opções originais | Não verificados | Solicitar captura ou lista ao original |

## Experiência essencial
Referência válida → interpretação fotográfica → prioridades → construção → tradução → validação → entrega bilíngue. Não trocar pela criação sem referência nem perguntar estilo quando o pedido já é reconstrução fiel.

## Melhorias distintas do original
Fidelidade sistemática, evidência explícita, realismo material/anatômico, técnicas equivalentes, modos avançados, refinamento, negativo opcional e auditoria bilíngue. A fonte os identifica como ampliações; não atribuir histórico comprovado a eles.

## Limitações
Exemplos reais e imagens pareadas ainda não disponíveis. A auditoria verifica requisitos textuais, não precisão visual. Testes comparativos permanecem não executados até registro com artefatos reais.
