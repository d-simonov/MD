# Projects:
## 1. EID (https://www.idnow.io/products/idnow-eid/).
This is a very fast way of identity verification. A fully automated process that requires only an ID card and smartphone.
### О чем этот проект простыми словами?
В Германии вместо внутреннего паспорта используются пластиковые ID карты с чипом. Проект дал возможность использовать этот чип для мгновенной идентификации пользователей для всех клиентов IDNOW. Нужно просто приложить ID карту к смартфону и ввести код из смс и личность подтверждена.
Если идти по старому пути то процесс занимает около 5 минут, новый процесс занимает около 1 минуты.
### Результаты проекта
Однозначно процесс идентификации стал быстрее для пользователя, если у него есть необходимая ID карта. Я также думаю что конверсия с новым способом выше чем со старым(меньше пользователей не доходит до конца идентификации, но это надо проверять).
С момента запуска много пользователей прошли идентификацию через новый процесс (точное количество сейчас не знаю, могу точно сказать, порядка десяток тысяч, думаю).

## 2. ACD system integration.
An Automatic Call Distributor (ACD) is a software system that routes incoming identification calls to a specific agent or department within a company. It is rather complex and analyses more than 100 parameters before the call gets distributed to its recipient.
### О чем этот проект простыми словами?
** Представьте себе колл центр где работники отвечают на звонки (у нас это запросы на идентификацию). В нашем случае все еще сложнее, потому что запрос на идентификацию имеет намного больше параметров чем звонок на линию поддержки. Необходимо учитывать на каком языке обслужить клиента, от какой компании он пришел (некоторые компании имеют приоритет). Как долго он ждет в очереди. Какой у него документ, нужно ли ему подписать документ или простая идентификация, и еще сотня подобных критериев. Задача в том чтобы найти наиболее подходящего работника колл центра для каждого запроса на идентификацию. Мы раньше эту логику делали сами, но в этом проекте интегрировались со специальной системой которая делает это все намного профессиональнее и лучше.
### Результаты проекта
Много улучшений, сократилось ожидание в очереди, более точное назначение работника итд итп. До этого француз звонит и ему мог попасться работник который разговаривает по английски. Теперь попытаемся ему найти подходящего который поймет его на французском.

## 3. Project to enable home-office work for call center agents during corona lockdown.
A security framework was established to provide better personal data protection.
### О чем этот проект простыми словами?
До коронавируса колл центр был всегда в офисе, и там очень много мер безопасности. Изза ковида все ждали закрытия колл центра, работать в офисе было нельзя. Пришлось на ходу изменять софт чтобы было возможна работа из дома. Добавили роли пользвателя, ограничения и такое прочее.
Это был быстрый проект на пару недель
### Результаты проекта
Компания продолжила работу после covid shutdown. Не единого дня простоя, и данные не утекли в интернет, что можно считать успехом.

## 4. Platform stability and scalability upgrades. That allows the company to onboard more customers now and maintain SLA's that were promised to the customers.
### О чем этот проект простыми словами?
Улучшили стабильность системы, подготовили систему к возросшей нагрузке.
### Результаты проекта
Будет сложно представить, но по метрикам уменьшилось время когда система недоступна. Клиенты заметили изменение в виде более точного выполнения service-level agreement прописанных в контрактах.

## 5. Project which increased company's gross margin.
### О чем этот проект простыми словами?
We wanted to reduce the overall time our identification process takes since it was the most expensive piece of the process. The challenge was that the process was already shortened to a minimum, and there was not much room for optimizations. However, a team led by Dmitry discovered that we might save some time on a review that is performed after every single identification and use intelligent rules to automate the process for some customers.
### Результаты проекта
As a result, Dmitry and his team cut the average identification time by more than 3 minutes for VideoIdent and by 1 minute for electronic signatures. That means 30% and 10% average identification time reduction. This saved company a significant amount of money.
Тут нужно понимать что уменьшение среднего времени идентификации на 1 секунду это сэкономленные десятки тысяч евро.

## 6. Improving backend component which is responsible for video streaming during the identification.
### О чем этот проект простыми словами?
Это был мой личный проект, занял полгода. У нас в системе есть видео звонки когда пользователь проходит идентификацию с работником колл центра. Компонент который отвечает за видео поток и запись видео был полностью переработан.
### Результаты проекта
Reduced the number of failed identification calls and improved the conversion rate. Улучшилось качество звонков и возможность общаться при плохом соединении.

## 7. Onboarding HelloSign as a partner and modifying our patented technology to integrate new Signing providers.
HelloSign is a Dropbox company, who were selected to be our partner (see here how they use our technology in their workflow https://www.hellosign.com/features/qualified-electronic-signatures). Also see the press release on our partnership here:  https://blog.dropbox.com/topics/product/hellosign-offers-eu-businesses-a-more-secure--legally-binding-wa
We had to change our signing technology to onboard HelloSign because they had a few specific requirements and wanted to use a new TSP (Trusted Signing Provider) called Namirial. We developed a solution for HelloSign to issue Qualified Electronic Signatures. A Qualified Electronic Signature (QES) is the only signature type given the same legal value as handwritten signatures. It is an advanced electronic signature with a qualified digital certificate that has been created by a qualified signature creation device (QSCD). The QSCD must be issued by a qualified EU Trust Service Provider (TSP) on the European Union Trust List (EUTL).
The project was a challenge from the start requiring us to change our signing module from our technology to be able to add new TSP’s. Usually, a company uses a single TSP; having many is not a standard requirement. Adding a new TSP to the system is a significant and complex integration work. There were some major differences in how the signing flow works in the new TSP compared to our existing TSP’s. The team led by Dmitry made this significant modification that made it possible to make our technology work with HelloSign.
В двух словах, проект позволил получить DropBox в качестве клиента компании.
