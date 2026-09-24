Мы создали скрипт и в режиме терминала их проверим через команду nl(чтобы посмотреть по строкам)

<img width="630" height="204" alt="image" src="https://github.com/user-attachments/assets/dec2ec32-7530-4465-bc43-5a2832cc5b03" />

Содержимое юнит sistemd

<img width="612" height="270" alt="image" src="https://github.com/user-attachments/assets/7a5b95ed-d4dc-4c18-b7f7-cd1956c2ed9d" />

<img width="832" height="301" alt="image" src="https://github.com/user-attachments/assets/d9dab5e5-2e5c-46a0-9710-d9cdddcb7b22" />

Мы убедились в том что введённые ранее команды работают и статус службы это подтверждает.

<img width="469" height="203" alt="image" src="https://github.com/user-attachments/assets/1f1b8a8a-f71e-4dc8-b46f-fbca46c6ed85" />

Пояснение type=oneshot как дословно можно понять служба сработает только один раз, то есть она запускается и завершается.
А wanteby=multi-user.target где первая половина(является службой) привязывается к второй половине (цель) - это обеспечивает 
автозапуск в обычном режиме загрузки.
