# Prova_2_Mod_6

# Respondendo as perguntas técnicas:

2.1
### Descreva de maneira concisa (um parágrafo no máximo) o funcionamento do método de detecção escolhido.

O funcionamento escolhido para fazer a detecção das faces e expressões foi o HaarCascade, que funcionca como um tipo de cascata mesmo (ora ora, temos um Sherlock Holmes aqui não é mesmo ???). Mas temos as imagens positivas = fotos de faces de pessoas para formar um banco de dados e as imagens negativas = imagens quaisquer como avião, carro, bicicleta, barco... E o Haar de fato são as features (retângulos pequenos pretos e brancos) que fazem as distinções de lábio, boca, nariz e olhos.

2.2
### Considere as seguintes alternativas para resolver o problema de detecção de faces:
* HAAR Cascade
* CNN
* NN Linear
* Filtros de correlação cruzada
### Classifique-os (coloque em ordem) em termos de viabilidade técnica (se é possível resolver o problema), facilidade de implementação e versatilidade da solução. Justifique sua classificação. 

1. HAAR Cascade
Nesse caso eu preferi usar o HAAR Cascade por que ele é mais fácil de implementar, ja tem um banco de dados contendo muitas faces então fica mais fácil de identificar no vídeo pois tem uma cara gigante do Messi e do CR7 no vídeo.

2. CNN (Redes Neurais Convolucionais)
Podemos perceber que as CNNs são mais eficientes para processar imagens e isso acontece por que as CNNs conseguem capturar padrões espaciais e temporais em imagens, enquanto as redes neurais tradicionais não conseguem.

3. NN Linear
É um módulo versátil no PyTorch e encontra inúmeras aplicações em aprendizado profundo. 
É bastante usado em camadas totalmente conectadas, onde cada neurônio de entrada está conectado a cada neurônio de saída. 

4. Filtros de correlação cruzada
Meio que você treina essa função com as imagens que deseja, nesse nosso caso é face e depois aplicamos mais itens para treinar para que ele consiga "cruzar" as relações para poder inplementar como se fosse um filtro a mais para detectar melhor a expressão.

2.3
### Considerando as mesmas alternativas acima, faça uma nova classificação considerando a viabilidade técnica para detecção de emoções através da imagem de uma face.


