# Sistema de Avaliação de Protocolos Médicos

Este repositório contém o sistema de avaliação de protocolos médicos hospitalares da rede Sancta Maggiore/Prevent Senior.

## Estrutura

- `DAK-XX - Nome/` - Protocolos individuais para avaliação
- `scripts/` - Ferramentas Python para processamento de PDFs e análise
- `prompts/` - Templates e metodologias de avaliação
- `Opus 4/` - Prompts e templates avançados

## Metodologia de Avaliação

O sistema utiliza uma metodologia de 9 dimensões para avaliar protocolos:

1. Estrutura Algorítmica (20%)
2. Objetividade Clínica (20%)
3. Aplicabilidade Clínica (10%)
4. Gestão de Encaminhamentos (15%)
5. Representação Visual e Fluxograma (10%)
6. Segurança Clínica e Populações Especiais (5%)
7. Utilidade das Informações Coletadas (10%)
8. Consistência entre Texto e Fluxograma (5%)
9. Implementabilidade Digital (5%)

## Como Usar

1. Extrair imagens dos PDFs:
   ```bash
   python scripts/extract_pdf_images.py "DAK-XX - Nome do Protocolo/*.pdf"
   ```

2. Analisar o protocolo seguindo a metodologia em `prompts/Avaliação de Protocolo/`

3. Gerar relatório em `DAK-XX/Avaliacao-Protocolo-DAKXX.md`

Veja [CLAUDE.md](CLAUDE.md) para instruções detalhadas.
