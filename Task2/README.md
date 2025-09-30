# Запуск

Используется менеджер пакетов `uv`

Установка зависимостей

```bash
uv sync
```

Применение манифестов

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl apply -f hpa.yaml
```

Проброс портов

```bash
kubectl port-forward svc/scaletestapp-service 8080:8080
kubectl proxy
```

Запуск locust

```bash
uv run locust
```
