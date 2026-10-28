# IAShots Turbo Ultimate

Versão 1.0.0 — engenharia de prompts para fotografia realista baseada em referências.

A Skill recebe uma imagem ou link acessível, interpreta sua construção fotográfica e entrega dois prompts completos: português e inglês. Seu núcleo preserva a ordem **sujeito → ação → ambiente → estilo → detalhes técnicos → qualidade** e a comunicação profissional sem emojis.

## Funções preservadas
Análise de pessoas, animais, produtos, veículos, arquitetura e paisagens; pose e ação; composição, ambiente, luz do sujeito e do fundo; estilo, materiais e óptica aparente; solicitação de referência ausente e entrega bilíngue. São funções documentadas no material fornecido, não desempenho empiricamente comprovado.

## Melhorias Ultimate
Análise interna em dez camadas, prioridade de fidelidade, controle de invenções, modos cinematográfico/editorial/comercial/técnico, refinamento, adaptação por plataforma e negativo opcional condicionado ao gerador. Esses recursos são extensões e ainda requerem teste comportamental.

## Uso
Enviar uma fotografia e pedir “Reconstrua esta referência em prompts realistas”. Uma imagem sem texto inicia o fluxo universal automaticamente. Para revisão: “Mantenha tudo e altere somente o fundo”. Sem referência, a Skill solicita o envio antes de analisar; não cria uma imagem imaginária para substituir a fotografia.

## Instalação e atualização
Ver [instalação](docs/INSTALLATION.md). O núcleo está em [.agents/skills/iashots-turbo-ultimate/SKILL.md](.agents/skills/iashots-turbo-ultimate/SKILL.md). Colocar a pasta completa no diretório de descoberta aceito pelo host ou importar pelo método da plataforma. Publicação no GitHub não instala automaticamente no ChatGPT.

## Pacote
- Núcleo autossuficiente e quatro referências especializadas.
- Auditoria, especificação e protocolo comparativo em `docs/`.
- Três exemplos completos bilíngues em `examples/`.
- Vinte casos de aceitação, validador, testes do validador e workflow de CI.
- A especificação original fornecida está preservada em `docs/SOURCE_SPECIFICATION.md`.

Os exemplos são cenários sintéticos identificados; não foram disponibilizadas imagens nem respostas reais do agente original. Testes visuais dependem de fixtures reais autorizadas.

## Dependências e permissões
Visão é necessária para observar imagens. Links exigem acesso externo autorizado. Sem essas capacidades, pedir a referência ou declarar limitação. Gerador externo é necessário apenas para produzir imagem: a saída padrão é texto. Não requer API, token ou serviço permanente.

O validador usa Python 3.9+ e PyYAML 6.x. A instalação inicial da biblioteca pode exigir rede, mas a validação não acessa serviços externos nem credenciais. GitHub Actions tem acesso somente de leitura ao conteúdo.

## Verificação
```bash
python -m pip install -r tests/requirements.txt
python tests/validate_skill.py
python tests/test_validator.py
```
Esses comandos verificam estrutura e detecção de falhas. [Casos de aceitação](tests/acceptance-cases.md) e [comparação](docs/COMPARATIVE_TESTS.md) requerem execução no modelo anfitrião; não são considerados aprovados pelo validador.

## Limitações
Não há garantia de reprodução idêntica, EXIF recuperado, superioridade universal do inglês, compatibilidade de versão ou equivalência ao GPT original. Separar observação de técnica sugerida. Suporte a negativo e geração direta dependem de plataforma e pedido. Não há iniciadores originais conhecidos.

## Contribuição e licença
Ver [contribuições](CONTRIBUTING.md) e [histórico](CHANGELOG.md). MIT, copyright 2026 mxcapellani. Implementação independente; marcas de plataformas pertencem aos respectivos titulares.
