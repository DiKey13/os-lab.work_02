В данном отчёте будут рассмотрены ошибки в журнале.

<img width="910" height="498" alt="image" src="https://github.com/user-attachments/assets/e2f09a2b-6249-421e-bcef-5dbdc7e5de0f" />

<img width="750" height="529" alt="image" src="https://github.com/user-attachments/assets/7cd26567-895d-483f-9fe3-7172ae15fd73" />

<img width="753" height="517" alt="image" src="https://github.com/user-attachments/assets/382862ea-f84e-4f98-8acc-282cbb1bdbed" />

<img width="658" height="509" alt="image" src="https://github.com/user-attachments/assets/b7f73d86-a3d2-43aa-a1e4-dd47996a3ebc" />

Критичных ошибок при вводе команды journalctl -b -p err выявлено не было, но есть массовые предупреждения 
ihnoring duplicate name от dbus-broker. Так же ВМ может выдавать ложные ошибки об отсутствии какого либо железа или модуля
(ВМ не имеет своих модулей таких как Звук или интернет, а является своеобразной песочницей на уже имеющейся системе)

Для написания второго отчёта использовал команду journalctl -u plymouth-quit-wait.service
Что частично отсылает нас к разбору прошлого отчёта о загрузке

<img width="985" height="546" alt="image" src="https://github.com/user-attachments/assets/5a4d44e5-50f9-444d-a0dc-d2cc0bce5751" />

В ней можно наблюдать систематизированную задержку в 5 секунд обусловленную графической заставкой образа.
Критических ошибок нет.

<img width="761" height="803" alt="image" src="https://github.com/user-attachments/assets/31fc31ae-61e7-4d7b-9cb3-dbacdc9df0fb" />

В последнем разборе команды можно обратить на параметр perf это своего рода частота ядра. Сообщение неоднократно повторяется,
где мы можем наблюдать что она упирается в свой максимум в лимитах и частота снижается.
