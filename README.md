# PentoGraf-BDI-TR-DOS  
  
> [English](README.en.md) | [Русский](README.md)
>
> 
## Beta Disk Interface (TR-DOS) controller for PentoGraf. Supports up to 4 drives, onboard +12V DC-DC converter, Reset to Bank 0, and 2 PLL versions (FDC9216 / KR556RT4A).
  
---
  
Контроллер БДИ для ПентоГрафа с поддержкой до 4 дисководов, встроенным DC-DC (+12 В), сбросом в нулевую банку и индикацией.

### Варианты ФАПЧ (PLL):
* **FDC9216B** (цифровой сепаратор): [iBOM](Export/BDI%20PentoGraf%20(FDC9216B).html) | [Схема](Export/BDI%20PentoGraf%20(FDC9216B).pdf) | [Gerber](Gerber/BDI%20PentoGraf%20(FDC9216B)_Gerber.zip)
* **КР556РТ4А (82S129)** (для «тяжелых» дискет): [iBOM](Export/BDI%20PentoGraf%20(PT4A).html) | [Схема](Export/BDI%20PentoGraf%20(PT4A).pdf) | [Gerber](Gerber/BDI%20PentoGraf%20(PT4A)_Gerber.zip) | [RT4](ROM/556RT4.bin)

*Иллюстрации плат, схем и сборок доступны в соответствующих папках репозитория (`Images/`).*
  
---
  
## Унификация и совместимость  
  
Обе версии плат имеют идентичные габариты и крепеж для взаимозаменяемости. Разработаны для [PentoGraf-Pentagon-1024k](https://github.com) (совместимы с NEMO-bus). Поддерживают [эмулятор ВГ93](https://github.com). При качественной сборке настройка не требуется.
