# msh
bash скрипт для параллельного запуска заданий

Используйте 

$ msh файл-с-заданиями число-процессов

Пример

$ msh tasks.sh 10

Файл с заданиями должен содержать по одному заданию на каждой строчке (задание это bash однострочник), msh запускает указанное число процессов (в примере 10) каждый процесс берёт по строчке, и запускает задание. После окончания задания процесс берёт следующее ещё никем не взятое ранее задание. После окончания процессов msh завершается.

bash script to run jobs in parallel

Use

$ msh job-file number-of-processes

Example

$ msh tasks.sh 10

The task file should contain one task on each line (the task is a bash one-line), msh starts the specified number of processes (in example 10), each process takes a line, and starts the task. After the end of the task, the process takes the next task that has not yet been taken by anyone. After the processes terminate, msh exits.
