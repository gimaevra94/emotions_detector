Проект представляет из себя сверточную сеть классифицирующую эмоции. Принцип работы сети: открывается окно в котором пользователь видит трансляцию с камеры своего компьютера. Программа в реальном времени считывает кадры с камеры и пропускает их через метод предсказания. Предсказание в виде смайлика соответствующего эмоции пользователя в реальном времени отображается в правом нижнем углу трансляции с камеры. Нажатие клавиши 'escape' останавливает процесс

Запустить тестирование работы обученной сети можно только на локальном компьютере так как библиотека cv2 с помошью которой реализовалась функция трансляции с камеры не работает на удаленных серверах. Чтобы запустить тестирование необходимо скачать скачать папку 'test' и запустить файл 'test.ipynb'. Раскомментировать установку библиотек в случае ошибки при запуске. Чтобы запустить саму сеть нужно открыть [ссылку](https://colab.research.google.com/github/gimaevra94/emotions_detector/blob/main/train.ipynb) и нажать 'ctrl+enter'

Папка 'test' хранит код запуска камеры, предсказания на основе изображений с камеры и вывода результата предсказания, смайлики соответствующие эмоциям в виде массива и обченную модель сети

'data.zip' хранит архивы с данными. Данные поделены на папку 'train' хранящую 6 классов по 3171 изображений и 'test 6 по 831. Изображения являются одноканальными и равносторонними

'train.ipynb' хранит код обучения сети
