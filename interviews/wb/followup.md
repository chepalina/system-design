23.10.2024
Проектирование маркетплейса
Команда Trust&Safety

Краткое впечатление: приятное интервью, интервьюер давал подсказки, указывал на ошибки в BoTEE (ошибки при подсчетах, не учтенные значения при расчете RPS), дополнительно указал на НФТ, которое я не уточнила (распределенность маркетплейса по регионам), давал коммуникацию что на текущем этапе все ок.


Ход собеседования: 
- Собрала ФТ
- Собрала НФТ
- Back of the envelope estimation
- Проработка первого ФТ
    - проговорила про saga паттерн
    - добавила очередь
    - проговорила exception flow
    - добавила сервис нотификаций при ошибках загрузки
    - поговорили про авторизацию (оставили за границей системы)
    - проговорила весь HP
 - Проработка второго ФТ
    - уточнила про рекомендации (оставили за границей системы)
    - наприсовала поисковик
    - наприсовала корзину (оставили за границей системы)
 - Перешли к детализации хранилища
     - определила сущности
     - определили модель основной сущности (Item)
     - обсудили варианты хранилища для картинок/текста
     - упомянула про масштабирование реляционных БД
     - попыталась определить критерии как выбрать тип БД (плохо) 

Что можно делать лучше: 
- считать BoTEE, проверять что влияет на объем данных (проговаривать до подсчета)
- определить критерии для выбора ХД
- четко проговорить сценарии использования ХД
- определить запись/чтение/стоит ли разделять
- РИСОВАТЬ ДЕТАЛИЗАЦИЮ по ХД ОТДЕЛЬНО (не использовать предыдущие схемы)
  
Не спросила а мб стоило: 
- Пиковая нагрузка

Мои вопросы: 
- Как в команде принимаются архитектурные решения

Что стоило спросить: 
- Что используется в WB в качестве поискового движка

