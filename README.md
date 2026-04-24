# Aula Prática 4 — DFT e DCT

Relatório desenvolvido para a disciplina **Processamento de Sinais I** no **CEFET/RJ**, com foco em análise espectral, resolução em frequência e compressão de sinais utilizando a **Transformada Discreta de Fourier (DFT)** e a **Transformada Discreta de Cossenos (DCT)**.

## Autor

**Caio Bernardo Maciel**

## Disciplina

**Processamento de Sinais I**  
**CEFET/RJ**

---

## Visão geral

Este repositório reúne os materiais utilizados na elaboração da **Aula Prática 4 — DFT e DCT**, incluindo:

- relatório em LaTeX;
- versão final em PDF;
- imagens e gráficos gerados ao longo da análise;
- arquivos de entrada utilizados nos experimentos;
- scripts empregados para gerar resultados numéricos e figuras.

O trabalho explora aplicações práticas da DFT e da DCT em problemas clássicos de processamento digital de sinais, tanto em sinais unidimensionais quanto bidimensionais.

---

## Objetivos do trabalho

O principal objetivo desta prática é investigar o comportamento da DFT e da DCT em diferentes contextos, observando como essas transformadas se comportam em tarefas de:

- representação de sinais no domínio da frequência;
- comparação entre DTFT e DFT;
- análise de resolução espectral;
- avaliação do efeito do zero-padding;
- compressão de sinais de áudio;
- análise de energia em imagens;
- compressão de imagens por DCT em blocos.

---

## Conteúdo abordado

O relatório está dividido em cinco partes principais:

### 1. Comparação entre DTFT e DFT
Análise do sinal com comparação entre a DTFT contínua e a DFT para diferentes valores de \(N\), evidenciando como o aumento do número de pontos melhora a representação espectral.

### 2. Resolução espectral e zero-padding
Estudo do sinal composto por duas senoides muito próximas em frequência, com o objetivo de analisar:

- a influência do número de amostras reais;
- a diferença entre aumento real do tempo de observação e uso de zero-padding;
- as limitações do zero-padding na separação de componentes espectrais próximas.

### 3. Compressão de áudio com DFT e DCT
Compressão do arquivo `handel.wav` por retenção dos coeficientes mais energéticos da DFT e da DCT, comparando:

- número de coeficientes necessários;
- erro quadrático médio;
- eficiência de compactação energética;
- qualidade esperada do sinal reconstruído.

### 4. Análise de energia da imagem no domínio da DCT
Aplicação da DCT 2-D à imagem `sosias.jpg` para avaliar a distribuição da energia na transformada, verificando a predominância das componentes de baixa frequência.

### 5. Compressão de imagem por DCT em blocos
Compressão da imagem `sosias.jpg` em blocos \(8 \times 8\) e \(64 \times 64\), analisando a relação entre:

- tamanho do bloco;
- taxa de preservação de energia;
- número de coeficientes mantidos;
- erro quadrático médio;
- qualidade visual das imagens reconstruídas.

---

## Principais conclusões

A partir dos experimentos realizados, observou-se que:

- a **DFT** pode ser interpretada como uma amostragem da **DTFT**;
- o aumento de \(N\) melhora a representação do espectro, mas não altera o conteúdo espectral do sinal;
- o **zero-padding** melhora a visualização do espectro, mas não aumenta a resolução espectral real;
- para compressão de áudio, a **DCT** apresentou melhor compactação energética do que a **DFT**;
- na análise da imagem, a maior parte da energia da DCT ficou concentrada nas componentes de baixa frequência;
- na compressão por blocos, blocos menores preservaram melhor a qualidade visual, enquanto blocos maiores favoreceram compressão mais agressiva com maior degradação.
