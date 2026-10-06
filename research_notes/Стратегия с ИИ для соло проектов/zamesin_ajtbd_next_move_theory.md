# Advanced JTBD (Продвинутый JTBD) Ивана Замесина, канон и AI-скиллы Next Move Theory, скилл brainstorming из obra/superpowers

> **Как собирались данные (читать первым).** Дата исследования: 2026-10-06.
> - **Главный первоисточник**: публичный репозиторий `zamesin/Next-Move-Theory-Canon-and-Skills`, скачан через `git clone` (ветка main, коммит `f8e87d1` от 2026-09-13 = версия бандла **v0.6.18**). Канон написан **на английском**: в README Замесин пишет, что перевёл свои русскоязычные тезисы на английский с помощью Claude. В репозитории **нет ни одной строки на русском**: я проверил это поиском кириллицы по всем .md-файлам.
> - Репозиторий `obra/superpowers` тоже скачан через `git clone` (коммит `8ca22db` от 2026-09-25 = **v6.4.2**).
> - **Русскоязычные первоисточники открыть не удалось.** Прокси этой среды блокирует zamesin.ru, zamesinschool.ru, t.me, setka.ru, gopractice.ru, habr.com, vc.ru, medium.com, nextmovetheory.com и youtube.com. Поэтому русская терминология ниже взята только из **сниппетов и сводок поисковика**. Такие места помечены «[RU, сниппет поиска]»: это не дословная цитата со страницы. Ближе к концу работы закончился и лимит веб-поиска.
> - Видео https://www.youtube.com/watch?v=r5kc7AMTEJE **посмотреть не удалось**: YouTube заблокирован, а поиск по ID ничего не нашёл.
> - Все английские цитаты из канона дословные. Русские пояснения к ним — мои переводы, если не указано иное.

## 1. Advanced JTBD: точные определения Job, её элементов и уровней (Core / Big / Small / Micro / Super Big), иерархия и «лесенка» через «зачем?»

### Takeaway
В AJTBD (стабильная версия v3.4 на 2026 год) **Job (работа)** — это *«specification of a desired transition»*, то есть спецификация желаемого перехода из Состояния A в Состояние B *«in order to»* (чтобы выполнить) работу уровнем выше. Полная работа состоит из **8 элементов**. Уровни работ задаются **относительно охвата вашего продукта**, а не абсолютно. **Core Job** — самая высокая работа, которую продукт выполняет полностью. **Big Job** — на уровень выше: продукт вносит в неё вклад, но не выполняет её целиком, и именно в ней живёт мотивация клиента. **Small Job** — работа того же уровня, что Core (сестринская, «sibling»), под тем же Big Job, но выполняет её не ваш продукт. **Micro Job** — уровень ниже Core. Иерархию проверяют вопросом *«For what? / In order to do what?»* («Для чего? Чтобы что?»), который задают к каждому узлу графа.

### Cited Findings
**Определение работы и базовые тезисы**
- Дословно: *«A Job is the specification of a desired transition. It names the person's situation (State A), the transition process, and the expected outcome (State B), in order to perform a higher-level Job that ultimately satisfies a need.»* — [ajtbd-key-theses.md §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- Цель, задача и работа — синонимы: *«Goal = task = Job. The terms are interchangeable. Anything described with `I want + infinitive verb` … is a Job. Each verb is a separate Job.»* По-русски получается «цель = задача = работа», и это даёт ответ на вопрос о терминах «работа» и «задача». — [ajtbd-key-theses.md §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- Работа — это не потребность: *«A Job is not a Need… Needs (safety, status, autonomy, contact, control, self-realization) live in the unconscious… A Job is the concrete, conscious way a person tries to satisfy a set of needs.»* Тот же файл: *«A Job is the root cause of every human action»* и *«A Job is a unit of human motivation.»* — [ajtbd-key-theses.md §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- Правила для агентов прямо отвергают классическое определение Кристенсена и Моесты: работа — это *«not "the customer's struggle for progress," not a need, not a problem, not a feature. It is a unit of motivation.»* — [CLAUDE.md §1](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/CLAUDE.md)
- Три единицы анализа AJTBD: **Job**; **Job Graph of the segment** (граф работ сегмента); **Map of Segments** (карта сегментов) — *«the set of distinct Job-based segments… with their economic attractiveness attached — size, Jobs budget, frequency, reachability, ability to create value, competition.»* — [ajtbd-key-theses.md §1](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)

**8 элементов работы.** Они сгруппированы в три смысловых блока: *«when ___, I want to ___ (with these success criteria), in order to ___»*. — [ajtbd-key-theses.md §3](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
  - **When (Когда)**:
    1. *Context* (контекст) — *«the features of the person and the situation (or, in B2B, the company and the role) that make this person want exactly this outcome with exactly these criteria»*;
    2. *Negative emotions* (негативные эмоции) — *«anxiety, irritation, doubt, shame»*;
    3. *Consideration Set* — *«the information that loaded the awareness that a more effective way to perform the higher-level Job exists»*;
    4. *Trigger* (триггер) — *«the event in time that kicks off the action»*.
  - **I want to (Я хочу)**:
    5. *Expected outcome* (ожидаемый результат) — `I want to + infinitive verb`;
    6. *Success criteria* (критерии успеха) — *«the concrete, measurable criteria by which the person judges that the outcome was reached well enough»*.
  - **In order to (Чтобы)**:
    7. *Higher-level Job* (работа уровнем выше), *«named by its expected outcome»*;
    8. *Positive emotions* (позитивные эмоции) — *«calm, satisfaction, pride»*.
- Сокращать работу до формы «I want to + expected outcome» можно только в разговоре: *«That shorthand is the main part of the Job, but it is not the whole Job. The whole Job is all eight elements.»* К полной записи работы добавляются ещё три характеристики: **Job Frequency** (частота), **Job Budget** (бюджет работы) и **Job Importance (1–10)** (важность). — [ajtbd-key-theses.md §3–4](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- [RU, сниппет поиска] Русский словарь AJTBD описывает 8 элементов так: *«контекст, эмоции, активирующее знание, триггер, ожидаемый результат, критерии, работу выше уровня и позитивные эмоции»*. То есть в русской версии третий элемент назывался **«активирующее знание»**, а в английском каноне 2026 года ему соответствует *Consideration Set*. В английском гайде по интервью до сих пор есть строка *«Activating knowledge (optional)»*. — [Словарь терминов AJTBD, zamesinschool.ru (через поиск)](https://zamesinschool.ru/knowledge_base/slovar-ajtbd); [interview guide §7](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/HowTos/basic-ajtbd-interview-guide-and-principles.md)
- [RU, сниппет поиска] В русском словаре **49 терминов** AJTBD и Next Move Theory: «работа», Core Job, Big Job, триггер, критерии успеха и другие. — [zamesinschool.ru (через поиск)](https://zamesinschool.ru/knowledge_base/slovar-ajtbd)

**Уровни работ. Это главное место для формулировок Core и Big Job.**
- *«The four levels are defined relative to our product's reach, not as absolute positions on the customer's full life-Graph… Two products competing for adjacent territory will label different Graph levels as their Core, and both are correct.»* — [ajtbd-key-theses.md §9](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- **Core Job**: *«the highest-level Job your product performs fully, and that you cannot climb above with the product's current shape. The operational test is whether most of the Micro Jobs underneath are performed inside your product, by your team, or by automation you own.»* — [job-graph.md §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md)
- **Big Job**: *«one level above your Core Job. It carries the motivation. Your product contributes to it but doesn't fully perform it. A single set of Core Jobs typically serves several Big Jobs at once.»* — [job-graph.md §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md)
- **Small Job**: *«a sibling of your Core Job, at the same level, under the same Big Job, that your product doesn't perform. It is performer-agnostic… Small Jobs are siblings of Core, not below it.»* Дальше: *«Our Small Jobs are another product's Core Jobs, and our Core Jobs are theirs. They are the primary source of growth opportunities.»* — [job-graph.md §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md); [ajtbd-key-theses.md §9](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- **Micro Job**: *«one level below your Core Job and Small Jobs. The fine grain where customer experience lives.»* **Super Big Job**: *«one level above Big. It is often near the customer's life-level motivation.»* — [job-graph.md §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md)
- *«Levels above our Core Job carry motivation; levels below carry mechanism.»* Это граф, а не дерево: связи «многие ко многим». *«The more higher-level Jobs a single lower-level Job contributes to, the higher the customer's motivation to perform it.»* — [ajtbd-key-theses.md §9](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- Несколько Core Jobs на одном уровне — это норма. Например, у Uber *«get there fast when I'm in a hurry / with my dog / with room for four suitcases»*. — [job-graph.md §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md)
- Типичная ошибка: *«The recurring error is putting Small Jobs below Core Jobs.»* — [job-graph.md §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md)
- Пример из консалтинга про относительность уровней: *«A consultant who delivers "build your personal brand" turnkey has that as a Core Job. An agency that only "writes your LinkedIn posts" has the same Job two levels lower.»* — [job-graph.md §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md)
- [RU, сниппет поиска] Русские формулировки: *«Big Job — это работа на один уровень ВЫШЕ Core Job, в которую продукт вносит вклад, но НЕ выполняет полностью. Big Job несёт мотивацию клиента, а Core Job — то, что делает продукт. Например, для DoorDash Big Job — «накормить семью сегодня, не готовя»»*. Также *«Micro Job (микроработа)… работа на один уровень ниже Core Job»*. В русских текстах названия уровней (Core/Big/Small/Micro Job) пишутся по-английски. — [zamesinschool.ru / zamesin.ru (через поиск)](https://zamesinschool.ru/knowledge_base/slovar-ajtbd)
- [RU, сниппет поиска, вторичный источник: пост ученика на setka.ru] *«Big Job всегда отвечает на вопрос: «Зачем выполняется core job?»»*. Пример из поста: Core Job «освоить подход Scrum», Big Job «стать востребованным специалистом, способным обеспечивать ритмичную поставку инкрементов продукта командой через внедрение Scrum». Поисковик вернул этот текст в английском пересказе, так что русская формулировка восстановлена приблизительно. — [setka.ru (через поиск)](https://setka.ru/posts/01942a83-dcbd-494e-a79d-384f780fc241)

**Как поставить Core Job на правильный уровень (climb test, «тест подъёма»)**
1. Спросите платящих клиентов: *«What tasks do you solve with our product?»*
2. *«Does our product fully perform this Job, every sub-Job inside our product, end-to-end?»* Если нет — работа слишком высоко, опуститесь на уровень. Если да — *«Can we climb one level higher and still fully perform that higher Job?»*
3. Остановитесь на уровне, где ответ на первый вопрос «да», а на второй «нет». *«Climb as high as you can.»*

Источник: [job-graph.md §3](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md). Если поставить Core слишком высоко, продукт не выполнит обещанное, и коммуникация сама создаст клиенту Problem. Если слишком низко, неверными получатся сегменты, механики и рост — [job-graph.md §3](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md).

**«Лесенка» через «зачем?»**
- Вопрос интервью: *«Why did you want {expected outcome}?»*, затем *«and that, in order to do what?»*. Обычно останавливаются на Big и Super Big Jobs. Признак, что вы упёрлись в потолок: респондент *«repeats the previous answer»*. Это значит, что дошли до потребности, а она неосознаваема. — [job-structure.md §9](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-structure.md)
- Проверка готового графа: *«apply "for what? / in order to do what?" to every node in succession»*. Так находятся 4 ошибки: **skip-a-level** (пропущен уровень, самая частая), **wrong parent** (неверный родитель), **multi-verb Job** (несколько глаголов в одной работе), **Fake Job**. — [job-graph.md §18](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md)
- **Критическая цепочка работ (Critical Chain of Jobs)** — граф работ, развёрнутый во времени для выбранного решения: *«What a team actually ships is the Critical Chain of Jobs, not the Job.»* Идея заимствована из *Critical Chain* Голдратта. — [ajtbd-key-theses.md §10](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md); [nmt-key-theses.md §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Next-Move-Theory/nmt-key-theses.md)

**Типы работ и связанные понятия** (все из [job-types-and-properties.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-types-and-properties.md))
- Типы: **Regular, Orientation, Tax, Fake, Emotional, Viral**.
- **Orientation Job** — работа, которую выполняют, чтобы обновить знания о доступных решениях и выбрать одно из них. Её узнают по глаголам *«understand, find out, find, choose, figure out, decide between, research, compare»*. Фактически это и есть «принятие решения» клиентом.
- **Tax Job** — *«a Job the customer never planned to perform, and now has to, because the Solution hired… failed.»*
- **Fake Job** — *«the customer's fantasy about a future Job… never performed in the past.»* Диагностический вопрос: *«In the past, have you done anything to {expected outcome}?»*
- **Viral Job** — работа, которую выполняют для другого человека или вместе с ним. *«Teachers, consultants, agencies, content creators… consistently rank near the top»* по количеству вирусных работ.

### Inferences
- Для команды проекта: в AJTBD нет понятий «маленькая работа» или «более мелкие работы» в смысле «работы под Core». **Small Job — это соседняя работа на том же уровне.** Всё, что ниже Core, называется **Micro Job**. Здесь легче всего ошибиться при переводе на русский.
- «Core» и «Big» — это не свойства самой работы, а её положение относительно продукта. Если продукт — «стратсессия 1:1 + AI-скиллы», Core Job ставится на уровень, который сессия реально **доводит до результата целиком**. Ставить туда «вырастить бизнес» нельзя.
- Русскоязычные материалы Замесина до 2026 года (словарь, книга «Как делать продукт») используют более старые формулировки, например «активирующее знание». Английский канон 2026 года их переименовал и расширил: Consideration Set, Consideration Activators, Critical Chain of Jobs, Super Big Job. Рабочий глоссарий команды лучше строить по канону 2026 года, а русские термины давать как глоссы.

### Gaps
- Дословные русские определения из словаря на zamesinschool.ru (49 терминов) открыть не удалось: сайт заблокирован. Русские эквиваленты новых терминов (Consideration Set/Activators, Critical Chain of Jobs, Tax/Fake/Orientation/Viral Job, Super Big Job) мной **не проверены**.
- Понятия **«кредит доверия», «сложность», «сегмент по работе»** (дословно) в английском каноне не встретились. Есть ли они в русских курсовых материалах, проверить не удалось. «Мотивация» в каноне есть, но как свойство уровней (*«Big Jobs carry the customer's motivation»*), а не как отдельный термин.

---

## 2. Как правильно формулировать работу: шаблоны, критерии хорошей формулировки, частые ошибки

### Takeaway
Официальная грамматика: **When {context + trigger + negative emotions}, I want to {expected outcome} with success criteria {concrete, measurable}, in order to {higher-level Job + positive emotions}**. Канон требует писать *«in order to»*, а не *«so that»*. Работу можно записать с тремя уровнями детальности, но источником правды считается только полная запись из 8 элементов. Главные правила: работа — это глагольная фраза в инфинитиве; один глагол — одна работа; критерии конкретные (у каждого есть направление и уровень); тот же результат с другими критериями — это уже другая работа.

### Cited Findings
- **Канонический формат** (как записано в скилле): *«Format: When {context + trigger + negative emotions before}, I want to {expected outcome} with success criteria {concrete, measurable criteria — plain text}, in order to {higher-level Job + positive emotions after}. The canon uses "in order to," not "so that."»* Дополнительно: *«Name the level every time — Big / Core / Small / Micro Job»* и *«In questions addressed to customers, use the everyday word task, never "Job."»* — [nmt-market-research/SKILL.md, раздел «Job grammar»](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Skills/claude/nmt-market-research/SKILL.md)
- **Три уровня детальности** ([ajtbd-key-theses.md §4](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)):
  - *Level 1* — все 8 элементов плюс Frequency, Budget, Importance. Нужен для заметок после интервью, дизайна ценностного предложения, графа и RAT-карточек.
  - *Level 2* — `When {context} + {trigger}, I want to {expected outcome} with {main success criteria}, in order to {expected outcome of the higher-level Job}.` Для брифов и сравнения сегментов.
  - *Level 3* — `I want to {expected outcome} with {main success criteria}.` Для заголовков и рекламы.
  - *«Level 1 is the source of truth; Levels 2 and 3 are derived artifacts.»*
- Готовый пример Level 2 из канона: *«When I'm finishing Friday-night Mission dinner at 11:30pm (two glasses of wine, no car, 9am yoga tomorrow) and the check arrives, I want to get to my Russian Hill apartment door safely, under $25, in <5 min, clean Comfort-tier car, quiet driver, in order to be in bed by 12:30am rested for yoga and feel I made the responsible adult choice.»* — [ajtbd-key-theses.md §4](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- **Минимально пригодная запись**: *«The minimum-viable Job description is `I want to {expected outcome} with {main success criteria}`… Anything else… can in principle be reconstructed from interviews. Criteria cannot.»* — [job-structure.md §7](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-structure.md)

**Правила для ожидаемого результата** ([job-structure.md §7](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-structure.md))
1. *«A Job statement is a verb-phrase, not a noun-phrase. "Rental management," "retirement management," "tax filing" are not Jobs — they are category labels.»*
2. *«A Job looks from the present into the future. Wrong: "I want to have figured it out"… Right: "I want to understand".»*
3. Грамматику работы нужно соблюдать везде: в каноне, в выводах скиллов, в брифах, в текстах лендинга.
4. Объект добавляется, когда глагол без него неполон: *«learn → learn how to code; hire → hire a senior engineer»*. Для чувств используется *«feel + a state»*.

**Правила для критериев успеха** ([job-structure.md §8](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-structure.md))
- Критерий должен быть конкретным, но не обязательно числовым: ❌ *«fast»* → ✅ *«the car arrived in under 4 minutes»*; ❌ *«good UX»* → ✅ *«booked in three taps, no form to fill in»*.
- У каждого критерия две компоненты. **Direction** (направление): *«what axis the value is being created on»*. **Level** (уровень): *«the threshold above which the customer feels value, below which they feel a problem»*.
- Критерии одновременно служат метриками активации: *«The team that writes down the segment's criteria has, in the same act, written the metric set the product should be measured on.»*
- [RU, сниппет поиска; источник страницы не установлен] *«Критерии успеха — параметры, по которым человек оценивает результат работы. Должны быть конкретными и измеримыми. «Быстро», «качественно», «надёжно» — абстракции, не критерии.»* — [поисковая сводка; ссылалась среди прочего на zamesinschool.ru](https://zamesinschool.ru/knowledge_base/slovar-ajtbd)

**Тот же результат + другие критерии = другая работа**
- *«Same expected outcome plus different success criteria equals different Core Jobs… and different segments, where different people perform them.»* Пример — тарифы Uber X / Comfort / Black. — [ajtbd-key-theses.md §5, §12](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- Порядок приоритетов между критериями тоже разделяет сегменты: *«price-first vs done-for-me-first vs no-stress-first vs control-first are different segments performing the same Core Job.»* — [CLAUDE.md §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/CLAUDE.md)

**Несколько глаголов в одной фразе — это стопка работ** ([job-structure.md §13](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-structure.md))
- ❌ *«Rent out my duplex and generate predictable monthly income»*.
- ✅ Super Big Job: *«Generate predictable monthly income from my real estate»*; Big Job: *«Rent out my duplex»*.
- Ограничения вроде *«without consuming my evenings»* — *«belong in success criteria, not inside the Job statement.»*

**Не путать работу уровнем выше со своей Core Job**
- *«Don't claim the Higher-level Job as your deliverable. That sets up inflated expectations and manufactured Problems.»* Пример: Wealthfront выполняет Core *«manage my retirement portfolio»*, а работа уровнем выше — *«have enough money at 65 to retire how I want to.»* — [job-structure.md §9](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-structure.md)

**Три понятия, которые путают между собой**
- *«Trigger ≠ Consideration Set ≠ Aha Moment»*. Порядок во времени: сначала загружаются активаторы, потом срабатывает триггер, потом наступает Aha. — [job-structure.md §12](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-structure.md)

**Абстрактная и конкретная работа**
- До выбора решения работа абстрактна. Когда решение выбрано, она становится конкретной, и под ней появляются новые Micro Jobs. — [job-structure.md §14](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-structure.md)

**«Проблема» клиента — не его работа.** Пример из канона, близкий к консалтингу: *«A founder says "I've been trying to hire a Product Manager for six months." … The Job underneath is usually "save a failing product"… The right move may not be hiring at all.»* — [ajtbd-key-theses.md §7](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)

**Списки ошибок, которые скиллы проверяют при стресс-тесте:** *«wrong Job of wrong segment; demographics masquerading as a segment; a Big Job mistaken for a segment (Rule 18); multi-verb Job statements (Rule 7); Small Jobs placed below Core (Rule 8); ≥5 stacked unvalidated assumptions (RAT).»* — [nmt-chat/SKILL.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Skills/claude/nmt-chat/SKILL.md)

### Inferences
- Мой русский перевод шаблона Level 2, сделанный по канону (официальной русской версии 2026 года я не нашёл): **«Когда {контекст} + {триггер} (+ {негативные эмоции}), я хочу {ожидаемый результат: глагол в инфинитиве + объект} с критериями успеха {конкретные: направление + уровень}, чтобы {ожидаемый результат работы уровнем выше} (+ {позитивные эмоции})».** Русское «чтобы» покрывает и «in order to», и «so that». Важно другое: после «чтобы» должна стоять **работа уровнем выше в форме ожидаемого результата**, а не выгода или фича.
- Чек-лист качества формулировки, собранный из правил выше:
  1. Есть инфинитивный глагол.
  2. Ровно один глагол.
  3. Смотрит в будущее.
  4. Критерии конкретные, у каждого есть направление и порог.
  5. Уровень назван (Big/Core/Small/Micro) и проверен тестом подъёма.
  6. Вопрос «чтобы что?» даёт честного родителя без пропуска уровня.
  7. Есть подтверждение в прошлом (платили, тратили время) — то есть это не Fake Job.
  8. Формулировка взята из слов респондента, а не придумана командой.
- Для стратегического продукта: ловушка «обещать Big Job» здесь особенно вероятна. «Стратегия, которая приведёт к росту» — это Big Job. Сессия реально выполняет что-то вроде «выбрать следующий ход и план проверки». Если Core и Big записаны неправильно, коммуникация будет сама создавать клиенту разочарование, то есть Problem.

### Gaps
- Официальный **русский** шаблон Замесина 2026 года (например, «Когда…, я хочу…, с критериями…, чтобы…») дословно проверить не удалось. Поисковая сводка вернула общий шаблон Job Story («Когда…, я хочу…, чтобы…») и не подтвердила, что он взят из материалов Замесина.

---

## 3. Ценность, сегменты, конкуренты, решение клиента («переход на новый граф»), связь со стратегией, позиционированием, ценностным предложением и ростом

### Takeaway
Ценность в AJTBD — это **энергоэффективность выполнения работы для мозга**: результат по критериям клиента, делённый на затраты. Aha-момент — это сигнал, что ценность превзошла прогноз, а Problem — сигнал, что недотянула. **Сегмент — это люди с похожими графами работ**, то есть с похожими Core Jobs и критериями. Демография сегмент не определяет. Реальные конкуренты определяются на уровне **Big Job**. Решение клиента сменить продукт — это **замена одного графа работ другим**, и запускают её пять **Consideration Activators**. Стратегия по определению — это выбор того, *«which Jobs of which people will we compete for, why these and not others, and why will we win?»*

### Cited Findings
**Ценность**
- *«Value is energy efficiency for the brain in performing a Job — outcome (per the customer's success criteria) over cost (time, money, effort, cognitive load, negative emotion, Tax Jobs).»* Основа — модель аллостаза Лизы Фельдман Барретт. — [ajtbd-key-theses.md §6](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- *«The Aha Moment is the pleasant surprise that signals value… The Aha is not value itself.»* *«The Problem is the unpleasant surprise that signals under-delivery.»* *«A feature is not value.»* — [ajtbd-key-theses.md §6](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- [RU, сниппет поиска] Aha-момент в русском словаре: *«описание момента и контекста, когда клиент получил ценность продукта и осознал его ценность… удивление клиента от того, что его работы выполняются эффективнее, чем он ожидал»*. — [zamesinschool.ru (через поиск)](https://zamesinschool.ru/knowledge_base/slovar-ajtbd)
- *«A problem is always the consequence of a Solution that was hired for a Job and screwed up against that Job's success criteria.»* — [ajtbd-key-theses.md §7](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)

**Механики создания ценности**
- Их больше 100. Базовые:
  - *«Move up to a higher-level Job»* — самая сильная;
  - *«Kill a Job»*;
  - *«Take a Job off the customer»*;
  - *«Fix breaks in the Critical Chain of Jobs»*;
  - *«Lower costs»*;
  - *«Eliminate a negative emotion»*.
  
  Источник: [ajtbd-key-theses.md §22–23](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- Подъём на уровень выше объясняет волну AI-продуктов: *«Claude Code climbed above writing code by hand by becoming the Core Job for "ship a working change in this codebase."»* *«This is the methodology-level explanation for the AI-product wave.»* Ориентир (North Star) — *«the invisible product»*. — [ajtbd-key-theses.md §23](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- Пример связи с несколькими Big Jobs, близкий к образовательному или консультационному продукту: *«an AJTBD course links learn product methodology to multiple Big Jobs at once — grow my career, build a side project, consult, become a respected practitioner.»* — [value-creation-mechanics.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/value-creation-mechanics.md)

**Сегменты**
- *«A segment is a group of people with similar Job Graphs.»* *«One person is in one segment, not in many.»* Сегментировать сначала по демографии, персонам или ICP — *«one of the most common and most expensive segmentation errors.»* — [ajtbd-key-theses.md §12](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- *«Big Job is motivation context, never the primary segmentation criterion. Same Big Job contains several segments.»* — [CLAUDE.md §3](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/CLAUDE.md)
- Причинные критерии сегментации и фейковые: ❌ *«spent $1,000 in 6 months," "NPS ≥ 9," "enterprise"»*; ✅ *«willing to delegate the whole project end-to-end," "lives in a different city — time matters more than money"»*. Причинные критерии превращаются в 4–5 вопросов для квалификации лидов. — [CLAUDE.md §3](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/CLAUDE.md)
- Описание сегмента должно отвечать на четыре вопроса:
  1. Можем ли мы дать заметную дополнительную ценность?
  2. Заработаем ли целевую маржу?
  3. Сможем ли создать или перехватить спрос?
  4. Хватит ли размера, чтобы масштабироваться?
  
  Плюс проверка на жёсткий блокер. В скилле это «selection screen». — [nmt-market-research/SKILL.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Skills/claude/nmt-market-research/SKILL.md); [CLAUDE.md §3](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/CLAUDE.md)
- Подсегмент и новый сегмент. *«A sub-segment keeps the same Core Job and the same main success criteria, but a sharper context adds extra success criteria»*. Новый сегмент появляется, *«when the Core Job, the success criteria, or their priority order change materially.»* — [segmentation.md §10](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/segmentation.md)
- **ABCDX** (автор методологии — Илья Красинский). Платящих клиентов делят по марже на единицу и удовлетворённости на группы A, B, C, D; в X попадают те, чьи работы лежат вне продукта. Это ход к локальному оптимуму. Пример из канона: *«A boutique HR-consulting practice… Naming the A pattern and shifting the offer toward it produced +60% revenue in 3–4 months.»* — [abcdx-segmentation-key-theses.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/ABCDX-Segmentation/abcdx-segmentation-key-theses.md)

**Конкуренты**
- *«Direct competitors share your Core Job. Indirect competitors share one or more of your Big Jobs.»* Косвенную конкуренцию обычно недооценивают *«by an order of magnitude»*. DIY (сделать самому) — тоже граф работ и тоже конкурент. — [job-graph.md §15–16](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md)

**Решение клиента и смена поведения.** Термин «next move» в названии Next Move Theory относится к **ходу компании**, а не к выбору клиента. Выбор клиента в AJTBD описан так:
- *«Behavior change is the customer swapping one Job Graph for another.»* Solution — это *«a label for the specific Job Graph»*. — [ajtbd-key-theses.md §2, §8](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- Пять **Consideration Activators** ([ajtbd-key-theses.md §18](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)):
  1. Существует новый граф работ для Big Jobs.
  2. Этот граф выполняет Big Job эффективнее, причём *«a concrete, criteria-anchored delta»*.
  3. Есть конкретный продукт: *«name plus door»* (имя и первый шаг).
  4. Конкретные страхи сняты.
  5. Альтернативы «уволены» конкретными проблемами и рисками.
- *«Value Creation creates the reason to switch Job Graphs; Barrier Removal creates the possibility to switch.»* — [ajtbd-key-theses.md §18–19](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- Барьер и страх — разные вещи. Барьер — это *«objective fact that makes the new way non-executable»*. Страх — *«the customer's prediction that a Barrier, Problem, or loss will happen»*. — [interview guide §8](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/HowTos/basic-ajtbd-interview-guide-and-principles.md)
- Четыре силы прогресса (Four Forces) переведены в архив: *«AJTBD has moved past them.»* — [ajtbd-key-theses.md §21](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)

**Стратегия, позиционирование, коммуникация**
- *«Every strategic product decision reduces to one type: which Jobs of which people will we compete for, why these and not others, and why will we win?»* — [ajtbd-key-theses.md §13](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- **Формула ценностного предложения**: *«[For which segment] + [Which Job — Big or Core] + [How much more effectively, in concrete success criteria] + [Through which features].»* Правило *«Promise must match delivery.»* — [ajtbd-key-theses.md §24](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- **Формула one-liner**: `[What it is] + [Core Jobs the product performs] + [value by criteria]`. Пример: *«Miro — collaboration canvas for running workshops and mapping work with a remote team.»* — [communication.md §5](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/communication.md)
- **Цепочка к прибыли** проходит две фазы:
  - исследование и валидация: рынок с деньгами → сегмент + работа → три условия в теории (маржа на единицу, объём лидов, масштаб без потери качества) → доказательство ценности;
  - масштабирование: те же три условия на практике → целевая прибыль.
  
  *«Low conversion almost never means a funnel problem.»* — [ajtbd-key-theses.md §14](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- **B2B**:
  - *«B2B motivation is usually dominated by personal Jobs, not business Jobs.»*
  - Пять типичных личных работ лица, принимающего решение, начинаются так: *«I want to make a vendor choice that won't get me blamed or fired… use the same tools the best people in my field use… build a career-defining story… offload operational routine… pick a vendor who will still support me at year 3.»*
  
  Источник: [ajtbd-key-theses.md §25](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)

### Inferences
- Для продукта «стратегия для соло-проектов и AI-native команд» механика «подняться на уровень» — центральная стратегическая гипотеза. Скиллы, по определению канона, поднимают Core клиента с «провести исследование рынка» до «выбрать следующий ход». Тогда сама сессия должна выполнять более высокую работу, чем выдают скиллы, например «принять и запустить проверку решения». Иначе её функции поглотит Claude плюс скиллы, то есть DIY-граф, который в AJTBD считается конкурентом.
- Для AI-native команд, если покупает руководитель, по логике B2B-раздела стоит отдельно картировать **личные работы** заказчика: «не ошибиться публично», «иметь историю для команды или инвесторов».

### Gaps
- Каталог из 100+ механик, алгоритм диагностики и полная интеграция юнит-экономики в публичный канон **не входят** (README: публичная часть — *«about 25% of the whole methodology»*). Их содержание проверить нельзя.

---

## 4. Метод JTBD-интервью: рекрутинг, ход интервью, анализ, синтез в граф работ и карту сегментов

### Takeaway
Интервью в AJTBD **восстанавливает мотивацию по тому, что человек уже сделал**: потратил деньги, время или силы. Рекрутируют **только тех, кто платил**. Структура — 7–8 блоков, на 60 минут. Ядро интервью — граф по 6 направлениям, где каждый вопрос привязан к ожидаемому результату работы уровнем выше. Затем подробно разбирают несколько работ по банку вопросов и в конце **обязательно пытаются продать**. Для поиска сегментов с нуля нужно около 60 интервью; останавливаются, когда 10 интервью подряд не дают новых работ. Результат — карта сегментов. Для анализа уже собранных интервью есть скилл `/nmt-analyze-interviews`.

### Cited Findings
**Принципы интервью** ([interview guide §1](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/HowTos/basic-ajtbd-interview-guide-and-principles.md))
- *«Study Jobs by past expenditure of money, time, and energy — never by future intent.»* Скрининг: *«When did you last pay for X? What did you pay? What did you do as a result?»* В B2B есть исключение: лицо, принимающее решение, *«is paid to forecast»*.
- Открывающий вопрос: *«Tell me which tasks you solve with {product}»*, со словом *task*, никогда *Job*. Дальше проверяются гипотезы, потом контроль: *«Does this genuinely annoy you, or did I lead you?»*
- *«Record what they said — don't invent.»* *«Never accept an abstract answer.»* *«Always come with an offer, and sell.»* *«In B2B, always study personal Jobs.»*
- Ограничение метода: *«Mostly-unconscious drivers (status, identity, safety) don't [interview cleanly]… generate the hypothesis yourself and validate it through sales, A/B, or messaging tests.»*

**Структура интервью на 60 минут** ([interview guide §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/HowTos/basic-ajtbd-interview-guide-and-principles.md))
1. Эмоциональный контакт — 3–5 мин.
2. Квалифицирующие вопросы — до 10 мин.
3. Карта графа работ — 5–10 мин.
4. Выбор работ для подробного разбора.
5. Разбор нескольких работ — 30–40 мин.
6. Продажа — 5–10 мин.
7. Просьба о рекомендации — 2–3 мин.

В B2B добавляется блок про роли, сделки и бюджет.

**Шесть направлений, по которым картируют граф** ([interview guide §5](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/HowTos/basic-ajtbd-interview-guide-and-principles.md); [job-graph.md §17](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md))
- Вверх (Big): *«Why do you want {Core outcome}? In order to do what?»*
- Предыдущие работы: *«Step by step, what tasks did you do for {Big Job outcome} before {Core outcome}?»*
- Следующие работы: *«…after {Core outcome}?»*
- Параллельные сестринские работы: *«What other tasks do you do for {Big Job outcome}, besides {Core outcome}?»*
- Вниз, по шагам: *«Step by step, what tasks did you do to get {outcome}?»*
- Вниз, сценарии: *«What are your usual usage scenarios with {product}?»*
- Правило привязки: *«every question carries the expected outcome of the higher-level Job in its frame»*.

**Банк вопросов по работе** ([interview guide §7](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/HowTos/basic-ajtbd-interview-guide-and-principles.md))
- Для повторяющихся работ вопросы задают в настоящем времени, для разовых — в прошедшем.
- Элементы работы: ожидаемый результат, критерии, активирующее знание (по желанию), контекст, триггер, работа уровнем выше, позитивные и негативные эмоции.
- Вес работы: частота и важность от 1 до 10 (*«10 is a matter of life-and-death»*).
- Блок о выбранном решении: удовлетворённость 1–10, ценность, Aha (*«At what point did you realize {solution}'s value — the moment you thought 'oh, that's cool'?»*), цена и ценность 1–10, проблемы, драйверы, страхи, барьеры, альтернативы.

**Масштаб исследования и синтез**
- *«run ~60 interviews comparing segment against segment, and stop when ten in a row produce no new Jobs. Output: a Map of Segments and the choice of target segment.»* — [interview guide §10](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/HowTos/basic-ajtbd-interview-guide-and-principles.md)
- Приоритет того, что выяснять: *«success criteria > Consideration Activators > value > Aha Moment > Barriers»*. — [interview guide §10](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/HowTos/basic-ajtbd-interview-guide-and-principles.md)
- Две стартовые точки. Первая — по платящей базе: ABCDX, затем интервью с группами A и B. Вторая — поиск сегментов с нуля: рекрутируют тех, кто платит конкурирующему решению, и выбирают уровень выборки — *«broad Big Job»* или текущий Core Job во всех вариантах критериев. — [interview guide §10](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/HowTos/basic-ajtbd-interview-guide-and-principles.md)
- Скилл анализа интервью работает так:
  - на каждое интервью запускается отдельный суб-агент, который его «дистиллирует»;
  - качество каждого интервью оценивается по рубрике;
  - сегменты строятся по Core Jobs, у каждого уровень уверенности Solid / Emerging / Hypothesis;
  - для каждого решения прослеживается цепочка «задача → инструмент → проблема»;
  - отдельно собирается consideration set;
  - высказывания одного человека выносятся в блок «Single signals»;
  - есть приложение «источник → сегмент» и список пробелов: кого интервьюировать дальше.
  
  Источник: [nmt-analyze-interviews/SKILL.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Skills/claude/nmt-analyze-interviews/SKILL.md)
- Сценарий интервью и дизайн исследования *до* выхода в поле — это *«a separate (not publicly shipped) product»*. Публично предлагается готовиться к интервью через `/nmt-chat`. — [nmt-analyze-interviews/SKILL.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Skills/claude/nmt-analyze-interviews/SKILL.md)
- [RU, сниппет поиска] На zamesin.ru: *«Advanced JTBD-интервью позволяет узнать граф работ другого человека [Big Jobs + Core Jobs + Small Jobs]»*. — [zamesin.ru (через поиск)](https://zamesin.ru/producthowto/book/about-jobs-to-be-done/)

### Inferences
- Для продукта команды: правило «только платившие» означает, что первых респондентов надо искать среди тех, кто уже **платил** за стратегическую помощь — фасилитаторам, трекерам, менторам, курсам — или **тратил заметное время** на стратегию с ИИ, как автор видео. Тех, кто только «хотел бы», не берут: это риск Fake Job.
- Приём «продавать на каждом интервью» хорошо подходит фасилитатору: в конце интервью можно предложить пилотную стратсессию как проверку гипотезы.

### Gaps
- Полный платный гайд по интервью, шаблоны таблиц синтеза (job map или граф в Miro) и русская версия гайда в доступных источниках не найдены.

---

## 5. Next Move Theory: что это, кто автор, где живёт, лицензия, структура канона, версии

### Takeaway
Next Move Theory (NMT) — мета-фреймворк Ивана Замесина поверх AJTBD. Он объединяет **AJTBD + юнит-экономику + RAT (Riskiest Assumption Test) + ABCDX-сегментацию + Теорию ограничений Голдратта**, а OKR используется как поддерживающая методология. Цель — *«a step-by-step algorithm for every product decision»*. Открытый канон и скиллы лежат на GitHub (`zamesin/Next-Move-Theory-Canon-and-Skills`) под лицензией **CC BY-NC-SA 4.0**. Сайт — nextmovetheory.com. Статус на сентябрь 2026: **AJTBD v3.4 stable, NMT v0.6 in active development**, бандл **v0.6.18** (2026-09-13).

### Cited Findings
- README: *«Next Move Theory is a methodology with a step-by-step algorithm for every product decision: it lays out every tactical and strategic move open to you and helps you choose the best, with the odds on your side.»* *«Advanced JTBD — v3.4 · stable… Next Move Theory — v0.6 · in active development — integrating AJTBD with Riskiest Assumption Test, ABCDX Segmentation, Theory of Constraints, and Unit Economics.»* — [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md)
- Аудитория: *«founders, indie hackers, product managers, and product marketers»*. — [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md)
- Объём открытой части: *«This public canon is the foundation, about 25% of the whole methodology»*. Остальное (алгоритм диагностики, пошаговые алгоритмы по типовым задачам, 100+ механик, брендинг, goal-setting и т.д.) доступно в продуктах и курсах на nextmovetheory.com. — [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md)
- Об авторе (самоописание):
  - *«Trained 13,000+ founders and product managers… running since 2017»*;
  - руководил поиском по картинкам в *«his home market's largest tech company»* (рост доли с 55% до 72%);
  - основал и продал сервис подбора психотерапевтов;
  - *«Two independent industry studies ranked him the #1 product expert in his home market.»*
  
  Источник: [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md)
- О языке канона: *«I built this methodology over eight years in my own language… To bring it into English, I used Claude to render those theses.»* — [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md)
- Определение стратегии в NMT: *«A Company Strategy is a sequence of actions of the company's functions that leads the company toward an expected outcome.»* *«The Chosen Company Strategy is anchored on AJTBD: the choice of Jobs of segments.»* — [nmt-key-theses.md §1](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Next-Move-Theory/nmt-key-theses.md)
- **Алгоритм** — 10 шагов, 3 фазы, работает как цикл ([the-algorithm.md §3](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Algorithms/the-algorithm.md)):
  - **Фаза I — Frame & hypothesize**:
    1. Challenge the business goal (5 Whys).
    2. Diagnose the current state.
    3. Assemble the layer: Map of Segments, Job Graph, Consideration Sets.
    4. Shortlist mechanics.
  - **Фаза II — Research & generate**:
    5. Field research.
    6. Apply mechanics to the REAL Job Graph.
    7. Rank by RICE.
  - **Фаза III — De-risk & ship**:
    8. RAT.
    9. Validate value: *«sales first, then UX 4/4»*.
    10. Ship and вернуться к шагу 1.
  
  Ключевая цитата: *«Phase I is fast and cheap: head, expert, or an LLM drafts the layer in an hour.»*
- **Неправильный порядок работы**: *«feature → customer-interview → value-check»*. Правильный: *«goal → diagnosis → hypothetical Job Graph → mechanic shortlist → research → real Job Graph → apply mechanics → RAT → validate → ship → loop.»* — [CLAUDE.md §5](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/CLAUDE.md)
- **Локальный и глобальный оптимум.** Локальный — когда не меняются сегмент, Core Jobs и бизнес-модель: *«Its growth is limited (+10–30%)»*. Глобальный — новый сегмент, новая Core Job или новая бизнес-модель. — [local-vs-global-optimum.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Next-Move-Theory/local-vs-global-optimum.md)
- **RAT**: *«risk priority = (probability wrong × cost if wrong) / cost to validate»*. *«Segments-and-Jobs is almost always the highest-leverage assumption.»* — [CLAUDE.md §4](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/CLAUDE.md)

**Структура канона** (~23 файла) — [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md)
- `Next-Move-Theory/`: nmt-key-theses, focus-as-company-attention-management, local-vs-global-optimum, subtraction.
- `Advanced-Jobs-To-Be-Done/`: ajtbd-key-theses, scientific-foundations, job-structure, job-graph, job-types-and-properties, critical-chain, value-creation, value-creation-mechanics, behaviour-change, customers-attention-management, consideration-activators, barrier-removal, communication, segmentation, b2b.
- `ABCDX-Segmentation/`, `Riskiest-Assumption-Test/`, `HowTos/` (basic-ajtbd-interview-guide-and-principles), `Algorithms/` (the-algorithm).
- Рекомендованный порядок чтения: nmt-key-theses → ajtbd-key-theses → rat-key-theses → abcdx.

**Лицензия**
- **CC BY-NC-SA 4.0**. Пояснение в README: применять методологию можно и в коммерческой компании. Ограничение NonCommercial касается только самого материала: *«reselling copies, bundling the text into a paid product or course, or putting it behind your own paywall.»* — [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md)

**Версии и история (CHANGELOG)** — [CHANGELOG](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/CHANGELOG.md)
- 0.6.13 (2026-06-20): установщик одной командой и скилл diagnose.
- 0.6.14 (2026-06-22): префикс `nmt-` и раздельные версии для Claude и Codex.
- 0.6.17 (2026-06-24): простой язык.
- 0.6.18 (2026-09-13):
  - «anti-hallucination pack»;
  - `nmt-upgrade` переименован в `nmt-update`;
  - правило *«purchase channel is not a segment, industry is not a segment when the Core Jobs and success criteria coincide»*.

**Прочее**
- Описание репозитория на GitHub (судя по поисковой выдаче) до сих пор упоминает *«a product advisor you can /ask-nmt»*. Это старое имя, сейчас скилл называется `/nmt-chat`. В поиске видны публичные форки (thisnikitas, ztemerbekov). — [GitHub (поисковая выдача)](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills)
- Есть статья на Medium «Next Move Theory: How Ivan Zamesin Built an Algorithm for Every Product Decision» (Семён Колосов). Видна только в выдаче, содержание недоступно. — [Medium](https://medium.com/@semyonkolosov/next-move-theory-how-ivan-zamesin-built-an-algorithm-for-every-product-decision-986659e5222c)
- Книга *The Nature of Product*, первая в серии, бесплатна на сайте и посвящена AJTBD. — [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md)

### Inferences
- **Лицензия важна для коммерческого продукта команды.** Применять идеи и запускать скиллы для клиентов можно. Включать тексты канона или скиллов в платный продукт или курс, а также в собственные платные скиллы-производные **нельзя без разрешения** автора: NC запрещает, а SA требует ту же лицензию для адаптаций. Если команда хочет сделать свои скиллы «на базе NMT», ей нужно либо писать их с нуля своими словами, либо договориться с автором (ivan@nextmovetheory.com).
- Шаги 1–4 алгоритма (Фаза I, «LLM drafts the layer in an hour») — то, что автор видео, по описанию задачи, делал с Claude. Фазы II–III (полевые интервью, RAT, продажи) из сессии с ИИ не закрываются. Это естественная зона ценности для живого фасилитатора.

### Gaps
- Содержимое сайта nextmovetheory.com (academy, cases, changelog, цены курсов) и русскоязычный Telegram-канал Замесина открыть не удалось. Дата первого публичного релиза канона (до v0.6.13) по клону глубины 1 не установлена.
- Заявления про «hundreds of companies», «dozens of documented cases», «13,000+» и «#1 эксперт» — самоописание автора, независимо не проверено.

---

## 6. AI-скиллы Next Move Theory: полный список, вход и выход, как использовать в Claude Code и Codex

### Takeaway
Скиллов 8, у каждого две версии: `Skills/claude/` (вызов `/nmt-…`) и `Skills/codex/` (вызов `$nmt-…`). Это два входа — **`/nmt-chat`** (советник) и **`/nmt-diagnose`** (диагностика живого продукта). Четыре скилла-«продюсера» образуют конвейер: **`/nmt-market-research` → `/nmt-craft-value-proposition` → `/nmt-product-requirements` и/или `/nmt-craft-go-to-market`**. Ещё два — **`/nmt-analyze-interviews`** и служебный **`/nmt-update`**. Скиллы читают канон из папки `Next-Move-Theory-Canon/` прямо во время работы. У продюсеров два режима: Quick (без интернета) и Deep (веб плюс параллельные суб-агенты). Результат — один файл в `Skills-Results/`. Сам автор подчёркивает: *«hypotheses, not conclusions»*.

### Cited Findings
**Таблица скиллов** (описания по README и frontmatter каждого SKILL.md):

| Скилл | Что делает (цитата / пересказ) | Вход → Выход |
|---|---|---|
| `nmt-chat` | *«A conversational advisor… Ask any product, strategy, segmentation, value, pricing, growth, positioning, B2B, or methodology question and get an answer grounded in the canon, not generic JTBD.»* Пять режимов: Explain / Diagnose / Pressure-test / Apply / Teach. | Любой текст («paste whatever you have») → ответ в чате и маршрут к нужному продюсеру. Файл создаётся только по просьбе. |
| `nmt-diagnose` | *«A chat-first diagnostic for live products. Through up to ~15 adaptive questions it challenges the goal you walked in with (climbing your business-Job graph for a higher-leverage move), then surfaces all the risks, all the growth points, and the risky assumptions hiding inside your current initiatives.»* | Контекст продукта (файлы в папке читаются только с разрешения) → ранжированный список рисков и точек роста, первый ход, маршрут к следующему скиллу. |
| `nmt-market-research` | *«Sizes the market and scores segments to answer "which Jobs of which segment should we compete for first?"»* | Идея → one-pager с вердиктом **GO / NARROW / PIVOT**, оценка сегментов по selection screen, прямые и косвенные конкуренты, план RAT, альтернативные рынки уровня Big Job. |
| `nmt-craft-value-proposition` | *«value hypotheses mapped over the Job Graph and the value-creation mechanics, filtered on feasibility, unit-economics, and competitiveness, ranked, with the top RAT cards.»* Конвейер S0–S6 с «гейтами» критика. | Результат market-research или ручное описание «сегмент + работы» → основное и дополнительное ценностное предложение, топ-3 RAT-карточки, спецификация, готовая к PRD. |
| `nmt-product-requirements` | Сначала гейт *«challenge the build»*: ищет более дешёвый способ достичь той же бизнес-цели. Потом пишет PRD. | Сегмент + ценность → PRD: функциональность (Core → Big → механика → критерии → Aha на критической цепочке) и пограничные случаи, покрывающие ~90% использования. |
| `nmt-craft-go-to-market` | *«landing-page copy, ad / creative formulas, and an acquisition + growth-communication plan (channels loaded with Consideration Activators, lead magnets, viral loops, retention messaging).»* Всё через Big Job, *«features as proof not message»*. | Ценностное предложение, PRD или market-research → тексты лендинга, рекламы, GTM-план. |
| `nmt-analyze-interviews` | *«extracts the AJTBD structure: segments by Core Jobs, personas, existing Solutions and Problems, a Consideration Set, and value hypotheses — each with an honest confidence — plus a gap list.»* | Транскрипты, заметки, звонки продаж и поддержки, открытые ответы опросов → отчёт из 9 разделов (качество данных, сегменты, решения и проблемы, consideration set, гипотезы, единичные сигналы, приложение, пробелы). |
| `nmt-update` | Обновляет канон, скиллы и блок правил, перезапуская официальный установщик с GitHub. Раньше назывался `nmt-upgrade`. | — |

Источники: [README «The skills»](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md); [Skills/claude/*/SKILL.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/tree/main/Skills/claude)

**Маршруты** (по README):
```
new idea → /nmt-chat → /nmt-market-research → /nmt-craft-value-proposition → /nmt-product-requirements → /nmt-craft-go-to-market
live product → /nmt-diagnose
interviews on disk → /nmt-analyze-interviews
update everything → /nmt-update
```
— [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md)

**Установка**
- Команда: `curl -fsSL https://raw.githubusercontent.com/zamesin/Next-Move-Theory-Canon-and-Skills/main/install.sh | bash` (для Windows — `install.ps1`).
- Скиллы ставятся в `.claude/skills/` (Claude Code) и `.agents/skills/` (Codex). Канон кладётся в корень проекта под именем `Next-Move-Theory-Canon/`, и это имя менять нельзя.
- В `CLAUDE.md` и `AGENTS.md` между маркерами `<!-- Next-Move-Theory-Rules:start/end -->` вставляется блок из 5 строк.
- Предупреждение агентам: *«do not stop at git clone»*.

Источники: [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md); [install.sh](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/install.sh)

**Блок правил, который вставляется в CLAUDE.md**:
> «Methodology source of truth: ./Next-Move-Theory-Canon/ — for product/strategy work always prefer it over generic Jobs To Be Done knowledge (the definitions differ substantially). New here? Start with /nmt-chat… Skill outputs go to Skills-Results/.»

Источник: [install.sh](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/install.sh). Полный файл правил для агентов (`CLAUDE.md` / `AGENTS.md`, около 28 КБ) лежит в корне репозитория — [CLAUDE.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/CLAUDE.md).

**Producer contract** — 11 обязательных поведений всех продюсеров ([PRODUCER-CONTRACT.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Skills/claude/PRODUCER-CONTRACT.md)):
1. «Вид с вертолёта» до первого вопроса.
2. Выбор формата: Markdown или HTML.
3. *«Critical treatment of all user input — everything the user provides is a hypothesis».*
4. Видимый «долг валидации»: вердикт `GO` превращается в `GO (to validation)`.
5. Настраиваемый путь вывода.
6. QA-цикл в Deep-режиме.
7. Обязательный вопрос о рынке и языке.
8. Чтение файлов в папке только с разрешения.
9. Статус каждого утверждения: цитата / вывод / гипотеза модели.
10. Частоты в агрегированных утверждениях: *«a single source can't carry a segment».*
11. Уверенность пропорциональна объёму входных данных.

**Как устроены выводы**
- Трёхслойный формат: Layer 1 — ответ на одной странице; Layer 2 — обоснование; Layer 3 — полный пакет.
- Путь к файлу: `Skills-Results/{product-slug}/market-research/{YYYY-MM-DD_HH-MM}_…-result.{md|html}`.

Источник: [nmt-market-research/SKILL.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Skills/claude/nmt-market-research/SKILL.md)

**Особенности `nmt-diagnose`** ([nmt-diagnose/SKILL.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Skills/claude/nmt-diagnose/SKILL.md))
- Шаг 1 — обязательный гейт: *«Do not accept the task the user walked in with… Ask "Why do you want this? In order to do what?" and trace it up 3–5 levels (5 Whys)… At each level up, look for a better move.»*
- Затем выбор: *«Tune vs. bigger bet»*.
- Затем проход по всей цепочке к прибыли с таблицей «симптом → обычная настоящая причина». Например: *«Low / falling conversion → Wrong Segment+Job, or value doesn't beat alternatives».*
- Отдельно есть *«growth-points lens»*: Previous/Next Jobs, подъём на уровень, Small Jobs соседнего сегмента, kill-a-Job.

**Телеметрия**
- В конце работы скилл проверяет, вышла ли новая версия. Отправляются только имя скилла и версия.
- Отключается тремя способами: `update-check: off` в `.nmt-config`, `DO_NOT_TRACK=1` или `NMT_NO_UPDATE_CHECK=1`.

Источник: [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md)

**Старые имена скиллов**
- [Сводка поиска, низкая уверенность, первоисточник не установлен] Раньше автор описывал «six Claude Code skills including /ask-nmt as a conversational AI CPO, /market-research, and /diagnose». Это имена до переименования в `nmt-` (v0.6.14, 2026-06-22). — [поиск: X / Telegram Замесина](https://x.com/zamesin)

### Inferences
- Набор для «стратегии соло-проекта» в духе видео:
  1. `/nmt-chat` — сбор контекста.
  2. `/nmt-diagnose`, если продукт уже живой, или `/nmt-market-research`, если это новая идея.
  3. `/nmt-craft-value-proposition`.
  4. `/nmt-analyze-interviews` после реальных интервью.
  5. `/nmt-craft-go-to-market`.
  
  «Диагностика» и «исследование рынка», которые упомянуты в описании видео, соответствуют `/nmt-diagnose` и `/nmt-market-research`. Если видео записано до июня 2026, в нём могут звучать старые имена (`/ask-nmt`, `/market-research`, `/diagnose`).
- Все скиллы задают вопросы пачками через `AskUserQuestion` и рассчитаны на продуктовые решения: что строить и кому продавать. Под «стратегию проекта» (личные цели основателя, ресурсы, ритм, командные договорённости в духе S3) они напрямую не заточены. Это ниша, которую можно занять своими скиллами или фасилитацией.

### Gaps
- Codex-версии я не читал построчно. По README они отличаются только механикой: *«structured questions, parallel sub-agents»*.
- Опубликованных разборов стратегического применения скиллов (кейсов) получить не удалось: nextmovetheory.com/cases и видео заблокированы.

---

## 7. obra/superpowers: что это и что делает скилл brainstorming (по шагам); как его применить к стратегии

### Takeaway
`obra/superpowers` (Jesse Vincent / Prime Radiant, лицензия MIT, v6.4.2 от 2026-09-25) — *«a complete software development methodology for your coding agents»*, набор составных скиллов. Скилл **brainstorming** превращает идею в согласованный дизайн или спецификацию **до** начала реализации. Порядок работы:
1. Выяснить намерение и записать его, чтобы человек мог поправить.
2. Классифицировать задачу (spike / bounded / architectural).
3. Задавать уточняющие вопросы **по одному**, лучше с вариантами ответа.
4. Предложить **2–3 подхода** с компромиссами и рекомендацией.
5. Показать дизайн секциями с одобрением после каждой.
6. Записать спецификацию, провести self-review и получить одобрение.
7. Передать работу скиллу writing-plans.

Между этапами стоят жёсткие «гейты».

### Cited Findings
- Что такое Superpowers: *«Superpowers is a complete software development methodology for your coding agents, built on top of a set of composable skills»*. *«As soon as it sees that you're building something, it doesn't just jump into trying to write code. Instead, it steps back and asks you what you're really trying to do.»* Скилл распространяется через официальный маркетплейс плагинов Claude и поддерживает Codex, Cursor, Gemini CLI и другие среды. Лицензия MIT, «Copyright (c) 2025 Jesse Vincent». — [README](https://github.com/obra/superpowers/blob/main/README.md); [LICENSE](https://github.com/obra/superpowers/blob/main/LICENSE)
- Frontmatter скилла: `description: "You MUST use this before any creative work - creating features, building components, adding functionality, or modifying behavior. Explores user intent, requirements and design before implementation."` — [skills/brainstorming/SKILL.md](https://github.com/obra/superpowers/blob/main/skills/brainstorming/SKILL.md)

**Шаг 0 — «Establish Shared Understanding»** ([SKILL.md](https://github.com/obra/superpowers/blob/main/skills/brainstorming/SKILL.md))
1. *«Discover intent… ask one focused question about purpose or intended use before proposing features».*
2. *«Write back your understanding… Separate what they said from assumptions. Invite correction».*
3. *«Carry intent into the design».*

Этот шаг добавлен в v6.4.1 (2026-09-18): *«Brainstorming finds out why you want the thing before proposing features»*. — [RELEASE-NOTES](https://github.com/obra/superpowers/blob/main/RELEASE-NOTES.md)

**Три пути**, которые скилл объявляет вслух ([SKILL.md](https://github.com/obra/superpowers/blob/main/skills/brainstorming/SKILL.md))
- **Spike** — вопрос о выполнимости, ответ без кода, который останется.
- **Bounded** — небольшое изменение уже существующего кода, дизайн коротко в чате.
- **Architectural** — полный процесс.
- *«When in doubt between two paths, take the heavier one.»*
- Пути появились в v6.3.0 (2026-08-12): *«Ceremony now scales to the task.»* — [RELEASE-NOTES](https://github.com/obra/superpowers/blob/main/RELEASE-NOTES.md)

**Чек-лист для пути Architectural** ([SKILL.md](https://github.com/obra/superpowers/blob/main/skills/brainstorming/SKILL.md))
1. Explore project context.
2. Предложить визуального компаньона (браузерные мокапы), но *«just-in-time»*, а не заранее.
3. *«Ask clarifying questions — one at a time, understand purpose/constraints/success criteria».*
4. *«Propose 2-3 approaches — with trade-offs and your recommendation».*
5. *«Present design — in sections scaled to their complexity, get user approval after each section».*
6. Записать дизайн-документ в `docs/superpowers/specs/YYYY-MM-DD-<topic>-design.md` и закоммитить.
7. Spec self-review: *«Placeholder scan… Internal consistency… Scope check… Ambiguity check»*.
8. Пользователь проверяет спецификацию.
9. Вызов writing-plans.

**Ключевые правила** ([SKILL.md](https://github.com/obra/superpowers/blob/main/skills/brainstorming/SKILL.md))
- *«Only one question per message»*; *«Prefer multiple choice questions when possible»*.
- *«Lead with your recommended option and explain why»*; *«YAGNI ruthlessly»*.
- Большой проект сначала декомпозируется: *«help the user decompose into sub-projects»*.
- HARD-GATE: до одобрения нельзя ни писать код, ни что-либо скаффолдить. *«A reply approves the stage actually presented. Approval of an idea or feature scope does not approve artifacts that do not exist yet.»*
- Таблица Red Flags, например *«"This is too simple to need a design"»*.

### Inferences
- Как перенести brainstorming на стратегическую работу (это мои выводы, а не текст скилла):
  - сначала намерение и критерии успеха;
  - по одному вопросу за раз, с вариантами ответа;
  - 2–3 альтернативных стратегических хода с компромиссами и рекомендацией;
  - стратегия показывается секциями и согласуется по частям;
  - письменный стратегический документ проходит self-review (заглушки, противоречия, масштаб, двусмысленности);
  - жёсткий гейт «не исполнять, пока документ не одобрен».
  
  Это хорошо стыкуется с NMT: «challenge the goal» соответствует «discover intent», а Фаза I алгоритма — шагу «propose approaches».
- Ограничение: скилл явно рассчитан на софт (разделы «architecture, components, data flow, error handling, testing» и переход к writing-plans). Для стратегии его надо адаптировать: вместо writing-plans — план RAT и экспериментов, вместо спеки кода — стратегический документ.
- Если в видео использовали версию до августа 2026, поток был проще и без трёх путей: контекст → вопросы по одному → 2–3 подхода → дизайн секциями → документ.

### Gaps
- Какую именно версию superpowers использовал автор видео, установить нельзя: видео недоступно.

---

## 8. Конкретные примеры формулировок Core/Big Job (B2B-услуги, консалтинг, основатели, стратегия, принятие решений)

### Takeaway
В публичном английском каноне почти нет готовых Core/Big формулировок именно для стратегического консалтинга. Есть несколько близких примеров: консультант по личному бренду, основатель, который «нанимает PM», личные работы B2B-заказчика, ABCDX в HR-консалтинге, AJTBD-курс со многими Big Jobs, ученик со Scrum (вторичный источник). Примеры для продукта команды ниже — **мои гипотезы**, их нужно проверить интервью.

### Cited Findings
- Консалтинг, уровни работ: *«A consultant who delivers "build your personal brand" turnkey has that as a Core Job. An agency that only "writes your LinkedIn posts" has the same Job two levels lower.»* — [job-graph.md §2](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md)
- Основатель: заявленная «проблема» — *«hire a Product Manager»*, а работа под ней — *«save a failing product»*. — [ajtbd-key-theses.md §7](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- Лесенка для PM: *«I set up the experimentation platform → in order to ship features without breaking production → in order to hit the quarter's roadmap commitments → in order to get promoted to Group PM.»* — [job-graph.md §17](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/job-graph.md)
- Соло-разработчик (пример из раздела про активаторы): *«A solo developer who'd shipped three products in a year — none of them past initial revenue — paused, ran two weeks of customer-research interviews… found the one Big Job they had actually paid for, rebuilt around it. First paying customer of the new product within a month.»* — [consideration-activators.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/consideration-activators.md)
- Пять личных работ B2B-заказчика (*«won't get me blamed or fired»* и т.д.) — см. раздел 3. — [ajtbd-key-theses.md §25](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- Образовательный продукт: Core *«learn product methodology»*, Big Jobs *«grow my career, build a side project, consult, become a respected practitioner»*. — [value-creation-mechanics.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/value-creation-mechanics.md)
- Пример конкретного допущения RAT для соло-основателей: *«A US segment of solo founders and 2-to-3-person engineering teams at YC-stage B2B SaaS startups exists — currently spending weeks of engineering time integrating PayPal… and would pay 2.9% + $0.30 per transaction…»* — [rat-key-theses.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Riskiest-Assumption-Test/rat-key-theses.md)
- ABCDX в бутиковом консалтинге: A-клиенты — executive search с бюджетом ~$450K/мес против ~$150K у mid-market. Результат: +60% выручки за 3–4 месяца. — [abcdx-segmentation-key-theses.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/ABCDX-Segmentation/abcdx-segmentation-key-theses.md)
- [RU, вторичный источник: пост ученика, через поиск] Core Job «освоить подход Scrum»; Big Job «стать востребованным специалистом, способным обеспечивать ритмичную поставку инкрементов продукта командой через внедрение Scrum». — [setka.ru (через поиск)](https://setka.ru/posts/01942a83-dcbd-494e-a79d-384f780fc241)

### Inferences
Черновики-гипотезы в грамматике канона для продукта «стратегия для соло-проектов и AI-native команд». **Не из источников, проверить интервью с теми, кто платил.**
- **Core Job (кандидат)**, если продукт — фасилитированная сессия + AI-скиллы: «Я хочу **выбрать следующий стратегический ход** для проекта на ближайшие 4–12 недель с критериями успеха:
  - решение принято за ≤ N часов моего времени;
  - рассмотрено ≥ 3 альтернатив с явными компромиссами;
  - названо самое рискованное допущение и дешёвый тест к нему;
  - есть понятный первый шаг на завтра;
  
  — чтобы {Big Job}».
- **Big Job (кандидаты; продукт вносит вклад, но не выполняет их полностью)**:
  - «вывести соло-проект на устойчивую выручку, при которой можно не возвращаться в найм»;
  - «перестать распыляться между идеями и довести одну до первых платящих»;
  - для AI-native команды: «синхронно двигаться к одной цели без раздутых процессов».
- **Small Jobs (сестринские, тот же уровень, что Core)**: провести интервью с клиентами, собрать лендинг или оффер, посчитать юнит-экономику, договориться о ролях и ритме в команде (S3-практики). Это потенциальные точки роста: захват Previous или Next Job.
- **Micro Jobs**: собрать контекст, сформулировать гипотезы сегментов, приоритизировать ходы и т.д.
- Тест подъёма для фасилитатора. Если сессия выдаёт только документ, Core — «выбрать ход». Если в цену входят сопровождение RAT-экспериментов и валидация продаж, Core можно поднять до «проверить и запустить ход».

### Gaps
- Опубликованных Замесиным или его учениками формулировок Core/Big Job именно для стратегического консалтинга, фасилитации или соло-основателей в доступных источниках не найдено. Русские кейсы (zamesin.ru, nextmovetheory.com/cases) недоступны.

---

## 9. Критика Advanced JTBD и отличия от классического JTBD (Кристенсен, Ulwick ODI, Клемент)

### Takeaway
Сам Замесин подаёт AJTBD как методологию, **построенную с нуля** «чтобы получить алгоритм», и прямо запрещает агентам импортировать определения Кристенсена, Ульвика и Моесты. Главные отличия:
- Job — это переход A→B из 8 элементов с **критериями успеха**, а не «прогресс в обстоятельствах».
- Есть граф работ с уровнями, определёнными относительно продукта.
- Сегментация идёт по графу работ.
- Ценность определена через энергоэффективность и prediction error.
- Четыре силы прогресса отправлены в архив.
- Методология встроена в NMT вместе с юнит-экономикой, RAT, ABCDX и TOC.

Внешнюю критику в этой сессии удалось увидеть только во фрагментах. Основные слабые места: научная база — авторская гипотеза; данные об эффективности — самоотчёт; большая часть методологии закрыта и платная; интервью плохо достают неосознаваемые мотивы (это признаёт сам канон).

### Cited Findings
- *«Existing JTBD interpretations were deliberately not adopted… The full AJTBD canon stands on ~1,000 theses, most of them diverging from other JTBD interpretations.»* — [ajtbd-key-theses.md, вступление](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- *«Do not import Christensen / Ulwick / Moesta definitions. AJTBD diverges substantially.»* Работа — *«not "the customer's struggle for progress"»*. — [CLAUDE.md §1](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/CLAUDE.md)
- История от автора: *«I went deep into Jobs To Be Done and kept its deepest intuition: a person sits in a situation and wants to transition into a different state. I left the rest of the machinery behind, because it never told me how to research, segment, choose where to compete, or create value.»* — [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md)
- Four Forces объявлены устаревшими: *«there are more than four forces, and a Problem with the current Solution is usually the trigger… rather than a force in steady state.»* — [ajtbd-key-theses.md §21](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md)
- Научная база — это гипотеза автора. В каноне ссылка на *«AJTBD's key hypothesis of value»* в scientific-foundations §2; опора — работы Лизы Фельдман Барретт (аллостаз, reward prediction error). — [ajtbd-key-theses.md §6](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md); [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md)
- Ограничения, которые признаёт сам канон:
  - интервью плохо достают неосознаваемые мотивы (статус, идентичность), и их предлагается проверять продажами или A/B-тестами — [interview guide §1](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/HowTos/basic-ajtbd-interview-guide-and-principles.md);
  - освоение требует практики: *«on the order of ~100 honest mistakes»* — [ajtbd-key-theses.md](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/Next-Move-Theory-Canon/Advanced-Jobs-To-Be-Done/ajtbd-key-theses.md);
  - скиллы дают *«hypotheses, not conclusions»* — [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md).
- [Сводка поиска, вторичный источник] Обзор GoPractice «Jobs to Be Done: разные подходы за общим названием» называет AJTBD Замесина отдельной, популярной в русскоязычной среде интерпретацией рядом с теорией Кристенсена, Demand-Side Sales Моесты, ODI Ульвика и подходом Клемента. В сводке Ульвик описан как количественный подход с выборками («86%» успеха по данным Strategyn), полезный в B2B, а Клемент — как формализация мотивации через интервью, ближе к B2C. — [GoPractice (через поиск)](https://gopractice.ru/product/jtbd-the-theory-and-the-frameworks/)
- [Сводка поиска, атрибуция неясна: GoPractice или страницы Замесина] Упомянутые недостатки или ограничения:
  - *«none of the book and article authors on JTBD provided step-by-step algorithms»* — похоже, это критика классического JTBD самим Замесиным, мотивация создать AJTBD;
  - *«at the highest level of the graph are needs that people are not aware of»*;
  - подход *«not suitable for products based on dopamine cycles»*.
  
  — [поисковая сводка по gopractice.ru / zamesin.ru](https://zamesin.ru/producthowto/book/introduction-to-advanced-jobs-to-be-done/)

### Inferences
Сравнение с классическими подходами — мой синтез по канону и общему знанию; подходы Кристенсена, Ульвика и Клемента в этой сессии по первоисточникам не проверялись.
- **Кристенсен / Моеста**: «progress in circumstance», Four Forces, switch-интервью. В AJTBD то же интервью о переключении сохранилось (*«this is where a switch interview fits»*), но появились граф работ, уровни, критерии с порогом и сегментация по графу.
- **ODI Ульвика**: job map и desired outcome statements с направлением и метрикой, количественные опросы. «Success criteria = direction + level» в AJTBD концептуально близки к desired outcomes ODI. Но AJTBD опирается на качественные интервью (около 60) и продажу на интервью, а не на количественный opportunity score.
- **Клемент (Job Stories, «When…, I want to…, so I can…»)**: внешне похоже на Level 2 у Замесина. Но канон требует «in order to» с **работой уровнем выше**, обязательными **критериями успеха** и явным уровнем (Core/Big и т.д.). В Job Story нет ни критериев, ни уровня.
- Риски для команды:
  - зависимость от одного автора, при этом канон открыт лишь на ~25%;
  - быстро меняющаяся терминология (NMT v0.6 — «in active development»);
  - нейронаучная база — авторская интерпретация;
  - лицензия NC ограничивает коммерческое переиспользование текстов.

### Gaps
- Полные тексты внешней критики AJTBD на русском (Habr, vc.ru, GoPractice, Telegram) недоступны: заблокированы прокси. Систематической независимой оценки эффективности AJTBD или NMT не найдено.
- Первоисточники Кристенсена, Ульвика и Клемента в этой сессии не открывались. Сравнение выше — вывод, а не цитата.
