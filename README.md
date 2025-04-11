# -Dog-vs-Cat-Image-Classifier

Este projeto implementa um classificador de imagens para diferenciar entre **cachorros** e **gatos**, utilizando a arquitetura **MobileNetV2** e aprendizado profundo com TensorFlow/Keras.

## 📚 Sobre

O notebook `dogVsCat.ipynb` apresenta:
- Pré-processamento de imagens com `ImageDataGenerator`;
- Transfer Learning com MobileNetV2;
- Treinamento e avaliação do modelo;
- Visualização de métricas (acurácia, loss).

## 🧠 Tecnologias

- Python 3.10+
- TensorFlow / Keras
- MobileNetV2 (transfer learning)
- Google Colab ou ambiente local com GPU

Dataset: imagens organizadas em diretórios `train/dog`, `train/not_dog`, etc.
![image](https://github.com/user-attachments/assets/c5a5bb5a-297f-46fa-b11a-52e1a05d433e)

 ##📊 Resultados
 A acurácia final pode variar dependendo do número de épocas e tamanho do dataset. Com poucas épocas e MobileNetV2 congelada, já é possível atingir bons resultados: 
 ![image](https://github.com/user-attachments/assets/c35cd389-771a-4c38-90af-a100ca931e06)

 ![image](https://github.com/user-attachments/assets/ce0856fb-cf79-4488-8d86-7a081f98a744)

 -resultados com `trainable`setado para TRUE ao inves de FALSE (descongelo os pesos e bias da mbV2):
 ![image](https://github.com/user-attachments/assets/17fffb68-284d-448d-a8ae-e18704b94cd0)
 ![image](https://github.com/user-attachments/assets/237d43f7-7fe3-4f6f-b6f0-02bd25a618e0)

 

passagem do teste unitario de imagem: img_path = '/content/drive/MyDrive/Colab Notebooks/teste/10936.jpg'
classe = "Gato" if prediction[0][0] > 0.5 else "Cachorro"
print(f"Predição: {classe} (score: {prediction[0][0]:.4f})")
![image](https://github.com/user-attachments/assets/7810f8db-861e-40cb-a94c-434f5c8b5307)



##📌 Objetivo
Este projeto faz parte de um estudo sobre classificação de imagens com redes neurais convolucionais, visando aplicações em visão computacional.
feito para estudo TCC, fique a vontade para dar um fork();

## 🚀 Como rodar
Fique a vontade para clonar meu repositorio, porém lembre-se te atualizar a estrutura do content sendo o meu: 
`drive.mount('/content/drive', force_remount=True)` para criar o ambiente e `caminho_dataset = '/content/drive/MyDrive/Colab Notebooks/dataset'` entrar nas pasta para dataset.



  
