# Benford's Law
This is a statistical law that predicts a logarithmic (non-uniform) distribution of the leading digits in a dataset, where the number 1 appears as the first digit about 30.1% of the time, while the number 9 appears only 4.6% of the time. In this repository, we will explore this further!

This project provides a mathematical and empirical proof od Benford's law (also known as the first-digit law). It was structured to serve as a GitHub portfolio project for study purposes, demonstrating statistical concepts, data analitycs and statistical hypothesis tests.

The script simulates different types of real-world data (and manipulated scenarios), analyzes the frequency of their leading significant digits, and performs a rigorous statistical goodness-of-fit test (Chi-Square) to determine whether or not the data adheres to the law.

# Lei de Benford
Esta é uma lei estatística que prevê uma distribuição logarítmica (não uniforme) dos primeiros dígitos de um conjunto de dados, onde o número 1 é o primeiro dígito em cerca de 30,1% das vezes e o 9 em apenas 4,6%. Neste repositório vamos ver um pouco mais sobre!

Este projeto apresenta uma comprovação matemática e empírica da Lei de Benford (também conhecida como a lei do primeiro dígito). Ele foi estruturado para servir como um projeto de portfólio no GitHub para fins de estudo, demonstrando conceitos estatísticos, análise de dados e testes de hipóteses estatísticas.

O script simula diferentes tipos de dados do mundo real (bem como cenários manipulados), analisa a frequência de seus dígitos significativos iniciais e realiza um teste estatístico rigoroso de aderência (Qui-Quadrado) para determinar se os dados seguem ou não a lei.

# What is Benford's Law?

Benford's Law states that, in many naturally and organically occurring numerical datasets, the leading digits are not uniformly distributed (where each number from 1 to 9 would have an 11.1% chance of appearing).

Instead, the digit 1 appears as the leading significant digit approximately 30.1% of the time, while the digit 9 appears only 4.6% of the time.

The theoretical probability of a digit $d \in {1, ..., 9}$ being the leading significant digit is modeled by the logarithmic equation:

$$P(d) = \log_{10}\left(1 + \frac{1}{d}\right)$$

# O que é a lei de Benford?

A Lei de Benford afirma que, em muitos conjuntos de dados numéricos que ocorrem de forma natural e orgânica, os dígitos iniciais não estão distribuídos de forma uniforme (onde cada número de 1 a 9 teria 11,1% de chance de aparecer).

Em vez disso, o dígito 1 aparece como o primeiro dígito significativo em aproximadamente 30,1% das vezes, enquanto o dígito 9 aparece em apenas 4,6% das vezes.

A probabilidade teórica de um dígito $d \in {1, ..., 9}$ ser o primeiro dígito significativo é modelada pela equação logarítmica:

$$P(d) = \log_{10}\left(1 + \frac{1}{d}\right)$$

# Intuição/justificativa matemática

A explicação mais sólida é a invariância de escala: se uma distribuição de primeiros dígitos é independente das unidades (metros vs. pés, reais vs. dólares), a única distribuição possível é a de Benford. Também há o argumento da invariância de base. A ideia central: se você olhar os dados numa escala logarítmica, eles tendem a se espalhar uniformemente ao longo das ordens de magnitude — e ao voltar pra escala linear, os intervalos que começam com dígitos menores são "mais largos" em log, capturando mais valores.

O intervalo em log de números que começam com dígito 
𝑑
d é [log 10 𝑑, log 10(𝑑+1))d

log 10 (d+1)), cujo comprimento é exatamente log 10(1+1/𝑑). Isso é a fórmula.
