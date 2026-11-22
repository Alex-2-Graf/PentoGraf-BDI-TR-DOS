# PentoGraf-BDI-TR-DOS  
  
> [English](README.en.md) | [Русский](README.md)
>
> 
## Beta Disk Interface (TR-DOS) controller for PentoGraf. Supports up to 4 drives, onboard +12V DC-DC converter, Reset to Bank 0, and 2 PLL versions (FDC9216 / KR556RT4A).
  
Данный проект — это реализация БДИ для Пентографа изначально убранного с основной платы.

• Ключевые особенности: поддержка до 4 дисководов (A, B, C, D), корректный сброс в нулевую банку ПЗУ, встроенный DC-DC преобразователь (+12 В), светодиодная индикация питания (+5V, +12V) и активности диска, а также совместимость с эмуляторами ВГ93.

## Варианты платы (PLL):  
  
На базе чипа FDC9216B (стабильный цифровой сепаратор без настройки)
[iBOM](Export/BDI%20PentoGraf%20(FDC9216B).html) [Схема](Export/BDI%20PentoGraf%20(FDC9216B).pdf) [Gerber](Gerber/BDI%20PentoGraf%20(FDC9216B)_Gerber.zip)
  
![](Images/BDI%20PentoGraf%20(FDC9216B)_PCB.png)  
  
![](Images/BDI%20PentoGraf%20(FDC9216B)_BDI.png)  
  
![](Images/BDI%20PentoGraf%20(FDC9216B).jpg)  
  
Классический вариант на ППЗУ КР556РТ4А (82S129) для работы с «тяжелыми» дискетами.  
  
[iBOM](Export/BDI%20PentoGraf%20(PT4A).html) [Схема](Export/BDI%20PentoGraf%20(PT4A).pdf) [Gerber](Gerber/BDI%20PentoGraf%20(PT4A)_Gerber.zip) [RT4](ROM/556RT4.bin)
  
![](Images/BDI%20PentoGraf%20(PT4A)_PCB.png)  
  
![](Images/BDI%20PentoGraf%20(PT4A)_BDI.png)  
  
![](Images/BDI%20PentoGraf%20(PT4A).jpg)  
  
## Унификация  
  
Обе версий плат имеют идентичные габаритные размеры и расположение крепежных отверстий.  
Это позволяет легко заменять одну ревизию контроллера на другую в рамках одного корпуса.  
  
## Техническое примечание:  
  
Контроллеры разработаны для бесшовного (Plug-and-Play) подключения к моей версии плат:
  
* [PentoGraf-Pentagon-1024k](https://github.com/Alex-2-Graf/PentoGraf-Pentagon-1024k)

Но допустимо использование и с другими клонами по шине NEMO-bus
  
В качестве контролера возможно использование [эмулятора ВГ93](https://github.com/Alex-2-Graf/VG93-MB8877-lgt8f328p-emulator)
  
При использовании исправных компонентов и качественной пайки настройка не требуется.  

