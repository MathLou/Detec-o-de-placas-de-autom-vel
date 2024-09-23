# Detectar placas de carro
Neste repositório estudos de modelos são treinados com diferentes datasets de placas de automóvel com o objetivo de identificação de objetos para extrair features úteis de imagens e vídeos de carros.
![image](https://github.com/user-attachments/assets/1ca35e48-9070-4999-b72d-92b0885db0dc)
![image](https://github.com/user-attachments/assets/65e491b4-1c62-4f7a-8578-dea100867c82)
![image](https://github.com/user-attachments/assets/ef547461-21e6-4fbe-8e21-66b373a2ebf8)


Etapas: 
* Em Explorando_primeiro_dataset, são explorados as imagens e anotações de 433 dados, com o objetivo final de conversão das anotações para o formato YOLOV8.
* Em Modelo_v1 um modelo YOLOV8 é treinado e validado com o dataset anteriormente gerado. Este modelo não apresentou performance adequada para inferência, o que resultou na adoção de outro dataset com anotações já nativas do formato YOLOV8
* Em Modelo_v2, um dataset com mais qualidade é utilizado, o que por fim trouxe uma performance superior e adequada para inferências. O modelo final treinado esta no arquivo arquivo modelo_v2
* Por fim, como aplicações do modelo detector de placas de carro, em Obtendo_caracteres é utilizado o modelo_v2 com um modelo pré treinado OCR de identificação de caracteres para identificar caracteres nas placas detectadas. Resultados e imagens são mostradas e discutidas.
* em inferencia por video eta um script que pode ser rodado localmente para detecção de placas com o modelo_v2 em videos
