# Simulador Processos de Negócios — TRANSPETRO 2026

Simulador de provas no estilo da banca **Cesgranrio**, feito sob medida para a ênfase **Análise de Sistemas — Processos de Negócios** do concurso TRANSPETRO/PSP/TERRA/NÍVEL SUPERIOR 2026.4.

O banco de questões não foi escrito no chute: nasceu da leitura integral do edital oficial e da catalogação, questão a questão, de 7 provas antigas da Cesgranrio (2006–2018) para identificar quais assuntos a banca realmente repete, em que formato e com que peso. O simulador reflete essa distribuição real, não uma cobertura genérica do edital.

## O que tem aqui

- **`index.html`** — aplicação completa em HTML/CSS/JS puro (sem build, sem dependências), com:
  - **90 questões inéditas** organizadas por Prioridade 1 (núcleo histórico da banca) e Prioridade 2 (reforço), cada uma com explicação pedagógica completa — não só o gabarito, mas por que a resposta certa está certa e por que cada alternativa errada falha.
  - **4 modos de prova**: Treino Rápido, Simulado Médio, Simulado Completo e Treino por Tópico.
  - **Área de Estudo** com conteúdo condensado por tópico (8 tópicos), pensado para o contexto exato da prova.
  - **Histórico de tentativas** persistente entre visitas (via capacidade de banco de dados do runtime de Artifacts da Claude, com fallback em `localStorage`).

## Como usar

Basta abrir `index.html` em um navegador. Não há passo de build.

## Como o banco de questões foi construído

1. Leitura integral do Edital nº 04 – TRANSPETRO/PSP/TERRA/NÍVEL SUPERIOR 2026.4 (Anexo IV, Ênfase 5).
2. Catalogação questão a questão de 7 provas antigas da Cesgranrio para a área de TI (2006, 2011, 2012, 2018), identificando tema, subtema e formato de cada questão específica.
3. Construção de um ranking de temas mais recorrentes e um mapa de prioridades de estudo a partir desses dados.
4. Escrita de questões inéditas, no mesmo estilo e proporção identificados, distribuídas proporcionalmente ao peso histórico de cada tema — não um volume arbitrário "tentando cobrir tudo".

Cada questão indica no campo `insp` qual tema/prova real inspirou seu assunto e formato — nenhuma é transcrição literal de prova antiga; todas foram escritas originalmente.
