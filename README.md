# Prova_2_Mod_6

# Como faz para rodar o projeto:
Para poder rodar o proeto, podemos baixar primeiro as dependências todas com o comando:
```bash
pip install -r requirements.txt
```
E para poder rodar o programa temos que entrar na pasta src/backend e depois digitar o comando:

```bash
python main.py
```

# Para que serve o programa e programa rodando:
Este projeto utiliza o OpenCV para detectar rostos em um vídeo e salvar o vídeo processado com as detecções em um arquivo MP4.

![imagem dele funcionando](/static/foto_rodando.PNG)

Ele consegue fazer as detecção dos rostos.

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

3. Filtros de correlação cruzada
Meio que você treina essa função com as imagens que deseja, nesse nosso caso é face e depois aplicamos mais itens para treinar para que ele consiga "cruzar" as relações para poder inplementar como se fosse um filtro a mais para detectar melhor a expressão.

4. NN Linear
É um módulo versátil no PyTorch e encontra inúmeras aplicações em aprendizado profundo. 
É bastante usado em camadas totalmente conectadas, onde cada neurônio de entrada está conectado a cada neurônio de saída. 

2.3
### Considerando as mesmas alternativas acima, faça uma nova classificação considerando a viabilidade técnica para detecção de emoções através da imagem de uma face.

1. CNN (Convolutional Neural Network)
CNN ia mandar super bem para poder reconhecer as emoções na face das pessoas do vídeo por que daria para capturar alguns detalhes bem pequenos que as outras talvez não conseguiriam.

2. HAAR Cascade
Ele é bom de detectar as faces das pessoas pelo seu banco de dados mas para poder detectar as expressões das pessoas ia ter que passar por mais cascatas o que ia ficar um pouco mais complexo o programa. 

3. NN Linear (Rede Neural Linear)
Viabilidade Técnica: Baixa. Insuficiente para capturar a complexidade das emoções nas expressões faciais.
Acredito que não ia se dar bem para capturar as emoções e expressões faciais. O Pytorch não lidaria muito bem com essas detecções e por requerir a conecção dos neurônios de entrada e o de saída.

4. Filtros de Correlação Cruzada
Os filtros são bons mas teria que aplicar muitos e muitos (muitos filtros mesmo) filtros para que pudesse conseguir classificar e detectar as emoções das pessoas no vídeo.

2.4
### A solução apresentada ou qualquer outra das que foram listadas na questão 2.2. tem a capacidade de considerar variações de um frame para outro (e.g. perceber que em um frame a pessoa está feliz e isso influenciar na detecção do próximo frame)? Se não, quais alterações poderiam ser feitas para que isso seja possível?

Acredito que nenhuma das soluções acima são capazes de verificar essa variação de emoções frame a frame mas se implementarmos alguma coisa a mais, alguma técnica expecífica de aprendizado profundo acho que poderiamos chegar em algum lugar. Enquanto tava estudando vi uma técnica que se chama Long Short-Term Memory (LSTM), meio que ele leva para frente (guarda na "memória") aquilo que estava no frame anterior para poder usar de referência e ver se teve alguma variação.

2.5
### Quem ganha a bola de ouro 2024?

# Vini Malvadeza 7 

