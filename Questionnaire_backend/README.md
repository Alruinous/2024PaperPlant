# Questionnaire_backend
## 安装包和依赖项
(The following commands should be executed under the root directory)
```
pip install -r requirements.txt
```
## 数据库迁移
修改`models.py`后，在`backend`下执行：
```
python manage.py makemigrations user
python manage.py migrate user
```

## 关闭占用当前端口的进程
找到端口`8000`对应的进程号(PID):
```
sudo lsof -i :8000
```
kill进程：
```
kill [PID]
```