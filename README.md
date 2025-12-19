![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white)![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9A825.svg?style=for-the-badge&logo=googlecolab&logoColor=white)![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

## Autoencoder-OpenCV

В качества датасета будем использовать [этот](https://storage.yandexcloud.net/academy.ai/watermarked.zip). 

В данном примере я не стремился получить качественных выходных изображений, основная задача заключалась в том, чтобы показать принцип. Улучшить качество изображений помогут: расширение датасета на несколько порядков, применение более продвинутой аугментации (не только яркость и контрастность), увеличение размеров изображений, а также серия экспериментов со слоями автокодировщика. Однако ограничения бесплатного **Google Colab** не позволят нам получить высокого результата для данного датасета.

Архитектура модели достаточно сложна. Она включает слои **Conv2D**, **MaxPooling2D** и **UpSampling2D**.

В качестве финального результата выполняется предсказание на тестовых данных и отображение *10 примеров* для каждого из вариантов: *оригинал*, *с водяным знаком*, *предсказанное* и *шум* (разница).

> Рекомендую использовать **графический ускоритель T4** для работы с
> этим кодом
