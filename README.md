## Порядок

1. Откройте `index.html` в VS Code и запустите через Live Server.
2. В Figma изучите карточку авторизации, поля и кнопку.
3. Удалите секцию `auth__placeholder`. Вместо неё создайте `section.auth-card` с `form#login-form`.
4. Создайте `label` и `input` для email и пароля, кнопку отправки, два `p` для ошибок и один `p` для результата.
5. Используйте **обязательные id**: `login-form`, `email`, `password`, `email-error`, `password-error`, `form-status`.
6. Введите `type="email" required` и `type="password" minlength="8" required`; для формы поставьте `novalidate`.
7. Допишите TODO 1–4 в `scripts/app.js`.
8. Проверьте сценарии из `CHECKLIST.md` и сделайте два скриншота.

## Пример структуры одной группы

```html
<div class="field">
  <label class="field__label" for="email">Электронная почта</label>
  <input
    class="field__input"
    id="email"
    name="email"
    type="email"
    required
    aria-describedby="email-error"
    aria-invalid="false"
  />
  <p class="field__error" id="email-error"></p>
</div>
```
