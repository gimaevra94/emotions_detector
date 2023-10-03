Проект представляет из себя сверточную сеть. Сеть будет располагаться на PaaS-платформе Heroku. Принцип работы сети: пользователь переходит по ссылке и в открывшемся окне нажимает кнопку "предоставить доступ к вебкамере" или "загрузить изображение" если у пользователя не будет вебкамеры. В первом варианте сеть отображает пользователю изображение с вебкамеры. Сеть в реальном времени считывает кадры с вебкамеры и пропускает их через метод предсказания. Предсказание в виде смайлика соответствующего эмоции пользователя в реальном времени отображается в правом нижнем углу изображения с вебкамеры. Во втором варианте пользователь загружает в сеть изображение и получает предсказание в виде текста рядом с изображением. Нажатие клавиши 'Escape' останавливает процесс

Папка 'emoji' хранит 7 изображений смайликов соответстующих 7 основным эмоциям и список этих смайликов в виде numpy массива. Сеть предсказывает число соответствующее одной из эмоций. Смайлик хранящийся под соответствующим индедксом в numpy массиве отображается пользователю

Папка 'models' хранит экземпляры обученных моделей

Папка 'scripts' хранит файлы с кодом. Файл 'detector' хранит код запуска вебкамеры, предсказания на основе изображений с вебкамеры и вывода результата предсказания. В настоящий момент не работает. Файл network хранит код обучения сети. Файл 'test' будет преобразован в альтернативный вариант проверки работы сети с помощью загрузки изображений если у проверяющего не будет вебкамеры. В настоящий момент хранит код тестирования работы сети с помощью загрузки изображений

Файл 'data_download_link.txt' хранит ссылку на данные хранящиеся на google drive. Данные описывают 7 основных эмоций: 'anger', 'disgust', 'fear', 'happy', 'neutral', 'sad', 'surprise'. Данные представленны в виде изображений и состоят из 3 папок. Папка test содержит 7 классов по 111 изображений. train 7 по 1000. val 7 по 3. Изображения в папках test и train одноканальные и равносторонние. Общий объем больше 100 мб
