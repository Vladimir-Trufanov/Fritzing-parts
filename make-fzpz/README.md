# [make-fzpz](https://github.com/mpilgrem/make-fzpz)

## Introduction

The [Fritzing](http://fritzing.org/home/) software tool allows users to document
their electronics prototypes, including by creating their own parts.

***Программное средство [Fritzing](http://fritzing.org/home/) позволяет пользователям документировать свои прототипы электроники, в том числе путем создания собственных деталей
***

This project seeks to provide Windows tools to create a bundle (\*.fzpz) file
from a part metadata (\*.fzp) file and its associated vector graphics (\*.svg)
files.

***Этот проект направлен на предоставление инструментов Windows для создания файла пакета (\*.fzpz) из файла метаданных части (\*.fzp) и связанных с ним файлов векторной графики (\*.svg)***

The tools assume that the metadata file is in subdirectory `\part` and the
vector graphics files are in subdirectories of subdirectory `\svg`.

***Инструменты предполагают, что файл метаданных находится в подкаталоге "/part", а файлы векторной графики находятся в подкаталогах подкаталога "/svg"***.


## Bundle file format

The format of the bundle file is a zip file containing the metadata file and
associated vector graphics files. The name of the metadata file begins `part.`.
The name of each vector graphics file begins `svg.<view>.`, where `<view>` is
one of icon, breadboard, schematic and pcb.


***Формат файла пакета - это zip-файл, содержащий файл метаданных и связанные с ним файлы векторной графики. Имя файла метаданных начинается с "part.". Название каждого файла векторной графики начинается с "svg.<вид>.", где "<вид>" - это один видов:   icon, breadboard, schematic and pcb.***

## Windows PowerShell Version 4 or higher

`make-fzpz.ps1` is a Windows PowerShell script, requiring version 4.0 or higher.
Specifically, it makes use of the `System.IO.Compression.ZipFile` class provided
by .NET Framework 4.5 or higher.

## Windows batch file

make-fzpz.bat  is a Windows batch file. It reqires application
[7-Zip](http://www.7-zip.org/) (`7z.exe`) to be in the path.

***make-fzpz.bat - это командный файл Windows. Для него требуется, чтобы в пути было указано приложение [7-Zip](http://www.7-zip.org/) (7z.exe).***


## [Оригинальный 7z.exe Игоря Павлова](https://originaldll.com/file/7z.exe/30125.html)

2024.02.15 удалось отработать bat-файл с помощью данного экземпляра [7z.exe](7z/7z.exe).

```
Category:            Open Server
Description:         7-Zip Console
File size:           296 Kb
File date:           18.04.2011 23:35
File version:        9.22 beta
Internal name:       7z
Original file name:  7z.exe
Product name:        7-Zip
Product version:     9.22 beta
Company name:        Igor Pavlov
```
