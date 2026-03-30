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

Дополнительное задание для варианта 9: 
Добавить (или убрать, если они были в исходной сети) слои Dropoutи сравнить качество классификации до и после внесенных изменений. Подобрать параметр слоя Dropout для получения лучшей классификации тестовой выборки.
Объяснить полученные результаты.

=== Сравнение точности на тесте ===
Dropout 0.0: 0.8235
Dropout 0.2: 0.8576
Dropout 0.3: 0.8553
Dropout 0.5: 0.8541
Dropout 0.7: 0.8201

Лучший параметр Dropout: 0.2 с точностью 0.8576
Улучшение на 0.0341 (3.41%) по сравнению с базовой моделью.

Вывод: Dropout помогает бороться с переобучением, но при слишком высоком коэффициенте
(например, 0.7) может ухудшить точность. Оптимальное значение для данной архитектуры – 0.2
