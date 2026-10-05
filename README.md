# 设备校准停用传播所在业务服务

这是一个使用 Python、FastAPI 与 SQLite 实现的后端项目。代码包含领域模型、数据访问、接口路由和业务规则，可在单个 Linux 应用容器内完成测试与运行。

## 安装

```bash
python3 -m pip install -r requirements.txt -r requirements-dev.txt
```

## 测试

```bash
python3 -m pytest -q
```

## 编译检查

```bash
python3 -m compileall -q .
```

## 接口冒烟

```bash
python3 -c "from app.main import app; print(len(app.routes))"
```

## 启动

```bash
uvicorn app.main:app --host 0.0.0.0 --port 8000
```
