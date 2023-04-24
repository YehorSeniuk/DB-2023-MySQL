# DB-2023-MySQL

<div class="container">
  
  <div class="content">
  <h2>Короткий зміст</h2>
  <ol >
    <li><a href="#section1"> Інсталяція MySQL Server, MySQL Workbench з використанням MySQL Universal Installer 🐬</a></li>
    <li><a href="#section2"> Елементарні операції побудови реляційної схеми в MySQL Workbench 🛠</a></li>
    <li><a href="#section3"> Базові поняття 🖇</a></li>
    <li><a href="#section4"> Приклад ствоерння реляційної схеми з використанням MySQL Workbench на основі ER-моделі 🔍</a></li>
    <li><a href="#section5"> Автогенерація DDL з використанням MySQL Workbench ⚙️</a></li>
	<li><a href="#section6"> Корисні посилання 🔗</a></li>
  </ol>
  </div>
  <div class="intro">
	<h2>Вступ</h2>
	<p>Це гайд на тему "Інсталяція через MySQL Universal Installer. Встановлення MySQL Server, MySQL Workbench. Створення реляційної схеми та автогенерація DDL за допомогою MySQL Workbench". Нище наведені позначення які будуть використовуватся в гайді.
	</p>
	<div class="recomendation">
		<h4>💡 Рекомендація</h4>
		<p>Містить приклади застосування, поради як краще скористатися даним інструментом.</p>
	</div>
	<div class="dangerous">
		<h4>⛔ Застереження</h4>
		<p>Містить обмеження, яких необхідно дотримуватися.</p>
	</div>
	<div class="playlist">
		<h4>📹 Відеоматеріал</h4>
		<p>Відсилка на відеоматеріал.</p>
	</div>
  </div>
</div>

<!-- Раздел 1 -->
<div class="section" id="section1">
  <h3>1. Інсталяція MySQL Server, MySQL Workbench з використанням MySQL Universal Installer 🐬</h3>
  <details>
   <summary>MacOS</summary>
  <p><span class="two">1.1</span> Запускаємо інсталяційний пакет</p>
  <img src="image/Install/MacOS/1_1.jpg"/>
  <p><span class="two">1.2</span> Після запуску одразу побачимо попередження, нажимаємо кнопку «Дозволити»</p>
  <img src="image/Install/MacOS/1_2.jpg"/>
  <p><span class="two">1.3</span> Бачимо коротенький вступ, нажимаємо «Продовжити»</p>
  <img src="image/Install/MacOS/1_3.jpg"/>
  <p><span class="two">1.4</span> Після вступу читаємо ліцензію угоду програми. Ми друкувати чи зберігати її не будемо, тому нажимаємо кнопку «Продовжити»</p>
  <img src="image/Install/MacOS/1_4.jpg"/>
  <p><span class="two">1.5</span> Після того, як натиснули кнопку,  погоджуємось з ліцензійними угодами, нажавши кнопку «Погоджуюсь»</p>
  <img src="image/Install/MacOS/1_5.jpg"/>
  <p><span class="two">1.6</span> Після згоди, інсталюємо пакет, обов’язково слідкуємо, щоб було вільне місце
Можем також змінити місце інсталювання( за умовчуванням  «Для всіх користувачів на цьому компʼютері»)</p>
  <img src="image/Install/MacOS/1_6.jpg"/>
  <p><span class="two">1.7</span> При натиснені кнопки «Змінити місце інсталяції»</p>
  <img src="image/Install/MacOS/1_7.jpg"/>
  <p><span class="two">1.8</span> Для інсталяції нам необхідно або ввести пароль від компʼютера або використати Touch ID</p>
  <img src="image/Install/MacOS/1_8.jpg"/>
  <p><span class="two">1.9</span> Обираємо  Use Strong Password Encryption, нажимаємо кнопку «Next»</p>
  <img src="image/Install/MacOS/1_9.jpg"/>
  <p><span class="two">1.10</span> У полі нам необхідно вигадати та ввести пароль, який ми будемо подальшому використовувати</p>
  <img src="image/Install/MacOS/1_10.jpg"/>
  <p><span class="two">1.11</span> Після введення, завершуємо інсталяцію, кнопка «Finish»</p>
  <img src="image/Install/MacOS/1_11.jpg"/>
  <p><span class="two">1.12</span> І знову для завершення необхідно або пароль від компʼютера або Touch ID</p>
  <img src="image/Install/MacOS/1_12.jpg"/>
  <p><span class="two">1.13</span> Все, інсталяція успішно завершилася, бачимо повідомлення про це, нажимаємо кнопку «Закрити»</p>
  <img src="image/Install/MacOS/1_13.jpg"/>
  <p><span class="two">1.14</span> Для того щоб перевірити, чи точно все успішно інсталювало, нам необхідно перейти в налаштування, знайти в кінці MySQL
Якщо виконали все правильно, то кружечки будуть горіти зеленим, як на фото</p>
  <img src="image/Install/MacOS/1_14.jpg"/>
  <p><span class="two">1.15</span> Переходимо в Термінал
Пишемо команду mysql -u root -p
Після запуску, вводимо пароль, який ми записували декілька пунктів вище</p>
  <img src="image/Install/MacOS/1_15.jpg"/>
  <p><span class="two">1.16</span> Після виконання цих дій, ми можем працювати з MySQL!</p>
  <img src="image/Install/MacOS/1_16.jpg"/>
  </details>
  <details>
   <summary>Windows</summary>
  <p><span class="two">1.1</span> Запускаємо інсталяційний пакет</p>
  <img src="image/Install/Windows/1_1.png"/>
  <p><span class="two">1.2</span> Обираємо «Custom» та нажимаємо кнопку «Next»</p>
  <img src="image/Install/Windows/1_2.png"/>
  <p><span class="two">1.3</span> Обираємо MySQL Server та нажимаємо на зелену стрілку вправо</p>
  <img src="image/Install/Windows/1_3_1.png"/>
  <img src="image/Install/Windows/1_3_2.png"/>
  <p><span class="two">1.4</span> Додоємо MySQL Workbench тієї ж версії</p>
  <img src="image/Install/Windows/1_4.png"/>
  <p><span class="two">1.5</span> Додоємо MySQL Documentation (за бажанням) За бажанням можна також додати Samples and Examples (у вкладці Documentation)</p>
  <img src="image/Install/Windows/1_5.png"/>
  <p><span class="two">1.6</span> Нажимаємо кнопку «Next»</p>
  <img src="image/Install/Windows/1_6.png"/>
  <p><span class="two">1.7</span> Натискаємо «Execute». Після повного завантаження натискаємо «Next»</p>
  <img src="image/Install/Windows/1_7_1.png"/>
  <img src="image/Install/Windows/1_7_2.png"/>
  <img src="image/Install/Windows/1_7_3.png"/>
  <p><span class="two">1.8</span> Натискаємо «Execute» та чекаємо інсталяції</p>
  <img src="image/Install/Windows/1_8_1.png"/>
  <img src="image/Install/Windows/1_8_2.png"/>
  <img src="image/Install/Windows/1_8_3.png"/>
  <p><span class="two">1.9</span> Нажимаємо кнопку «Next»</p>
  <img src="image/Install/Windows/1_9.png"/>
  <p><span class="two">1.10</span> В Config Type обираємо Development Computer та нажимаємо «Next»</p>
  <img src="image/Install/Windows/1_10.png"/>
  <p><span class="two">1.11</span> Обираємо Use Strong Password Encryption for Authentication та нажимаємо «Next»</p>
  <img src="image/Install/Windows/1_11.png"/>
  <p><span class="two">1.12</span> Потрібно вигадати та ввести пароль у поле MySQL Root Password та повторити введення у поле нижче. Натискаємо «Next»</p>
  <img src="image/Install/Windows/1_12.png"/>
  <p><span class="two">1.13</span> Залишаємо вибір за замовчуванням та нажимаємо «Next»</p>
  <img src="image/Install/Windows/1_13.png"/>
  <p><span class="two">1.14</span> Обираємо варіант який більше підходить під ваші потреби та нажимаємо «Next»</p>
  <img src="image/Install/Windows/1_14.png"/>
  <p><span class="two">1.15</span> Натискаємо «Execute»</p>
  <img src="image/Install/Windows/1_15.png"/>
  <p><span class="two">1.16</span> Натискаємо «Finish»</p>
  <img src="image/Install/Windows/1_16.png"/>
  <p><span class="two">1.17</span> Нажимаємо кнопку «Next»</p>
  <img src="image/Install/Windows/1_17.png"/>
  <p><span class="two">1.18</span> Натискаємо «Finish». У нас відкрилася вікно MySQLl Workbench.</p>
  <img src="image/Install/Windows/1_18_1.png"/>
  <img src="image/Install/Windows/1_18_2.png"/>
  <p><span class="two">1.19</span> Переходимо в Командний рядок. Переходимо в папку MySQL\MySQL Server 8.0\bin. Пишемо команду mysql -u root -p та вводимо пароль </p>
  <img src="image/Install/Windows/1_19.png"/>
  <p><span class="two">1.20</span> Після виконання цих дій, ми можем працювати з MySQL!</p>
  <img src="image/Install/Windows/1_20.png"/>
  </details>
</div>

<!-- Раздел 2 -->
<div class="section" id="section2">
  <h3>2. Елементарні операції побудови реляційної схеми в MySQL Workbench 🛠</h3>
  <h4><span class="one">2.1</span> Створення реляційної схеми</h4>
  <p><span class="two">2.1.1</span> Після того, як ви відкрили MySQL Workbench, натисніть Local instance MySQL Router</p>
  <img src="image/Operations/2_1_1.jpeg"/>
  <p><span class="two">2.1.2</span> Після відкриття необхідно відкрити нову модель як показано на фото File => New Model</p>
  <img src="image/Operations/2_1_2.jpeg"/>
  <p><span class="two">2.1.3</span> У вкладці MySQL Model  необхідно натиснути на Add Diagram</p>
  <img src="image/Operations/2_1_3.jpeg"/>
  <h4><span class="one">2.2</span> Створення та налагодження реляційної таблиці</h4>
  <p><span class="two">2.2.1</span> Натискаємо на значок таблиці на лівій панелі інструментів</p>
  <img src="image/Operations/2_2_1.jpeg"/>
</div>

<!-- Раздел 3 -->
<div class="section" id="section3">
  <h3>3. Базові поняття 🖇</h3>
  <h4><span class="one">3.1</span> Атрибути стовпців (PK, NN, UQ, B, UN, ZF, AI, G)</h4>
  <p><dfn>PK (Primary Key / Первиний Ключ)</dfn></p>
  <img src="image/Concepts/3_1_1.jpeg"/>
  <p>	Використовується для однозначної ідентифікації запису (строки таблиці) в реляційній таблиці. По суті є ідентифікатором (id) запису в даній таблиці.</p>
	<div class="dangerous">
	<h4>⛔ Первиний ключ має відповідати наступним вимогам:</h4>
	<ul>
		<li>Унікальність. Первиний ключ не має повторюватися в рамках однієї таблиці.</li>
		<li>Повинен завжди мати значення (бути Not Null).</li>
	</ul>
  </div>	
  	<div class="recomendation">
		<h4>💡 Рекомендації щодо використання первинного ключа</h4>
		<ul>
			<li>Т.к. пошук в базі даних може виконуватися за допомогою бінарного алгоритму, то в якості первинного ключа можна використовувати цілочисельний тип (int), це прискорить пошук.</li>
			<li>В якості первинного ключа також може бути викорастано UUID (Universally Unique IDentifier). Кажучи простими словами, UUID - це такий ідентифікатор, що є унікальним в межах планети Земля. </li>
		</ul>
	</div>
  <p><dfn>NN (Not Null / Не порожній)</dfn></p>
  <img src="image/Concepts/3_1_2.jpeg"/>
  <p>Стовпець з атрибутом NN, на відміну від стовпця без даного атрибуту, зобов'язаний містити значення, що відповідає заданому типу стовпця, відмінне від NULL.</p>
  <p><dfn>UQ (Unique Index / Унікальний)</dfn></p>
  <img src="image/Concepts/3_1_3.jpeg"/>
  <p>Поле стовпця з атрибутом UQ кожного запису має містити унікальне значення в рамках даної таблиці.</p>
  <p><dfn>B (Binary / Бінарний)</dfn></p>
  <img src="image/Concepts/3_1_4.jpeg"/>
  <p>Використовується для зберігання даних у вигляді бінарних рядків.</p>
  <p><dfn>UN (Unsigned / Без знаку)</dfn></p>
  <img src="image/Concepts/3_1_5.jpeg"/>
  <p>Використовується, якщо поля цього стовпця мають містит тільки позитивне число починаючи з 0.</p>
  <p><dfn>ZF (Zero-Filled / Нульові розряди)</dfn></p>
  <img src="image/Concepts/3_1_6.jpeg"/>
  <p>До прикладу, ви хочете щоб ціле число мало сталу кількість розрядів, нехай буде 3. Ви визначаєте тип стовпця як int(3), і тоді коли ви будете зберігати в дане поле значення 21, буде збережено 021.</p>
  <p><dfn>AI (Auto Increment / Автоінкрементація)</dfn></p>
  <img src="image/Concepts/3_1_7.jpeg"/>
  <p>Кожен ново-доданий запис буде містити значення поля стовпця з атрибутом АI на одиницю більше за попередній запис.</p>
		<div class="dangerous">
	<h4>⛔ Стовпець з атрибутом АI має відповідати наступним вимогам </h4>
	<ul>
		<li>Тип даних стовпця має бути INT.</li>
	</ul>
  </div>
	 <div class="recomendation">
	<h4>💡 Рекомендації щодо використання автоінкрементації</h4>
		<ul>
			<li>Часто використовується у поєднанні з PK.</li>
		</ul>
	</div>
  <p><dfn>G (Generated Column / Генеруймий)</dfn></p>
  <img src="image/Concepts/3_1_8.jpeg"/>
  <p>Дозволяє генерувати значення, що буде збережено у полі, за допомогою заданого виразу.</p>
  <p><dfn>FK (FOREIGN KEY / Зовнішній клюс)</dfn></p>
  <p>Використовується для посилання на запис іншої таблиці.</p>
	<div class="dangerous">
	<h4>⛔ Зовнішній ключ має відповідати наступним</h4>
	<ul>
		<li>Повинен мати той самий тип, що і первинний ключ, на якій він посилається.</li>
		<li>Повинен мати значення первинного ключа, що дійсно існує в таблиці, на яку посилається.</li>
	</ul>
  </div>
  <div class="recomendation">
	<h4>💡 Рекомендації що до використання зовнішнього ключа</h4>
		<ul>
			<li>Нехай TableA містить зовнішній ключ по відношенню до TableB. Тоді зазвичай зовнішній ключ називають у форматі: fk_TableA_TableB.</li>
		</ul>
	</div>
  <h4><span class="one">3.2</span> Групи операцій (DDL, DML, DCL, TCL)</h4>
  <p>DDL (Data Definition Language) - група команд, що використовується для ствоерння, модифікації, видалення баз даних та реляційних таблиць (не самих даних)</p>
  <ul>
	<li>CREATE</li>
	<li>DROP</li>
	<li>ALTER</li>
	<li>TRUNCATE</li>
  </ul>
  <p>DML (Data Manipulation Language) - група команд, призначена для додавання, модифікації, видалення даних</p>
    <ul>
	<li>INSERT</li>
	<li>UPDATE</li>
	<li>DELETE</li>
	<li>CALL</li>
	<li>EXPLAIN CALL</li>
	<li>LOCK</li>
  </ul>	
  <p>TCL (Transaction Control Language) - група команд, для роботи з транзакціями </p>
      <ul>
	<li>COMMIT</li>
	<li>SAVEPOINT</li>
	<li>ROLLBACK</li>
	<li>SET TRANSACTION</li>
	<li>SET CONSTRAINT</li>
  </ul>	
  <p>DQL (Data Query Language) - група команд, призначена для отримання даних з бази даних</p>
        <ul>
	<li>SELECT</li>
  </ul>	
  <p>DCL (Data Control Language) - група команд, призначена для керування доступом до бази даних</p>
  <ul>
	<li>GRANT</li>
	<li>REVOKE</li>
  </ul>
  <img src="image/Concepts/SQLCommands.jpg"/>
    <div class="playlist">
	<h4>📹 Відео-лекції, що варто переглянути по темі:</h4>
	<ul>
		<li><a href="https://www.youtube.com/watch?v=KWPUSDHDf1k&list=PLXr7EDDqEOkYiUDqyM3yMg4K2abjEyagl&index=9">Lection 9</a></li>
	</ul>
  </div>
</div>

<!-- Раздел 4 -->
<div class="section" id="section4">
  <h3>4. Приклад ствоерння реляційної схеми з використанням MySQL Workbench на основі ER-моделі 🔍</h3>
  <h4><span class="one">4.1</span> ER-модель системи IOO</h4>
  <img src="image/RelSxem/4_1.svg"/>
  <h4><span class="one">4.2</span> Найпопулярніші елементарні типи даних</h4>
  <table border="3px">
	<tr>
		<th>Тип</th>
		<th>Опис</th>
	</tr>
	<tr>
		<td>INT(N)</td>
		<td>Ціле число. N - максимальна кількість рзрядів числа. Частина (N) - може опускатися</td>
	</tr>
	<tr>
		<td>VARCHAR(N)</td>
		<td>Рядок зазначеної довжини.N - максимальна кількість символів</td>
	</tr>
	<tr>
		<td>DATETIME</td>
		<td>Дата та час</td>
	</tr>
  </table>
  <h4><span class="one">4.3</span> Типи шкал</h4>
  <h4><span class="two">4.3.1</span> Номінальна шкала</h4>
  <p>Номінальна шкала - шкала, що використовується з метою відрізняти предмети один від одного. Вона є зручною для ідентифікації предметів. Одним з найяскравіших представників номінальної шкали є палітра кольорів.
	Ми не можемо сказати, що блакитний більше жовтного, або навпаки.
  </p>
  <h4><span class="two">4.3.2</span> Ординальна шкала</h4>
  <p>Ординальна шкала - номінальна шкала, між елементами якої встановлено відношення порядку. Дана шкала дозволяє порівняти два предмети і визначити їх взаємне відношення один-до-одного.
  </p>
  <h4><span class="two">4.3.3</span> Інтервальна шкала</h4>
  <p>Інтервальна шкала - ординальна шкала, в якій існує однозначне відображення, що співставляє кожному відношенню між двома предметами певне число. Це дозволяє визначити не тільки сам факт, що один предмет "більше" іншого, але й сказати на скільки. </p>
  <h4><span class="two">4.3.4</span> Абсолютна шкала</h4>
  <p>Абсолютна шкала - інтервальна шкала, в якій певний предмет приймається за нульовий, і існує функція, що співставляє кожному предмету шкали відстань (невід'ємне число) від нульового предмету. Відстань між двома довільними предметами визначається як різниця відстаней від нульового предмету вимірюваних предметів.
	Одним з найвідоміших прикладів абсолютної шкали є шкала Кельвіна. Вона починається з так званого абсолютного нуля і проводовжується в додатньмоу напрямку, себто не містить від'ємних значень.
  </p>
  <h4><span class="one">4.4</span> Реляційна схема системи IOO</h4>
	<div style="backgroundcolor: white;">
		<img src="image/RelSxem/4_4.svg"/>
	</div>
    <div class="playlist">
	<h4>📹 Відео-лекції, що варто переглянути по темі:</h4>
	<ul>
		<li><a href="https://www.youtube.com/watch?v=jfGZq4wBBoo&list=PLXr7EDDqEOkYiUDqyM3yMg4K2abjEyagl&index=8">Lection 8</a></li>
	</ul>
  </div>
</div>

<!-- Раздел 5 -->
<div class="section" id="section5">
  <h3>5. Автогенерація DDL з використанням MySQL Workbench ⚙️</h3>
  <p><span class="two">5.1</span> Для того, щоб згенерувати скрипт необхідно зайти по такому алгоритму: File =>Export=>Forward Engineer SQL CREATE Script</p>
  <img src="image/AutoGen/5_1.jpg"/>
  <p><span class="two">5.2</span> Під пунктом 1 обираємо шлях, або ж ми можемо прописати його вручну. 
Далі необхідно поставити галочки на три пункти, які позначені на фото цифрою два. 
Після всіх цих пунктів нажимаємо кнопку "Next".</p>
  <img src="image/AutoGen/5_2.jpg"/>
   <p><span class="two">5.3</span> Після цього, нам необхідно поставити галочку лише на першому пункті Export MySQL Table Objects та нажати кнопку "Next".</p>
  <img src="image/AutoGen/5_3.jpg"/>
	<p><span class="two">5.4</span> Ми отримали скрипт, який можем переглянути, подивитись на таблиці. Для завершення екпортування нажміть кнопку "Finish".</p>
  <img src="image/AutoGen/5_4.jpg"/>
</div>
<div class="section" id="section6">
  <h3>6. Корисні посилання 🔗</h3>
  <ol>
	<li><a href="https://dev.mysql.com/downloads/mysql/">Завантаження MySQL Universal Installer</a></li>
	<li><a href="https://www.youtube.com/playlist?list=PLXr7EDDqEOkYiUDqyM3yMg4K2abjEyagl">Плейліст лекцій БД 2023</a></li>
	<li><a href="https://github.com/YehorSeniuk/IOO">Репозиторій проекту IOO</a></li>
	<li><a href="https://yehorseniuk.github.io/IOO/">Gh-pages проекту IOO</a></li>
  </ol>
</div>
