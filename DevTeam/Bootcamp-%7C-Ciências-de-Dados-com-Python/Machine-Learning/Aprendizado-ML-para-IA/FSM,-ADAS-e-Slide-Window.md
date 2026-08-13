---
title: "FSM, ADAS e Slide Window"
nav_order: 5
parent: "Aprendizado ML para IA"
---

**1. Neuro FSM (Máquina de Estados Finitos Neurais)**

Uma Neuro FSM é uma combinação de redes neurais e máquinas de estados finitos. As redes neurais são usadas para aprender padrões complexos, enquanto a máquina de estados finitos ajuda a manter uma sequência lógica ou um fluxo de operações. No contexto da condução, uma Neuro FSM pode ser usada para detectar e corrigir falhas, como comportamentos inadequados do motorista.

**Exemplo com o Kinect**

O Kinect, originalmente desenvolvido pela Microsoft para jogos, possui sensores que podem detectar movimento e postura. Portanto, ao ser usado em um carro, pode perceber se o motorista está falando ao celular, dormindo ao volante ou se envolvendo em outras atividades distrativas. A combinação do Kinect com uma Neuro FSM permitiria ao sistema não apenas detectar tais comportamentos, mas também tomar ações corretivas, como alertar o motorista ou até mesmo assumir o controle do veículo em situações de emergência.

**2. Sistema ADAS (Sistemas Avançados de Suporte ao Motorista)**

ADAS refere-se a sistemas que fornecem ao motorista assistência em tempo real, melhorando a segurança e a condução. Inclui uma variedade de funções, desde alertas de ponto cego e assistência de manutenção de faixa até frenagem automática de emergência.

No contexto de manobras, um ADAS pode ajudar detectando objetos no caminho do veículo usando sensores e câmeras. Ele pode então fornecer feedback ao motorista sobre a distância e a direção do objeto, ou em sistemas mais avançados, realizar a manobra automaticamente.

**3. Algoritmo de Slide Window (Janela Deslizante)**

O algoritmo de janela deslizante é comumente usado em visão computacional. Ele envolve mover uma "janela" ou sub-região de uma imagem através da imagem completa para detectar objetos de interesse. Em reconhecimento de placas de veículos, por exemplo, a janela deslizante pode ser usada para localizar e identificar a placa em uma imagem maior do carro.

O processo geralmente envolve:
- Definir um tamanho de janela.
- Deslizar a janela por toda a imagem.
- Em cada passo, usar um classificador (como uma rede neural) para determinar se o objeto de interesse está presente na janela atual.
- Repetir o processo com diferentes tamanhos de janela para detectar objetos de diferentes escalas.

Esse método é intensivo em termos computacionais, pois a imagem é analisada várias vezes em diferentes posições e escalas. No entanto, com hardware moderno e otimizações de software, ele pode ser realizado em tempo real para muitas aplicações, incluindo a detecção de placas de veículos.