Папка 'emoji' хранит 7 изображений смайликов соответстующих 7 основным эмоциям и список этих смайликов в виде numpy массивов. Сеть предсказывает число соответствующее одной из эмоций. Смайлик хранящийся под соответствующим индедксом отображается пользователю

Папка 'models' хранит экземпляры обученных моделей

Папка 'scripts' хранит файлы с кодом. Файл network хранит код обучения сети

Файл 'data_download_link.txt' хранит ссылку на данные хранящиеся на google drive, представленные в виде изображений и состоящие из 3 папок. Данные описывают 7 основных эмоций: 'anger', 'disgust', 'fear', 'happy', 'neutral', 'sad', 'surprise'. Папка test содержит 7 классов по 111 изображений. train 7 по 1000. val 7 по 3. Изображения в папках test и train одноканальные и равносторонние. Общий объем больше 100 мб
