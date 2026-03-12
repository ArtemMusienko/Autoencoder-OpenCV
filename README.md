![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white)![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9A825.svg?style=for-the-badge&logo=googlecolab&logoColor=white)![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

## Autoencoder-OpenCV

[![ru](https://img.shields.io/badge/README_на_русском-2A2C39?style=for-the-badge&logo=github&logoColor=white)](README.ru.md)

As a dataset, we will use [this](https://storage.yandexcloud.net/academy.ai/watermarked.zip).

In this example, I was not trying to get high-quality output images, the main task was to show the principle. Image quality can be improved by expanding the dataset by several orders of magnitude, using more advanced augmentation (not only brightness and contrast), increasing image size, as well as a series of experiments with autoencoder layers. However, the limitations of the free **Google Colab** will not allow us to achieve a high result for this dataset.

The model architecture is quite complex. It includes **Conv2D**, **MaxPooling2D**, and **UpSampling2D** layers.

As a final result, the model is trained on the test data and displays *10 examples* for each of the following options: *original*, *watermarked*, *predicted*, and *noise* (difference).

> I recommend using the **T4 graphics accelerator** to work with
> this code