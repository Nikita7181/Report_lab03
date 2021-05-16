#           **Отчет Lab02**
##                *Report*
- `Ход работы`

![Домашняя работа](https://github.com/Nikita7181/lab03)

![](https://raw.githubusercontent.com/Nikita7181/Report_lab03/master/Screenshots/1.png)

![](https://raw.githubusercontent.com/Nikita7181/Report_lab03/master/Screenshots/2.png)

![](https://raw.githubusercontent.com/Nikita7181/Report_lab03/master/Screenshots/3.png)

![](https://raw.githubusercontent.com/Nikita7181/Report_lab03/master/Screenshots/4.png)

![](https://raw.githubusercontent.com/Nikita7181/Report_lab03/master/Screenshots/5.png)

### *Homework*
 - Создаем новую дерикторию и клонируем репрезетоий 
```
mkdir timp_lab03
cd timp_lab03
git clone https://github.com/tp-labs/lab03.git .
rm -rf CMakeLists.txt
rm -rf preview.png
rm -rf LICENSE
rm -rf README.md
git remote remove origin
git remote add origin https://github.com/Nikita7181/Report_lab03.git
```
-В папке formatter_lib был создан файл CMakeLists.txt

```
cd /formatter_lib
touch CMakeLists.txt
nano CMakeLists.txt 
```

![](https://raw.githubusercontent.com/Nikita7181/Report_lab03/master/Screenshots/6.png)

- Создаем папку, в котором собираем проект _build

```
mkdir _build
cd _build
cmake ..
cmake --build .
```

В папке formatter_ex_lib был создан файл CMakeLists.txt

```
cd /formatter_ex_lib
touch CMakeLists.txt
nano CMakeLists.txt 
```

![](https://github.com/Nikita7181/Report_lab03/blob/master/Screenshots/7.png)

- Создаем папку, в котором собираем проект _build

```
mkdir _build
cd _build
cmake ..
cmake --build .
```

В папке hello_world_application был создан файл CMakeLists.txt

```
cd /hello_world_application
touch CMakeLists.txt
nano CMakeLists.txt 
```

![](https://raw.githubusercontent.com/Nikita7181/Report_lab03/master/Screenshots/8.png)

- Создаем папку, в котором собираем проект _build

```
mkdir _build
cd _build
cmake ..
cmake --build .
```

В папке solver_applicatio был создан файл CMakeLists.txt

```
cd /solver_applicatio
touch CMakeLists.txt
nano CMakeLists.txt 
```

![](https://raw.githubusercontent.com/Nikita7181/Report_lab03/master/Screenshots/9.png)

- Создаем папку, в котором собираем проект _build

```
mkdir _build
cd _build
cmake ..
cmake --build .
```
- После чего все было выгружено на Git hub 

```
cd /home/nikita/Nikita7181/workspace/projects/Report_lab03
git add .
git commit -m "Complete tasks"
git push origin master
```
