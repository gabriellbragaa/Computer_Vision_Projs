# Vis-o_Computacional

# 📷 Processamento de Imagens com Filtros em Python

Este repositório demonstra a aplicação de conceitos de **processamento de imagens** em Python, com foco na utilização de **filtros espaciais** e **filtros no domínio da frequência**. As imagens utilizadas passaram por **transformações geométricas**, **operações lógicas** e **técnicas de realce**, permitindo a observação clara dos efeitos de cada filtro.

---

## 🧩 Etapas do Processamento

Antes da aplicação dos filtros, as imagens passam por:

- 🔄 **Transformações geométricas**: rotação, translação, redimensionamento;
- ⚙️ **Operações lógicas**: limiarização e operações bit a bit (AND, OR, NOT);
- Estas etapas ajudam a simular condições reais de ruído e facilitar a filtragem.

---

## 🧪 Algoritmos e Filtros Aplicados

### 📁 `spatial_filter.py` — Filtros Espaciais

Aplica filtros diretamente sobre os valores dos pixels, sendo ideais para suavização e remoção de ruídos.

- 📌 **Filtro de Média**: Suaviza a imagem calculando a média dos valores na vizinhança.
- 📌 **Filtro de Mediana**: Reduz ruídos como sal e pimenta substituindo o valor do pixel pela mediana local.

> **Objetivo**: Remoção de ruídos preservando as bordas.

---

### 📁 `fft_filter.py` — Filtros no Domínio da Frequência

Utiliza a **Transformada Rápida de Fourier (FFT)** para processar imagens no domínio da frequência.

- 🔍 Remove **componentes de alta frequência** (ruídos);
- 📉 Aplica **filtros passa-baixa** para suavização global;
- 📈 Permite visualizar o espectro da imagem para melhor análise.

> **Objetivo**: Redução de ruídos de alta frequência utilizando a FFT.

---

### 📁 `filter_responser.py` — Resposta de Filtros

Compara diferentes filtros e mostra como cada um afeta a imagem.

- ✨ **Filtro de Acentuação (Sharpening)**: Realça bordas e detalhes;
- 🧠 **Kernel de Acentuação**: Matriz convolucional para destacar mudanças de intensidade.

> **Objetivo**: Melhorar a nitidez e o contraste após a suavização.

---

## 🧠 Conclusão

Os filtros implementados demonstram na prática como é possível:

- Reduzir ruídos (espacial e frequência);
- Preservar ou acentuar detalhes importantes;
- Compreender o efeito individual de cada tipo de filtro.

Este projeto serve como base para aplicações em **visão computacional**, **realce de imagens médicas**, **análise de padrões** e muito mais.

---

## 🚀 Requisitos

- Python 3.x
- Bibliotecas: `numpy`, `opencv-python`, `matplotlib`, `scipy` (dependendo dos scripts)

```bash
pip install numpy opencv-python matplotlib scipy
