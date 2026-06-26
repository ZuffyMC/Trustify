# Configuration

Trustify is designed to be simple by default while still allowing deep customization.

## Runtime Folder

```text
plugins/Trustify/
├── config.yml
├── layout.yml
├── status.yml
├── rewards.yml
├── permissions.yml
├── integrations.yml
├── data/
├── messages/
└── modules/
```

## Important Notes

- Database files are stored inside `data/`
- Message files are stored inside `messages/`
- Advanced module settings are stored inside `modules/`
- GUI layout is controlled by `layout.yml`
- Rewards are controlled by `rewards.yml`
- Trust status ranges are controlled by `status.yml`

## Language

```yaml
settings:
  language: "english"
```

Available values:

```text
english
indonesia
```

## Storage

```yaml
storage:
  type: "SQLITE"

  sqlite:
    file: "data/database.db"

  mysql:
    host: "localhost"
    port: 3306
    database: "trustify"
    username: "root"
    password: "password"
    use-ssl: false
```
