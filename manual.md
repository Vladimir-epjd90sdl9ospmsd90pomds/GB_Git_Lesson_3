# Введение в Git

___Git - это самая популярная распределенная система управления версиями. GIT широко применяется для разработки как программного обеспечения (ПО) с открытым кодом, так и коммерческого ПО, предоставляя важные преимущества отдельным разработчикам, командам и компаниям.___

* GIT позволяет разработчикам просматривать всю временную шкалу изменений, решений и хода выполнения любого проекта в одном месте. С момента доступа к истории проекта разработчик получает всю необходимую информацию, чтобы разобраться в проекте и начать вносить свой вклад.

* Разработчики работают в разных часовых поясах. Благодаря распределенной системе управления версиями, такой как GIT, совместную работу можно вести в любое время, сохраняя целостность исходного кода. С помощью ветвей разработчики могут безопасно предлагать изменения для рабочего кода.

* Организации, использующие GIT, могут устранить коммуникационные барьеры между командами, чтобы те могли сосредоточиться на выполнении своих задач с максимальной эффективностью. Кроме того, GIT позволяет согласовать совместную работу экспертов над крупными проектами в масштабе всего предприятия.
___

## Комманды
   
**git init** — инициализирует новый репозиторий GIT и начинает отслеживание существующего каталога. В существующий каталог добавляется скрытая вложенная папка, в которой размещается внутренняя структура данных, необходимая для управления версиями.

  
**git clone** — создает локальную копию проекта, который уже существует удаленно. Клон включает в себя все файлы проекта, журнал и ветви.
   
**git add** — подготавливает изменение. GIT отслеживает изменения в базе кода разработчика, но для включения изменений в журнал проекта необходимо подготавливать их и создавать моментальные снимки. Эта команда выполняет первую часть этого двухэтапного процесса, то есть подготовку. Все подготовленные изменения станут частью следующего моментального снимка и журнала проекта. Раздельные подготовка и фиксация дают разработчикам полный контроль над историей проекта без необходимости изменять подход к написанию кода и работе в целом.

**git commit** — сохраняет моментальный снимок в журнале проекта и завершает процесс отслеживания изменений. Иначе говоря, фиксация похожа на создание фотографии. Все, что было подготовлено с помощью команды git add, станет частью моментального снимка при использовании git commit.

**git branch** — показывает ветви, с которыми ведется локальная работа.

**git pull** — применяет к локальной линии разработки обновления из удаленного аналога. Разработчики используют эту команду, если коллега выполнил фиксации в ветви удаленного репозитория и эти изменения нужно отразить в локальной среде.

**git merge** — выполняет слияние линий разработки. Эта команда обычно применяется для объединения изменений, внесенных в двух разных ветвях. Например, разработчик выполняет слияние, когда необходимо объединить изменения из ветви функции с главной ветвью для развертывания.

**git push** — обновляет удаленный репозиторий с учетом фиксаций, выполненных в ветви локально.

**git diff** — Команда git diff используется для вычисления разницы между любыми двумя Git деревьями. Это может быть разница между вашей рабочей директорией и индексом (собственно git diff), разница между индексом и последним коммитом (git diff --staged), или между любыми двумя коммитами (git diff master branchB).

**git reset** — Команда git reset, как можно догадаться из названия, используется в основном для отмены изменений. Она изменяет указатель HEAD и, опционально, состояние индекса. Также эта команда может изменить файлы в рабочей директории при использовании параметра --hard, что может привести к потере наработок при неправильном использовании, так что убедитесь в серьёзности своих намерений прежде чем использовать его.

**git checkout** — Команда git checkout используется для переключения веток и выгрузки их содержимого в рабочую директорию.

**git stash** — Команда git stash используется для временного сохранения всех незакоммиченных изменений для очистки рабочей директории без необходимости коммитить незавершённую работу в новую ветку.

**git log** — Команда git log используется для просмотра истории коммитов, начиная с самого свежего и уходя к истокам проекта. По умолчанию, она показывает лишь историю текущей ветки, но может быть настроена на вывод истории других, даже нескольких сразу, веток. Также её можно использовать для просмотра различий между ветками на уровне коммитов.

**git rm** — Команда git rm используется в Git для удаления файлов из индекса и рабочей директории. Она похожа на git add с тем лишь исключением, что она удаляет, а не добавляет файлы для следующего коммита.

**git fetch** — Команда git fetch связывается с удалённым репозиторием и забирает из него все изменения, которых у вас пока нет и сохраняет их локально.
