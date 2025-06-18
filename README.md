![Imagem Ilum](Imagens/header_ilum_leticia.png)

<h1 align="center">Modelagem Epidemiológica SIR e Extensões</h1>

## Descrição do Projeto
Este projeto tem como objetivo simular a propagação de uma doença infecciosa em uma população, utilizando o modelo epidemiológico SIR, considerando cenários de complexidade crescente. A proposta é fornecer uma ferramenta interativa, escrita em Python, que permita ao usuário inserir diferentes parâmetros epidemiológicos (como taxas de transmissão, recuperação, mortalidade, interação entre populações e renovação populacional) e observar como esses fatores afetam a evolução dos grupos Suscetíveis (S), Infectados (I) e Recuperados (R) ao longo do tempo.

Por meio da implementação numérica do modelo e da visualização dos resultados em gráficos, o projeto busca aprofundar o entendimento sobre como epidemias se comportam e como pequenas mudanças nos parâmetros podem impactar significativamente a disseminação de uma doença.

Uma das principais características deste trabalho é a possibilidade de o usuário escolher entre quatro diferentes modelos epidemiológicos, cada um incorporando novos parâmetros para representar fenômenos mais realistas da dinâmica populacional e da transmissão da doença. Além disso, o código serve como uma base didática, ideal para estudantes e pesquisadores interessados em explorar ou expandir modelos epidemiológicos com maior complexidade.

### Modelos disponíveis no projeto: ###
- SIR: Modelo clássico (Suscetíveis-Infectados-Recuperados).

- SIRD: Inclui mortalidade por causa da doença, com o parâmetro μ (taxa de mortalidade).

- SIRD - Dupla População Interagente: Simula a interação entre duas populações distintas, com os parâmetros kab e kba, que controlam a taxa de contato entre os grupos.

- SIRD - Dinâmica Vital: Inclui o efeito de nascimentos e mortes naturais, com o parâmetro eta, representando a taxa de renovação populacional.

A interface permite ao usuário escolher o modelo, inserir os parâmetros de forma personalizada e visualizar os resultados por meio de gráficos de fácil interpretação.

## Sobre o modelo Epidemiológico SIR
O modelo SIR é um modelo matemático clássico usado para descrever a propagação de doenças infecciosas em uma população. Ele divide a população em três grupos:
- S (Suscetíveis): indivíduos que podem ser infectados;
- I (Infectados): indivíduos que estão atualmente infectados e podem transmitir a doença;
- R (Recuperados): indivíduos que se recuperaram da doença e ganharam imunidade.
  
A dinâmica entre esses grupos é representada por um sistema de equações diferenciais que descreve como os indivíduos passam de um grupo para outro ao longo do tempo. As
principais taxas envolvidas são:
- β (beta): taxa de transmissão da doença;
- γ (gama): taxa de recuperação.
  
O modelo parte de algumas suposições simples:
- A população é fixa (não há nascimentos ou mortes naturais no modelo básico);
- A doença confere imunidade após a recuperação;
- A transmissão ocorre por contato entre suscetíveis e infectados.
  
Apesar de sua simplicidade, o modelo SIR é extremamente poderoso para entender o comportamento inicial de surtos e epidemias, como o crescimento de casos, o pico da infecção e o número total de pessoas afetadas.

## Índice

## Objetivos
O principal objetivo deste projeto é desenvolver uma ferramenta interativa e didática para simular diferentes cenários de propagação de doenças infecciosas em populações humanas, utilizando o modelo epidemiológico SIR e suas extensões.

Ao longo do desenvolvimento, buscamos atingir os seguintes objetivos específicos:
- Compreender a dinâmica de transmissão de doenças infecciosas por meio da implementação numérica de diferentes modelos epidemiológicos.
- Permitir a comparação entre diferentes cenários epidemiológicos, variando parâmetros como taxa de transmissão, recuperação, mortalidade, interação entre populações e dinâmica vital da população.
- Fornecer uma interface simples e intuitiva, que permita ao usuário escolher entre os quatro modelos implementados e inserir os parâmetros de forma personalizada.
- Promover a visualização gráfica dos resultados, facilitando a análise do comportamento dos grupos populacionais ao longo do tempo.
- Criar uma base de código modular e extensível, que possa ser utilizada por outros estudantes, pesquisadores ou interessados que desejem explorar novas variações ou incluir outros fenômenos epidemiológicos (como vacinação ou reinfecção).
- incentivar o aprendizado prático de conceitos relacionados à epidemiologia matemática, ciência de dados e programação cinetífica, integrando teoria e prática.

## Tecnologias e Bibliotecas Utilizadas
O projeto foi desenvolvido utilizando a linguagem Python, por sua versatilidade e ampla aplicação em projetos de ciência de dados, modelagem matemática e análise de dados científicos.

- Streamlit: Framework que permite transformar scripts Python em aplicações web interativas, facilitando a execução do projeto diretamente no navegador com uma interface amigável.

- NumPy: Para realizar cálculos numéricos e manipulação de arrays de forma eficiente.

- Matplotlib: Responsável pela geração dos gráficos que representam a evolução das populações ao longo do tempo.

- SciPy: Utilizada para resolver as equações diferenciais ordinárias (EDOs) que descrevem a dinâmica dos modelos epidemiológicos.

## Como Funciona a Simulação
A simulação é baseada na resolução numérica de equações diferenciais que descrevem a dinâmica de transmissão da doença, de acordo com o modelo epidemiológico escolhido pelo usuário.

O processo funciona da seguinte forma:

#### 1. Escolha do modelo: ####
O usuário seleciona um dos quatro modelos disponíveis (SIR, SIRD, SIRD - Dupla População Interagente ou SIRD - Dinâmica Vital).

#### 2. Definição dos parâmetros: ####
Em seguida, o usuário insere os valores para os parâmetros específicos de cada modelo, como taxa de transmissão, taxa de recuperação, mortalidade, taxas de interação entre populações ou taxa de renovação populacional.

#### 4. Resolução das equações: ####
O programa utiliza métodos numéricos (com apoio da biblioteca SciPy) para resolver as equações diferenciais que descrevem o comportamento das populações ao longo do tempo.

#### 5. Visualização dos resultados: ####
Após o cálculo, os resultados são apresentados de forma gráfica, mostrando a evolução de cada grupo populacional (S, I, R, e quando aplicável, D e demais categorias**) ao longo dos dias simulados.

## Parâmetros de Entrada

##  Exemplo de Saída (Gráficos)

## Como Executar o Projeto

## Conclusões

## Possíveis Extensões Futuras

## Contribuidores

## Professores

## Referências
