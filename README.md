# Simple Archiver

Простая консольная утилита для сжатия и распаковки файлов и папок с использованием **Zstandard (zstd)** и **Bzip2 (bz2)**.
Поддерживает cжатие и распаковка файлов и директорий `.zst`, `.bz2`, `.tar.zst`, `.tar.bz2`, измерение скорости и коэффициента сжатия (`--benchmark`) 

## Использование

```bash
# Сжать файл или папку
python archiver.py -c <источник> <архив> [--progress] [--benchmark]

# Распаковать архив
python archiver.py -x <архив> <папка_назначения> [--progress]
```

## Примеры

```bash
python archiver.py -c myfolder data.tar.zst --progress
python archiver.py -x data.tar.bz2 output_dir --benchmark
```
