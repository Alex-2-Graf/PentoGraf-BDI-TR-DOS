# PentoGraf-BDI-TR-DOS  
  
> [English](README.en.md) | [Русский](README.md)
>
> 
## Beta Disk Interface (TR-DOS) controller for PentoGraf. Supports up to 4 drives, onboard +12V DC-DC converter, Reset to Bank 0, and 2 PLL versions (FDC9216 / KR556RT4A).
  
---
  
Данный проект — это реализация БДИ для Пентографа, изначально убранного с основной платы.

## Ключевые особенности:
* Поддержка до 4 дисководов (A, B, C, D)
* Корректный сброс в нулевую банку ПЗУ
* Встроенный DC-DC преобразователь (+12 В)
* Светодиодная индикация питания (+5V, +12V) и активности диска
* А также совместимость с эмуляторами ВГ93.
  
---
  
# Варианты платы по ФАПЧ (PLL):  
  
---
  
## На базе чипа FDC9216B (стабильный цифровой сепаратор без настройки)  
  
[iBOM](Export/BDI%20PentoGraf%20(FDC9216B).html) [Схема](Export/BDI%20PentoGraf%20(FDC9216B).pdf) [Gerber](Gerber/BDI%20PentoGraf%20(FDC9216B)_Gerber.zip)  
  
![](Images/BDI%20PentoGraf%20(FDC9216B)_PCB.png)  
  
![](Images/BDI%20PentoGraf%20(FDC9216B)_BDI.png)  
  
![](Images/BDI%20PentoGraf%20(FDC9216B).jpg)  
  
---
  
## Классический вариант на ППЗУ КР556РТ4А (82S129) для работы с «тяжелыми» дискетами.  
  
[iBOM](Export/BDI%20PentoGraf%20(PT4A).html) [Схема](Export/BDI%20PentoGraf%20(PT4A).pdf) [Gerber](Gerber/BDI%20PentoGraf%20(PT4A)_Gerber.zip) [RT4](ROM/556RT4.bin)  
  
![](Images/BDI%20PentoGraf%20(PT4A)_PCB.png)  
  
![](Images/BDI%20PentoGraf%20(PT4A)_BDI.png)  
  
![](Images/BDI%20PentoGraf%20(PT4A).jpg)  
  
---
  
## Унификация  
  
Обе версии плат имеют идентичные габаритные размеры и расположение крепежных отверстий.  
Это позволяет легко заменять одну ревизию контроллера на другую в рамках одного корпуса.  
  
---
  
## Техническое примечание:  
  
Контроллеры разработаны для бесшовного (Plug-and-Play) подключения к моей версии плат:
  
* [PentoGraf-Pentagon-1024k](https://github.com/Alex-2-Graf/PentoGraf-Pentagon-1024k)

Но допустимо использование и с другими клонами по шине NEMO-bus
  
В качестве контроллера возможно использование [эмулятора ВГ93](https://github.com/Alex-2-Graf/VG93-MB8877-lgt8f328p-emulator)
  
При использовании исправных компонентов и качественной пайки настройка не требуется.  
  
---
  
## ⚖️ Лицензия / License  


Этот проект является открытым аппаратным обеспечением (Open Source Hardware). Графические материалы, схемы и топология печатной платы распространяются под лицензией **CERN OHL v2 Weak Reciprocal** (CERN-OHL-W-2.0).

Вы можете свободно распространять, модифицировать и производить это устройство при условии сохранения авторства **Alex-2-Graf** и публикации измененных исходных файлов платы под аналогичной открытой лицензией.
