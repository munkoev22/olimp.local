# olimp.local
Информационная система для организации образовательных мероприятий для школьников
<a target="_balnk" href="http://events.bsu.ru/index.php?r=/event/events/">events.bsu.ru</a>
<h2 dir="auto"><a id="user-content-описание-проекта" class="anchor" aria-hidden="true" href="#описание-проекта"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Описание проекта</h2>
Проект разработан по заказу Бурятского государственного университета имени Доржи Банзарова. 
Использование информационной системы позволит облегчить и частично автоматизировать организацию образовательных мероприятий. Использование информационной системы позволит участникам удаленно регистрироваться на мероприятия. Информационная система имеет систему единых аккаунтов, что позволит отслеживать участия школьников в образовательных мероприятиях, а также получать список потенциальных студентов. Также использование информационной системы позволит минимизировать время формирования плана размещения участников по аудиториям и рассылки информации участникам.

<h2 dir="auto"><a id="user-content-описание-проекта" class="anchor" aria-hidden="true" href="#описание-проекта"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg><h2>Модели системы</h2>

  <ul>
    <li><code>Login</code>  реализует функционал аутентификации и авторизации пользователей</li>
    <li><code>User</code> реализует функционал изменения статусов и паролей пользователей.</li>
    <li><code>Status</code> реализует функционал по добавлению и обработке статусов пользователей.</li>
    <li><code>Attrbute</code> реализует функционал управления дополнительными атрибутами для регистрации на мероприятие.</li>
    <li><code>AttributeValue</code> реализует функционал управления дополнительными атрибутами для регистрации на мероприятие.</li>
    <li><code>Aud</code> реализует функционал управления аудиториями.</li>
    <li><code>Event</code> реализует функционал управления мероприятиями.</li>
    <li><code>Log</code> реализует функционал управления действиями пользователя.</li>
    <li><code>Mailer</code> реализует функционал рассылки информации пользователям.</li>
    <li><code>UserInfo</code> реализует функционал управления данными участников.</li>
  </ul>
  
<h2 dir="auto"><a id="user-content-описание-проекта" class="anchor" aria-hidden="true" href="#описание-проекта"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg><h2>Роли системы</h2>
  <ul>
    <li><code>Guest</code> все пользователи сети Интернет, не прошедшие авторизацию. Гости могут просматривать расписание.</li>
    <li><code>Member</code> пользователи системы, которые могут регистрироваться на мероприятия. Пользователь с ролью «Участник» может зарегистрироваться на мероприятия и заполнять персональные данные.</li>
    <li><code>Organizer</code> пользователь системы, который может проводить мероприятия. Для этого Администратор должен назначить им роль «Организатор». Организаторами могут быть как студенты, так и преподаватели.</li>
    <li><code>Administrator</code> пользователь, который выполняет управляющую роль в системе. Администратору доступен весь функционал системы.</li>
  </ul>


Система хранит информацию о мероприятиях <code>Events</code> и пользователях системы <code>User, UserInfo</code>, аудиториях <code>Aud</code>.
Для участника:
Система позволяет удаленно регистрироваться на мероприятия, для этого создать аккаунт в системе и заполнить персональные данные.
Система оповещает участников об изменении статуса регистрации.
