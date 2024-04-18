# Обучение модели семантической сегментации SegFormer 

В данной практике я обучил модель SegFormer на предоставленном мне датасете фотографий машин сбоку и масок для данных фотографий. Маски классифицируют части машины такие как окна, корпус, фары. 

В результате обучения на протяжении 200 эпох были получены веса модели которые можно загрузить в саму модель чтобы сегментировать изображения машин сбоку вне датасета. Мною было скачано больше тысячи картинок машин сбоку из интернета для проверки модели на новом сете изображений.

Узнать больше о модели SegFormer на HuggingFace:  

[![Model on HF](https://huggingface.co/datasets/huggingface/badges/resolve/main/model-on-hf-sm.svg)](https://huggingface.co/docs/transformers/model_doc/segformer)

### Установка зависимостей  

```sh
pip install -r requirements.txt
```

###  Файлы в репозитории

| Название файла | Описание | Открыть в Google Colab |
| --- | --- | --- |
| model_finetune.ipynb | Обучение модели на датасете | [![Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Podjob/CarSegmentation/blob/main/model_finetune.ipynb) |
| download_images.ipynb | Программа скачки изображений с интернета | [![Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Podjob/CarSegmentation/blob/main/download_images.ipynb) |
|apply.ipynb | Применение обученной модели на скачанных изображениях | [![Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Podjob/CarSegmentation/blob/main/apply.ipynb) |

## Пример результата обучения 

### Изображение с интернета 

![](https://i.ibb.co/SvLcK1K/car.png) 

### Маска сегментации полученная после обучения модели 

![](https://i.ibb.co/tZc305C/mask.png)
