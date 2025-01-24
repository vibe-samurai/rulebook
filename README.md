# Convention

*Конвенция по ведению проекта, основные правила и требования к написанию кода*

---
**Архитектура**

В проекте используется архитектурная методология: [FSD (docs)](https://feature-sliced.design/docs/get-started/overview)

---
**Командная разработка (Git)**

Правила работы с Git:

Правила работы с ветками:
 1. В проекте существует две постоянные ветки **main** и **dev**
 2. Для работы над текущими задачами следует создавать *свою рабочую ветку* от ветки **dev**
 3. Название рабочей ветки должно содержать номер задачи взятой в работу, а также тип (**feat**, **fix**, **hotfix**, **tech**)
 *Пример:* **feat/IT-54, fix/TECH-244, hotfix/VIBE-999**
 4. Вливание изменений в **dev** проводится с помощью **Pull Request**, после ревью кода со стороны других членов команды. 
 5. Исключительным правом вливания изменений в **dev** и **main** ветки, обладает член команды на позиции **Front-End (main)**

Правила работы с коммитами:

 Коммиты именуются согласно спецификации [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)

Согласно схеме:
```
<type>[optional scope]: <TASK ID> <description>
```
**type**  (согласно [Angular convention](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines)):
-   **build**: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
-   **ci**: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)
-   **docs**: Documentation only changes
-   **feat**: A new feature
-   **fix**: A bug fix
-   **perf**: A code change that improves performance
-   **refactor**: A code change that neither fixes a bug nor adds a feature
-   **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
-   **test**: Adding missing tests or correcting existing tests

**scope** - обозначение части приложение над которым велась работа:
-   **animations**
-   **common**
-   **compiler**
-   **compiler-cli**
-   **core**
-   **elements**
-   **forms**
-   **router**
- является опциональным, может быть указан как "*" (звездочка)
	
**TASK ID** - номер задачи из таск-трекера проекта

**description** - краткое описание проделанной работы

Пример названия коммита:
```
feat(auth): VIBE-999 add password recover option
```

---

**Codestyle**

При работе над проектом придерживаться [React styleguide](https://react-style-guide.staging.it-incubator.ru/) от it-incubator

---
