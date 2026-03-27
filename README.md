# CIFAR_10_Smirnova
ЗИТ-24м. Практика 3. Вариант 9. Для БД CIFAR-10 – полноцветных изображений реальных объектов создать архитектуру сверточной НС с наименьшим числом нейронов, достаточных для правильной классификации изображений тестовой выборки на уровне не менее 92%. Обучить НС с контролем эффекта переобучения путем использования выборки валидации.

<img width="1200" height="400" alt="training_curves" src="https://github.com/user-attachments/assets/7fec166a-d66d-4d66-9765-4fcc51d947b3" />
![1](https://github.com/user-attachments/assets/05c259f7-9bd2-4c9f-b025-7ef3534d0ac4)
![2](https://github.com/user-attachments/assets/ac8de05b-8500-4926-85dc-f80359217300)
![3](https://github.com/user-attachments/assets/d4e62f5a-2366-41de-afea-c79d172e46c4)

Обучение завершено за 117.6 минут.

Точность на тестовой выборке (без Dropout): 0.8348
Условие не выполнено. Рекомендуется увеличить количество эпох или добавить аугментацию.
WARNING:absl:You are saving your model as an HDF5 file via `model.save()` or `keras.saving.save_model(model)`. This file format is considered legacy. We recommend using instead the native Keras format, e.g. `model.save('my_model.keras')` or `keras.saving.save_model(model, 'my_model.keras')`.
Модель сохранена как 'cifar10_best_model.h5'.
Графики сохранены как 'training_curves.png'.

