# Simulador Cesgranrio — TRANSPETRO 2026

Simulador de provas no estilo da banca **Cesgranrio**, para as ênfases de TI do concurso TRANSPETRO/PSP/TERRA/NÍVEL SUPERIOR 2026.4.

O banco de questões não foi escrito no chute: nasceu da leitura integral do edital oficial e da catalogação, questão a questão, de 7 provas antigas da Cesgranrio (2006–2018) para identificar quais assuntos a banca realmente repete, em que formato e com que peso. O simulador reflete essa distribuição real, não uma cobertura genérica do edital.

## Áreas cobertas

O edital tem 5 ênfases de TI. O banco de questões está sendo construído área por área:

| Ênfase | Status | Questões |
|---|---|---|
| Análise de Sistemas — Processos de Negócios | ✅ completo | 108 |
| Análise de Sistemas — Infraestrutura | ✅ completo | 110 |
| Análise de Sistemas — SAP | 🔒 em construção | — |
| Análise de Sistemas — Segurança Cibernética e da Informação | 🔒 em construção | — |
| Ciência de Dados | 🔒 em construção | — |

Alguns tópicos (Segurança da Informação, Lógica/Raciocínio Lógico, Banco de Dados básico, Gestão de Projetos) são compartilhados entre ênfases cujo Anexo IV traz o mesmo conteúdo quase literalmente — por isso o total de questões de cada área não é a simples soma de blocos exclusivos.

## O que tem aqui

- **`index.html`** — aplicação completa em HTML/CSS/JS puro (sem build, sem dependências), com:
  - **Seletor de área**, guiado pelas vagas reais do Anexo I do edital, cobrindo as 5 ênfases de TI.
  - **Questões inéditas** organizadas por Prioridade 1 (núcleo histórico da banca), Prioridade 2 (reforço) e Prioridade 3 (itens novos do edital sem precedente nas provas antigas), cada uma com explicação pedagógica completa — não só o gabarito, mas por que a resposta certa está certa e por que cada alternativa errada falha.
  - **4 modos de prova**: Treino Rápido, Simulado Médio, Simulado Completo e Treino por Tópico.
  - **Área de Estudo** com conteúdo condensado por tópico, pensado para o contexto exato da prova.
  - **Histórico de tentativas** persistente entre visitas, com revisão completa de qualquer prova antiga (via capacidade de banco de dados do runtime de Artifacts da Claude, com fallback em `localStorage`).
  - **Aba Concurso** com cronograma, formato de prova e vagas de todas as ênfases de TI, direto do edital oficial.

## Como usar

Basta abrir `index.html` em um navegador. Não há passo de build.

## Como o banco de questões foi construído

1. Leitura integral do Edital nº 04 – TRANSPETRO/PSP/TERRA/NÍVEL SUPERIOR 2026.4 (Anexo IV de cada ênfase).
2. Catalogação questão a questão de 7 provas antigas da Cesgranrio para a área de TI (2006, 2011, 2012, 2018), identificando tema, subtema e formato de cada questão específica — cobrindo as ênfases Software, Infraestrutura, Processos de Negócio e SAP (não existe prova antiga para Segurança Cibernética nem Ciência de Dados, ênfases novas neste edital).
3. Construção de um ranking de temas mais recorrentes e um mapa de prioridades de estudo a partir desses dados, por ênfase.
4. Escrita de questões inéditas, no mesmo estilo e proporção identificados, distribuídas proporcionalmente ao peso histórico de cada tema — não um volume arbitrário "tentando cobrir tudo". Para ênfases sem prova antiga no acervo, as questões seguem o Anexo IV e o estilo geral da banca, sinalizando honestamente a ausência de precedente histórico.

Cada questão indica no campo `insp` qual tema/prova real inspirou seu assunto e formato — nenhuma é transcrição literal de prova antiga; todas foram escritas originalmente.
