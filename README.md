## Big data student lab homework

 This python script analyze data from NYC taxi and limousine 
 commission and write it into csv files:  
 * gen_stat.csv - mean cost, longest ride, time of 10 min
  interval, which contain max amount of trips and amount of
  invalid rows  
 * missing_dates.csv - dates of invalid rows  
 * trip_stat.csv - month, average passenger count and mean
 trip duration
 * usage_stat.csv - trip count per day
 
 To launch this script launch main file with python and give file path via arguments.
   ```Shell    
  python main.py [-dir] file_paths   
  ```  
 If `-dir` then instead of file path use path to directory with csv files.  
  
  More data: https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page


#### Q&A:  
1) Тип источника данных в файле  
    * Данные пришли от водителей, их собрала TLC. Описани данных было указано,что она не гарантирует точности ээтих данных. Скорее всего данные будут "загрязнены".
2) Структурированы ли данные в файле?
    * Да, данные в файле структурированы. Количество категорий может меняться в зависимости от года сбора данных.
3) Какие возможны изменения в структуре данных, по-прежнему позволяющие человеку в них разобраться, но которые нарушат работоспособность программы?
    * Название колонок синонимани или сокращениями, другая расстановка слов, изменение заглавных букв, другой формат записи времени, название числовых значений строками и т.п
4) Придумать несколько дополнительных требований по обработке данных, не поддерживаемые программой на данный момент
    * Различная визуализация, загрузка данных из базы, вычисление различных статистических характеристик   