本实验是通过配置不同的参数组合，找到表现最好的组合然后将这个参数组合应用在验证集C上。 
在代码中，首先analyse.ipynb文件处理了原始数据Data_Set_(A+B).xlsx和Data_Set_C.xlsx，通过公式将V2,V3算出. 
并保存为processed_(A+B)data.xlsx和processed_C_data.xlsx 
然后通过prepare_data.py进行数据处理，
将Type设置为目标特征 设置二分器（binary splitter），
保留Type=1，其他Type=2，3，4，5都变为0 
并将结果保存为train(A+B).csv和test_C.csv，
方便后面测试 train_(A+B)sorted.csv是排序后的数据，
将所有Type=1放在一起，Type=0放在一起 
Этот эксперимент настраивает различные комбинации параметров, находит наиболее эффективную комбинацию, а затем применяет эту комбинацию параметров к набору проверки C.
В коде сначала файл analyze.ipynb обрабатывает исходные данные Data_Set_(A+B).xlsx и Data_Set_C.xlsx и вычисляет V2 и V3 с помощью формулы.
И сохраняет их как processing_(A+B)data.xlsx и processing_C_data.xlsx
Затем prepare_data.py для обработки данных,
Установите Type на целевой признак и установите двоичный разделитель,
Сохраните Type=1, а другие Type=2, 3, 4, 5 все изменены на 0
И сохраните результаты как train(A+B).csv и test_C.csv,
для последующего тестирования train_(A+B)sorted.csv — это отсортированные данные,
Объедините все Type=1 вместе и Type=0 вместе
