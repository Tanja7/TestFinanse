
# Менеджер личных финансов

Это серверное мавен-приложение, играющее роль **менеджера личных финансов**. 
У приложения в корневой папке находится текстовый файл *categories.tsv*, 
категоризирующий название каждой покупки.

На сервер приходят запросы с информацией о покупке: наименование, 
дата покупки и сумма (дата в формате: "год.месяц.число").

Если названия покупки в файле категорий нет, то она относится к категории "другое".

Результатом работы приложения является получение **максимальной по абсолютным тратам категории** за весь период,
а также за год, месяц и день сохранённой покупки.