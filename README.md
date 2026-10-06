# ЭСТЕТ media

render.svg → PNG 1080×1350. Каждый результат сохраняется как
posts/<source-commit>-render.png плюс manifest с image_sha256.
Legacy render.png сохраняется для действующего автопостинга.
Workflow summary содержит raw URL итогового media commit SHA: передавайте именно
его в публикацию. Завершения рендера следует дождаться до подготовки поста.

PR рендерит preview artifact без коммита. Изменение render.svg на main создаёт
версионные файлы; повторная попытка сверяет существующий PNG и не перезаписывает его.
Push конфликт повторяется с актуальной main без force-push.
