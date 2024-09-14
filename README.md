# Wagon Number Detection

## Описание

Проект предназначен для автоматического обнаружения и распознавания номеров вагонов на изображениях и видео с использованием модели YOLOv5.

## Установка

1. **Клонируйте репозиторий**:

   ```bash
   git clone https://github.com/ArtyomPass/wagon-number-detection.git

2. **Перейдите в директорию проекта:**:

   ```bash
   cd wagon-number-detection

3. **Установите зависимости:\:**:

   ```bash
   pip install -r requirements.txt

## Использование

1. **Обнаружение на изображении:**:

   ```bash
   python detect.py --source path/to/your/image.jpg


2. **Обнаружение на видео:**:

   ```bash
   python detect.py --source path/to/your/video.mp4

3. **Обнаружение с веб-камеры:**:

   ```bash
   python detect.py --source 0


## Обучение модели (при необходимости)

Подготовьте датасет в формате, совместимом с YOLOv5.
Измените файл конфигурации data.yaml для указания путей к вашему датасету.
Запустите обучение:

   ```bash
   python train.py --img 640 --batch 16 --epochs 50 --data data.yaml --weights yolov5s.pt
