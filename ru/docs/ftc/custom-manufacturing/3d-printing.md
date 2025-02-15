# 3D Печать

## Виды 3D Печати

Существует несколько различных видов 3D печати. FDM (Fused Deposition Modeling) (также известная как Fused Filament Fabrication) экструдирует расплавленный филамент для создания детали и является самым распространенным типом, на котором мы сосредоточимся в этом руководстве. SLA (стереолитография) и SLS (Selective Laser Sintering) — это другие варианты 3D печати пластиков, но они обычно более сложные, дорогие или имеют другие недостатки в приложениях FTC |reg|. По этим причинам они не рекомендуются.

Металлическая 3D печать (SLS и другие) также становится все более доступной, но она не рассматривается в рамках этого руководства.

> Рекомендуем ознакомиться с [разделом 3D печати в документации FTC](https://ftc-docs.firstinspires.org/en/latest/manufacturing/3d_printing/index.html), руководством по FDM 3D печати в рамках FTC. Оно охватывает такие темы, как: сцепление с платформой, допуски, проектирование для 3D печати, настройка и выбор оборудования.

## Преимущества 3D Печати

- 3D печать позволяет настраивать размеры и идеально оптимизировать детали; например, команды могут напечатать катушку нужного диаметра для достижения оптимальной скорости или шкив с определенным количеством зубьев.
- 3D печать позволяет командам адаптировать детали между комплектами и индивидуальными частями, так как не все комплекты имеют адаптируемые крепления или кронштейны. Хороший пример — адаптеры для механум-колес Nexus, которые команды 3D печатают.
- 3D печать позволяет командам изготавливать детали, которые были бы невозможны для изготовления с помощью таких материалов, как алюминий, из-за ограничений обработки.
- 3D печать позволяет командам создавать индивидуальные решения для защиты проводов и соединений от напряжений. Это отличный проект, который стоит потратить время.

## Недостатки 3D Печати

- **Если на соревнованиях у вас нет запасных 3D напечатанных частей, скорее всего, вам не повезет. Командам рекомендуется печатать хотя бы один комплект каждой 3D напечатанной детали как запасные части для соревнований.**
- 3D напечатанные компоненты обычно слабее других материалов, таких как алюминий. Однако печать в правильной ориентации может обеспечить большую прочность — команды печатали крюки и другие детали, которые выдерживают нагрузки на роботе FRC |reg| (120 фунтов) и FTC (40 фунтов).
- 3D напечатанные детали должны подвергаться нагрузке только в одной ориентации. То есть, если робот висит на крюке, нагрузка должна идти только на нижнюю сторону изогнутой части крюка. Постарайтесь минимизировать боковые нагрузки, чтобы избежать поломки детали.
- Размер 3D напечатанных частей ограничен размером вашей печатной платформы.
- Большие и толстые детали могут печататься долго (ночью), что повышает риск неудачи.
- 3D печать может быть довольно дорогой, хотя филамент можно найти по разумной цене у онлайн-продавцов, таких как Amazon.

## Распространенные Филаменты

Для большинства деталей, которые необходимо напечатать для FTC, **PLA (или PLA+, Pro и т.д.) и/или PETG полностью удовлетворяют все требования к прочности, долговечности и эстетике.** Эти два типа филаментов являются самыми простыми в печати и продаются множеством производителей по разумным ценам. Большинство других филаментов имеют очень специфические преимущества (например, TPU), которые требуют больше усилий, времени и денег.

!> **Предупреждение**: Если в вашем экструдере (часть, которая расплавляет филамент) используется PTFE (Тефлон), и PTFE трубка идет прямо до нагревательного блока (что часто встречается в недорогих принтерах, таких как Ender 3 и его варианты), то **не следует печатать при температуре 250 градусов Цельсия и выше**. Это приведет к разрушению PTFE трубки и выделению токсичных паров. Если вам нужно печатать при таких температурах, и у вас экструдер с PTFE трубкой, вы можете рассмотреть возможность обновления до экструдеров с полностью металлическим нагревателем.

### PLA (Полиактид)

Самый распространённый 3D-печатный филамент — полиактид, или PLA. Это пластик, изготовленный из биологических источников, таких как кукурузный крахмал и сахарный тростник. PLA жёсткий, но более хрупкий по сравнению с другими вариантами филамента и, как правило, не имеет или имеет минимальное количество деформации при печати. PLA хорошо подходит для большинства частей роботов, но может не выдерживать ударные нагрузки (удачные на детали), и поэтому детали следует проектировать соответствующим образом.

- Температура экструдера PLA: 190 |deg|–230 |deg| C
- Температура стола PLA: 20 |deg|–60 |deg| C, но наличие подогреваемого стола для PLA не является обязательным

> Из-за относительно низкой температуры плавления PLA не рекомендуется оставлять PLA-части в таких местах, как горячая машина, так как это может привести к сильному искривлению этих частей.

Существует множество разновидностей PLA, продающихся разными производителями, например PLA+ или PLA Pro. Эти филаменты содержат различные добавки для улучшения прочности, печатности и других свойств. Хотя они более дорогие, такие продукты могут значительно улучшить характеристики PLA и устранить его слабые места.

### PETG (Полиэтилентерефталат гликоль)

PETG можно описать как улучшенную версию PLA по прочности. Он несложен в печати, но часто вызывает заметное образование нитей и другие мелкие артефакты. Хотя его прочность на растяжение теоретически ниже, чем у PLA, он гораздо менее хрупкий и лучше сопротивляется ударам за счёт легкой гибкости. Это отличный выбор для деталей FTC, которые должны быть устойчивы к ударам, в то время как PLA не выдержит. Более высокая температурная стойкость также означает, что он не будет деформироваться при высокой окружающей температуре, такой как в горячей машине.

> PETG известен отличной адгезией к печатным столам, **особенно стеклянным и PEI**, и часто рвёт куски с поверхности стола. Рекомендуется использовать клейкую палочку или лак для волос перед печатью.

- Температура экструдера PETG: 230 |deg|–260 |deg| C
- Температура стола PETG: 60 |deg|–80 |deg| C

## Менее распространённые филаменты

Эти филаменты используются реже, чем те, что указаны выше, но могут найти множество применения в роботах FTC. Обычно их используют из-за специфических свойств материала, таких как гибкость или долговечность. Однако, они часто сталкиваются с серьёзными проблемами при печати, которые могут помешать использовать их на принтерах "из коробки", а также они часто гораздо дороже.

### ABS (Акрилонитрилбутадиенстирол)

ABS был стандартным филаментом для печати до появления PLA в коммерческом доступе. Возможно, вы использовали ABS для деталей конструктора LEGO |reg|. Этот материал выдерживает высокие нагрузки и обладает хорошей вязкостью. Это достигается за счёт трудности печати, где часто необходима камера для поддержания температуры и предотвращения сильной деформации деталей. Преимущества по прочности, которые можно получить от PLA, проще найти в PETG, поэтому детали из ABS реже используются в FTC. Тем не менее, ABS довольно доступен и продаётся по той же цене, что и PLA.

- Температура экструдера ABS: 230 |deg|–250 |deg| C
- Температура стола ABS: 100 |deg|–120 |deg| C
- Рекомендуется использовать камеру для предотвращения деформации

Из-за трудностей печати ABS и его ограничений, можно рассматривать альтернативы, такие как ASA, которые предлагают похожие свойства с гораздо лучшей печатностью.

### TPU/TPE (Термопластичный полиуретан/Термопластичный эластомер)

TPU и TPE — это распространённые филаменты для печати, широко используемые благодаря своим гибким свойствам. Это позволяет создавать печатные детали, которые легко сгибаются и растягиваются. Эти материалы продаются с разными дюрометрами (мерой жесткости/гибкости материала по шкале Shore), а их высокая ударная стойкость и сцепление слоёв делают их не только универсальными, но и чрезвычайно прочными. В FTC команды используют TPU/TPE для создания накладок для захватов вместо трубок, а также для изготовления нестандартных ремней для применения с низкими нагрузками.

> Из-за своей гибкости принтерам с системой экструзии через Bowden-трубку, где двигатель экструдера не находится на горячем конце, будет чрезвычайно сложно печатать TPU/TPE.

- Температура экструдера TPU/TPE: 210 |deg|–250 |deg| C
- TPU/TPE обычно не требует подогреваемого стола, но если он используется, температура не должна превышать 60 |deg| C, так как это может сплавить TPU с печатным столом.
- TPU/TPE имеет склонность к поглощению влаги из воздуха, и его, вероятно, придётся сушить перед печатью и, возможно, в процессе печати.
- Рекомендуется использовать экструдер с прямым приводом

## Экзотические филаменты

Эти филаменты редко используются в FTC. Они обладают выдающимися материалами для деталей, которые должны подвергаться высоким силам и неблагоприятным условиям. Они все значительно дороже, чем вышеупомянутые филаменты, и обладают множеством сложностей при печати.

### Нейлон

Нейлоновые филаменты могут быть с добавлением стекловолокна, углеродного волокна или чистыми. Нейлон — это лидер по устойчивости к ударам в ситуациях, где деталь может согнуться, а не полностью сломаться. Иногда нейлон используется для таких частей, как крышки колёс в трансмиссиях и в местах, где детали будут подвергаться частым ударам. Нейлон требует очень высоких температур, обычно требует камеры и обязательно должен быть высушен перед (и во время) печати.

- Температура экструдера нейлона: 240 |deg|–260 |deg| C
- Температура стола нейлона: 55 |deg|–80 |deg| C
- Нейлон известен тем, что сильно поглощает влагу из воздуха и должен быть тщательно высушен перед и во время печати. Несоблюдение этого требования, вероятно, приведёт к непригодности детали.
- Рекомендуется использовать камеру

### Наполненные углеродным волокном

Многие филаменты также продаются с добавлением небольших частиц углеродного волокна, смешанных с самим филаментом. Хотя их часто воспринимают как улучшение прочности, на самом деле эти филаменты предназначены для повышения жесткости и улучшения печатности таких материалов, как нейлон. Филаменты, наполненные углеродным волокном, обычно требуют более высоких температур и закаленных стальных сопел, но если вы можете печатать с чистыми вариантами этих филаментов, вы также сможете печатать с их углеродно-волокнистыми аналогами.

### Поликарбонат (PC)

Поликарбонат и его варианты являются очень прочными, техническими материалами. Поликарбонат особенно выделяется своей способностью быть очень жестким и хорошо выдерживать удары. Поликарбонат также требует, чтобы материал был сухим, наличие принтера, способного работать при **очень** высоких температурах, и камеры для печати. Это очень сложный материал для печати, и он часто очень дорогой. В FTC практически нет случаев, когда требуется использование поликарбонатных частей, так как их прочности недостаточно для таких задач.

Существуют несколько смесей PC, которые значительно легче печатать, одним из ярких примеров является PolyMaker PolyMax PC. Это более легкая для печати версия с более низкими температурами, но сохраняющая многие преимущества чистого поликарбоната. PolyLite не такая ударопрочная, но гораздо дешевле. Оба варианта намного легче печатать, чем чистый PC.

- Температура нагрева экструзера PC: 250 |°C| - 320 |°C|
- Температура нагрева стола PC: 80 |°C| - 140 |°C|
- Требуется камера для печати
- Филамент должен храниться в сухом месте

### Премиум экзотические филаменты

Существуют и другие материалы с высокими показателями, которые могут существенно расширить возможности 3D печати, но они не должны использоваться, если вы не *очень* уверены в своих навыках печати, и, как правило, они не пригодятся в FTC. К таким материалам относятся, но не ограничиваются: Delrin (Полиоксиметилен Гомополимер Ацеталь), PEI (Полиэфиримид, бренд ULTEM), PEEK (Полиэфирэфиркетон) и PEKK (Полиэфиркетонкетон). Эти материалы крайне сложны в печати, требуют невероятных температур (некоторые настолько высоких, что закаленная стальная насадка начинает плавиться) и чрезвычайно дорогие.

### Руководство по проектированию для 3D печати

Вот краткое руководство по проектированию 3D напечатанных частей, которое может быть полезно для команд, которые не знакомы с 3D частями.

Первое, что нужно учитывать при проектировании 3D напечатанных частей, — это ориентация печати. Это касается стороны, которая будет контактировать с печатной платформой. Желательно, чтобы деталь имела плоское дно для максимального контакта с платформой.

>**Совет**: Максимизация контакта с платформой обеспечит, чтобы деталь не отслоилась и не деформировалась при печати, а также повысит качество печати.

Если невозможно сделать деталь с плоской стороной для печати, простое решение — разделить деталь на несколько частей вдоль плоскости. Например, нижняя плата редуктора на изображении ниже не имела плоской стороны для печати, поэтому она была разделена пополам. Позже части были соединены с помощью множества винтов и пластикового клея. Если бы эта плата была напечатана как одно целое, пришлось бы использовать поддержку для создания всех необходимых отверстий. Детали, не использующие материал поддержки, гарантируют минимальные потери пластика.

![3D напечатанный редуктор, напечатанный в 2 частях, разделенных по плоскости](https://dd8f408.webp.ee/2-piece-gearbox.jpg)  
*3D напечатанный редуктор, напечатанный в 2 частях, разделенных по плоскости*

>**Совет**: Не стоит делать фаски или округлять края первого слоя на нижней поверхности детали. Фаски или округления увеличат вероятность деформации детали, особенно на неподогреваемых платах.

### Угол наклона

Угол наклона относится к углу выступающей стороны детали по отношению к нормали поверхности печатной платформы. Максимальный угол наклона — это максимальный угол, который принтер может напечатать без использования материала поддержки. Этот угол зависит от принтера, настроек печати (особенно скорости, температуры и охлаждения) и типа филамента. Чтобы уменьшить использование материала поддержки, следует учитывать каждый угол наклона и убедиться, что он находится в пределах максимального угла наклона. Соблюдение этого угла также уменьшит вероятность деформации детали.

### Напряженные векторы

Один из важнейших аспектов — это векторы напряжений. 3D напечатанные детали по своей природе сильнее на двух осях и слабее на одной оси. Слабая ось возникает из-за слоистой структуры, характерной для технологии FDM печати. Обычное решение — это увеличение температуры печати до определенного предела, пока это не начнет ухудшать качество печати. Однако слабую ось можно укрепить, опять же разделив деталь на несколько частей. Суть в том, чтобы усилить часть конструкции, оптимизируя ориентацию на плоскости, на которой она печатается. Например, эта сборка ниже была ответственна за подвешивание всего робота, поэтому она должна была быть максимально прочной для 3D напечатанных деталей.

>**Совет**: Может показаться нелогичным разделить деталь на несколько частей для увеличения прочности, но за этим стоит определенная логика.

Деталь можно было бы легко напечатать как одну часть, но она была бы довольно слабой, если на нее воздействовали бы силы в вертикальном направлении. Разделив деталь и создав новые плоские поверхности для печати, можно усилить каждую ось. *Если одна небольшая деталь выйдет из строя, робот все равно может продолжать работать.* Это предпочтительнее, чем полное разрушение всей детали. В этом примере боковые части были напечатаны как отдельные детали на взаимодополняющей оси для укрепления сборки.

![Многокомпонентная сборка для 3D печати](https://dd8f408.webp.ee/printing-multipart.jpg)  
*Многокомпонентная сборка для 3D печати*

![Собранная версия многокомпонентных частей](https://dd8f408.webp.ee/assembled-multipart.jpg)  
*Собранная версия многокомпонентных частей, которые печатались на предыдущем изображении*

Эта сборка является хорошим примером того, как учитывать ориентацию деталей, углы наклона и векторы напряжений в каждой части дизайна. Сложные детали можно сделать прочными и без использования поддержки, просто правильно разделив их.
