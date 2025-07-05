### Установка  
Для установки необходимых зависимостей выполните команду:  

```bash
pip install -r requirements.txt  
```  

### Основные возможности  
- **Парсинг логов** (файл `access.log` в папке `logs`):  
  ```bash
  python cli.py parse  
  ```  

- **Просмотр логов** (по умолчанию выводится 100 строк):  
  ```bash
  python cli.py show  
  ```  

- **Фильтрация записей**:  
  - По IP-адресу:  
    ```bash
    python cli.py show --ip 192.168.1.1  
    ```  
  - По ключевому слову в URL:  
    ```bash
    python cli.py show --keyword admin  
    ```  
  - За определённый период:  
    ```bash
    python cli.py show --date-from 2023-01-01 --date-to 2023-12-31  
    ```  
  - С ограничением количества записей:  
    ```bash
    python cli.py show --limit 50  
    ```  

### Расположение файлов  
- Логи: `./logs/access.log`  
- База данных: `./logs.db`  
- Конфигурация: `./config.ini`
