# Buzzer-orchestra
Create your own orchestra of piezo buzzers, some wires and 555 microchip
<img width="2782" height="1566" alt="image" src="https://github.com/user-attachments/assets/4b6dc920-77db-4530-bae2-fab3d841f125" />


## Содержание
[Компоненты](#компоненты)  
[Первоначальная сборка](#первоначальная-сборка)  
[Настройка частоты сигнала](#настройка-частоты-сигнала)  
[Подготовка печатной платы](#подготовка-печатной-платы)
[Подготовка корпуса и сборка](#подготовка-корпуса-и-сборка)

## Компоненты
<details>
  <summary>Нажмите, чтобы раскрыть</summary>
  
  - Таймер NE555;
  - Пьезоэлектрический излучатель;
  - Резисторы 50-80 Ом, 1кОм, 10кОм;
  - Конденсаторы 10нФ, 100нФ;
  - Потенциометр 10кОМ;
  - Тактовая кнопка;
  - Литий-ионный аккумулятор 18650 и батарейный отсек;
  - Соединительные провода.
</details>

## Первоначальная сборка
<details>
  <summary>Нажмите, чтобы раскрыть</summary>
  
  1. Перед началом сборки необходимо было проверить работоспособность пьезоэлектрического излучателя (пищалки). Для этого мы припаяли к нему провода:
  <img width="4032" height="2268" alt="PXL_20261009_114828676" src="https://github.com/user-attachments/assets/28dc6174-21fc-4245-b53c-8324d49d8b4e" />
  <img width="4032" height="2268" alt="PXL_20261009_115053528" src="https://github.com/user-attachments/assets/034aaa75-75d4-46e9-8d62-d3fcc000d586" />
  <img width="4032" height="2268" alt="PXL_20261009_115745591" src="https://github.com/user-attachments/assets/2cef24b8-dd29-4695-9fac-dd58e91bb333" />
  И при помощи генератора сигналов подали на него ШИМ-сигнал с квадратной формой волны, амплитудой 5В, частотой 311,11Гц и шириной 90%:
  
  https://github.com/user-attachments/assets/6ae5d274-33ae-4b5a-9b0c-a80e4de3d9dc
  
  Как выглядит данная цифровая волна на осциллографе: 
  <img width="4032" height="2268" alt="PXL_20261009_120339695" src="https://github.com/user-attachments/assets/c584483c-c546-4963-b25c-d33b7dd30240" />
  2. После успешной проверки приступили к размещению всех элементов на сборочной плате, согласно схеме:
  <img width="1911" height="1080" alt="photo_2026-11-25_12-53-47" src="https://github.com/user-attachments/assets/a6740dfc-ad18-4b1d-a0ea-98affaa952b8" />
  <img width="2948" height="2002" alt="image" src="https://github.com/user-attachments/assets/5c04cc7c-e68d-49c8-8290-873ec77959e9" />
  И протестировали:
  
  https://github.com/user-attachments/assets/d3b6e001-2eed-44be-8ab6-4ef780d44314

</details>

## Настройка частоты сигнала
<details>
  <summary>Нажмите, чтобы раскрыть</summary>

  Для настройки частоты сигнала, а также для подбора величины резисторов и конденсаторов можно воспользоваться [данным сайтом](https://overcme.github.io/Calculator-555/).  
  _Мы же в своём устройстве ограничились использованием компонентов приведенных в начале, так как такой набор удовлетворяет нашим потребностям, предоставляя выходной сигнал в диапазоне от ~500Гц до ~1000Гц._  
  Мы подключили осциллограф к контактам пищалки, чтобы анализировать частоту выходного сигнала (данная частота соответствует частоте звукового сигнала, испускаемого нашим устройством). Далее при помощи потенциометра и показаний осциллографа подобрали частоту 698Гц, соответствующую музыкальной ноте Фа второй октавы (F5) в стандартном строе.
</details>

## Подготовка печатной платы
<details>
  <summary>Нажмите, чтобы раскрыть</summary>
  1. Лист стеклотекстолита с медным покрытием покрываем акриловой краской.
  2. После высыхания удаляем краску с ненужных областей, оставляя только области под будущие дорожки. Для этого отправляем плату на лазерный станок и гравируем её по предварительно настроенному шаблону.
  <img width="4032" height="2268" alt="PXL_20261016_110904150" src="https://github.com/user-attachments/assets/65cca3f6-138c-4e9f-8776-dda144930bed" />
  
https://github.com/user-attachments/assets/7a8a9a43-6899-434c-8da1-acf9cda63a21

<img width="4032" height="2268" alt="PXL_20261016_111510466" src="https://github.com/user-attachments/assets/7fa622ea-38a2-42a2-97b9-7ec0a4fcce2e" />
Стираем остатки краски при помощи спирта:

https://github.com/user-attachments/assets/1804bd56-5969-42c7-9163-892bd23dfa9a

3. Далее приступаем к  процессу травления.
   Подготавливаем раствор:
   - Лимонная кислота 15г
     <img width="4032" height="2268" alt="PXL_20261016_103444342" src="https://github.com/user-attachments/assets/50d85a84-517c-4fe4-bf0e-bcc3933f428c" />
   - Соль пищевая 2,5г
     <img width="4032" height="2268" alt="PXL_20261016_103711447" src="https://github.com/user-attachments/assets/b96f1efe-45d8-4879-8c01-ddca31cdd216" />
   - Пероксид водорода 50мл
     <img width="4032" height="2268" alt="PXL_20261016_103852680" src="https://github.com/user-attachments/assets/1c802175-85a7-498a-93f3-307a9d0e18c2" />  

Всё перемешиваем:
  <img width="4032" height="2268" alt="PXL_20261016_104217456" src="https://github.com/user-attachments/assets/49834ec7-ee6c-4ccb-9b86-e543b0a38255" />
  Помещаем туда плату. Также используем ванночку с подогретой водой (40°-60°) и постоянно помешиваем смесь для ускорения реакции.

  https://github.com/user-attachments/assets/50bc97e5-6d4f-47d2-8b71-b93aee4d1e20

  В итоге вся медь с поверхности должна перейти в раствор:
  <img width="4032" height="2268" alt="PXL_20261016_114216528" src="https://github.com/user-attachments/assets/1441e4f5-80a1-4bba-b74e-450a3ef63a58" />
  <img width="960" height="1280" alt="photo_5_2026-11-25_12-51-27" src="https://github.com/user-attachments/assets/cbdb7e63-de38-4872-b1c5-899e91402572" />
4. На плате осталась краска, которой покрыты дорожки. Удаляем её при помощи ацетона. Получаем медные дорожки:
<img width="2268" height="4032" alt="PXL_20261016_120239452" src="https://github.com/user-attachments/assets/72b4abdc-0c17-483f-ac38-4abd1d1ff30c" />
5. Сверлим отверстия в плате для установки компонентов и крепежей:
<img width="2268" height="4032" alt="PXL_20261023_104949198" src="https://github.com/user-attachments/assets/835d82de-3c5f-4fb6-a718-4a338e4e141a" />
6. Соединяем плату винтами и гайками с заготовленным деревянным шаблоном. Ориентируясь на шаблон срезаем лишний текстолит канцелярским ножом, доводим поверхности и скругляем углы при помощи наждачной бумаги:
<img width="2268" height="4032" alt="PXL_20261023_113320105" src="https://github.com/user-attachments/assets/27033a19-a1c4-4b47-8e1c-52e2afab7e81" />
<img width="4032" height="2268" alt="PXL_20261023_113518155" src="https://github.com/user-attachments/assets/aa37f53d-9863-4bc1-92ea-581c5aa85e1e" />
Получившаяся плата:
<img width="2356" height="1326" alt="image" src="https://github.com/user-attachments/assets/b52fd7b8-6e95-430e-acd6-504926d0fc14" />
7. Покрываем обратную сторону акриловой краской:
<img width="1875" height="1054" alt="image" src="https://github.com/user-attachments/assets/af69d8ca-4cab-4c75-809e-32fe65bfced3" />
8. После высыхания проводим гравировку:

https://github.com/user-attachments/assets/2a127d88-3ee5-4c89-8d68-fed89d4112da

9. Припаиваем все электронные компоненты к плате:
<img width="4032" height="2268" alt="PXL_20261030_112814444" src="https://github.com/user-attachments/assets/2bd14b48-f873-414e-b185-f2b430c313a9" />
Подготовка платы завершена.
</details>

## Подготовка корпуса и сборка
<details>
  <summary>Нажмите, чтобы раскрыть</summary>
  Корпус печатаем на 3д-принтере из PLA пластика:
  <img width="4032" height="2268" alt="PXL_20261023_115157398" src="https://github.com/user-attachments/assets/4f4eec20-47f8-4219-8b53-d68b0825954b" />

  https://github.com/user-attachments/assets/dea23407-06bd-418b-9ed2-72dbb67024f0

  Помещаем плату в корпус, закрываем акриловым стеклом, соединяем две половинки корпуса саморезами:
  <img width="1280" height="960" alt="photo_7_2026-11-25_12-51-27" src="https://github.com/user-attachments/assets/a6e381b6-d49c-44bd-b063-274fe10328f1" />
  Приклеиваем батарейный отсек к нижней части корпуса:
  <img width="2452" height="1880" alt="image" src="https://github.com/user-attachments/assets/bf3c8bc7-88ab-425f-95db-28e51ee1cf38" />
  Готовый однонотный синтезатор:
  <img width="1832" height="1031" alt="image" src="https://github.com/user-attachments/assets/5d14e3c9-7d1f-4b3f-ae9e-1735ea01cf1e" />
</details>
