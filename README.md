# Projeto Python de detecção de gênero e idade com OpenCV

Primeiro apresentando a você as terminologias usadas neste projeto python avançado de detecção de gênero e idade

## O que é Visão Computacional?
Visão Computacional é o campo de estudo que permite que os computadores vejam e identifiquem imagens e vídeos digitais como um humano faria. Os desafios que enfrenta decorrem em grande parte da compreensão limitada da visão biológica. A Visão Computacional envolve a aquisição, processamento, análise e compreensão de imagens digitais para extrair dados de alta dimensão do mundo real, a fim de gerar informações simbólicas ou numéricas que podem ser usadas para tomar decisões. O processo geralmente inclui práticas como reconhecimento de objetos, rastreamento de vídeo, estimativa de movimento e restauração de imagens.

## O que é OpenCV?
OpenCV é a abreviação de Visão Computacional de Código Aberto. Intuitivamente pelo nome, é uma biblioteca de visão computacional e aprendizado de máquina de código aberto. Esta biblioteca é capaz de processar imagens e vídeos em tempo real, ao mesmo tempo em que possui recursos analíticos. Ele suporta as estruturas de Deep Learning TensorFlow , Caffe e PyTorch.

## O que é uma CNN?
Uma Rede Neural Convolucional é uma rede neural profunda (DNN) amplamente utilizada para fins de reconhecimento e processamento de imagens e PNL . Também conhecida como ConvNet, uma CNN possui camadas de entrada e saída e várias camadas ocultas, muitas das quais são convolucionais. De certa forma, as CNNs são perceptrons multicamadas regularizados.

Projeto Python de Detecção de Gênero e Idade - Objetivo
Para construir um detector de gênero e idade que possa adivinhar aproximadamente o gênero e a idade da pessoa (rosto) em uma imagem usando Deep Learning no conjunto de dados Adence.

Detecção de Gênero e Idade – Sobre o Projeto
Neste projeto Python, usei o Deep Learning para identificar com precisão o sexo e a idade de uma pessoa a partir de uma única imagem de um rosto. Usaremos os modelos treinados por Tal Hassner e Gil Levi . O gênero previsto pode ser 'Masculino' e 'Feminino', e a idade prevista pode ser uma das seguintes faixas- (0 – 2), (4 – 6), (8 – 12), (15 – 20) , (25 – 32), (38 – 43), (48 – 53), (60 – 100) (8 nós na camada softmax final). É muito difícil adivinhar com precisão uma idade exata a partir de uma única imagem devido a fatores como maquiagem, iluminação, obstruções e expressões faciais. E assim, fazemos disso um problema de classificação em vez de torná-lo um problema de regressão.

## A arquitetura da CNN
A rede neural convolucional para este projeto python tem 3 camadas convolucionais:

camada convolucional; 96 nós, tamanho do kernel 7
camada convolucional; 256 nós, tamanho do kernel 5
camada convolucional; 384 nós, tamanho do kernel 3
Possui 2 camadas totalmente conectadas, cada uma com 512 nós, e uma camada de saída final do tipo softmax.

Para ir sobre o projeto python, vamos:

Detectar rostos
Classifique em masculino/feminino
Classifique em uma das 8 faixas etárias
Coloque os resultados na imagem e exiba-a

## O conjunto de dados
Para este projeto python, usei o conjunto de dados Adience; o conjunto de dados está disponível em domínio público e você pode encontrá-lo aqui . Esse conjunto de dados serve como referência para fotos de rosto e inclui várias condições de imagem do mundo real, como ruído, iluminação, pose e aparência. As imagens foram coletadas de álbuns do Flickr e distribuídas sob a licença Creative Commons (CC). Tem um total de 26.580 fotos de 2.284 indivíduos em oito faixas etárias (como mencionado acima) e tem cerca de 1 GB de tamanho. Os modelos que usaremos foram treinados neste conjunto de dados.

## Pré-requisitos
Você precisará instalar o OpenCV (cv2) para poder executar este projeto. Você pode fazer isso com pip

pip instalar opencv-python
