<div align="center">

[![Hebrew](https://img.shields.io/badge/עברית-Click-blue)](README.md)
[![English](https://img.shields.io/badge/English-Click-yellow)](README_EN.md)
[![Portuguese](https://img.shields.io/badge/Português-Click-green)](README_PT.md)

</div>

# AI Analyzer - Melhoria para n8n-workflows

**Eliad Shahar**, convido você a avaliar esta implementação. Como alguém que aprecia muito o trabalho que você dedicou ao n8n-workflows, acredito que o AI Analyzer agrega um valor significativo à comunidade, tornando os fluxos de trabalho acessíveis a usuários menos técnicos e economizando tempo para os profissionais. Eu adoraria colaborar, receber feedback e ajudar a mesclar (Merge) esses recursos em seu repositório oficial.

*Vídeo de Demonstração: AI Analyzer - Enhancement for n8n-workflows*

[![AI Analyzer Demo](https://img.youtube.com/vi/LGa-HX_uU9U/0.jpg)](https://www.youtube.com/watch?v=LGa-HX_uU9U)

## Sobre
Este projeto apresenta o **AI Analyzer**, um complemento (Add-on) significativo para o excelente projeto original [n8n-workflows](https://github.com/Zie619/n8n-workflows).
O objetivo deste complemento é enriquecer a experiência do usuário adicionando uma camada de Inteligência Artificial que analisa, explica e otimiza fluxos de trabalho de automação complexos.

> **Aviso Legal:** Este desenvolvimento é uma melhoria independente e uma iniciativa voluntária submetida à consideração do criador original, Eliad Shahar. Não é uma parte oficial do projeto original até que seja potencialmente mesclado.

---

## Capacidades do AI Analyzer
O AI Analyzer transforma arquivos JSON técnicos em insights de negócios claros. As principais capacidades incluem:

*   **Análise Inteligente de Fluxo de Trabalho**: O sistema "lê" a estrutura JSON, ignorando descrições genéricas e focando na lógica real dos Nós (Nodes) e suas conexões.
*   **Detecção de Padrões e Anomalias**: Detecção automática de valores codificados (Hardcoded) que podem atrapalhar os usuários, como IDs de planilhas específicos, endereços de e-mail ou chaves de API.
*   **Sugestões de Otimização**: Recomendações baseadas em IA para melhorar a eficiência do fluxo de trabalho e adaptá-lo a diferentes necessidades de negócios.
*   **Integração Transparente**: A ferramenta é incorporada naturalmente na Interface de Usuário existente (Modal de Detalhes do Fluxo de Trabalho), não exigindo instalações externas complexas.

---

## Vantagens e Benefícios
A análise produzida pelo AI Analyzer cobre de forma abrangente os seguintes pontos:

*   🎯 **Objetivo Principal ("Elevator Pitch"):** Um resumo conciso e focado (2 frases) do valor e resultado do fluxo de trabalho.
*   ⚡ **Lógica Passo a Passo**: Uma explicação narrativa e simples do fluxo de ações: Gatilho -> Ação -> Resultado, evitando jargões técnicos confusos.
*   🛠️ **Pontos de Configuração:** Uma lista precisa de nós que requerem configuração manual pelo usuário. Por exemplo: "No nó 'Gmail', altere o endereço do destinatário para o seu próprio."
*   💡 **Casos de Uso no Mundo Real:** Exemplos concretos de como o fluxo de trabalho economiza tempo ou dinheiro.
*   ⚠️ **Pré-requisitos:** Detalhes sobre credenciais, chaves de API ou colunas de banco de dados necessárias.
*   🚀 **Dicas de Personalização:** Ideias criativas para usar o fluxo de trabalho para diferentes tipos de negócios ou integrações alternativas (por exemplo, trocar Slack por WhatsApp).

**Suporte Multi-Modelo e Multi-Idioma:** O sistema suporta vários idiomas (Hebraico, Inglês, Espanhol, Russo, etc.) e permite que o usuário edite o System Prompt para refinar os resultados ou alterar a personalidade da IA.

---

## Seção Técnica e Implementação
*   **Estrutura do Código:** As mudanças estão concentradas principalmente em `static/index.html` e arquivos JavaScript associados, onde a lógica do `WorkflowApp` e a interação com os Prompts são definidas. Além disso, novos arquivos foram adicionados: `ai_analyzer.py` contendo a lógica de análise JSON, e `system_prompts.py` que centraliza as instruções do sistema para todos os idiomas. Além disso, `.env.example` deve ser usado como modelo para configuração de variáveis de ambiente.
*   **Compatibilidade:** O desenvolvimento foi projetado para ser totalmente compatível com o projeto original. Não requer alterações no banco de dados existente ou no servidor Backend (Python/FastAPI).
*   **Teste:**
    1.  Execute o projeto (`python run.py`).
    2.  Abra um navegador no endereço local.
    3.  Clique em qualquer fluxo de trabalho para abrir o modal.
    4.  Clique no botão "AI Analyzer" (ou selecione um idioma) para ver a mágica acontecer.
