![Prototypes](../../images/3-3.3-prototypes.png)

```
@startuml
!define RECTANGLE_ICON_COLOR #ADD8E6
skinparam rectangle {
    BackgroundColor RECTANGLE_ICON_COLOR
    BorderColor black
    FontSize 12
    FontColor black
}
title Горизонтальний прототип системи безпеки на будівельному майданчику

rectangle "<b>Головна панель</b>" {
    rectangle "<b>Сповіщення</b>\nПерегляд та налаштування сповіщень" as Notifications
    rectangle "<b>Звіти</b>\nФормування та перегляд щотижневих звітів" as Reports
    rectangle "<b>Моніторинг</b>\nПоточний статус зон ризику" as Monitoring
    rectangle "<b>Керування користувачами</b>\nРолі та права доступу" as UserManagement
}

rectangle "<b>Сповіщення</b>" {
    rectangle "<b>Налаштування сповіщень</b>\nРозподіл сповіщень за ролями" as NotificationSettings
    rectangle "<b>Перегляд сповіщень</b>\nОстанні сповіщення та історія" as ViewNotifications
}

rectangle "<b>Звіти</b>" {
    rectangle "<b>Формування звітів</b>\nЩотижневі, критичні інциденти" as ReportGeneration
    rectangle "<b>Історія звітів</b>\nПерегляд збережених звітів" as ReportHistory
}

rectangle "<b>Моніторинг</b>" {
    rectangle "<b>Візуалізація майданчика</b>\nЗони ризику в реальному часі" as SiteView
    rectangle "<b>Карта ризиків</b>\nІнтерактивна карта зон" as RiskMap
}

rectangle "<b>Керування користувачами</b>" {
    rectangle "<b>Додавання/видалення користувачів</b>\nРеєстрація працівників та керівників" as AddUsers
    rectangle "<b>Розподіл ролей</b>\nРолі: працівник, оператор, керівник" as RoleAssignment
}

Notifications -[hidden]-> Reports
Reports -[hidden]-> Monitoring
Monitoring -[hidden]-> UserManagement

Notifications --> NotificationSettings
Notifications --> ViewNotifications
Reports --> ReportGeneration
Reports --> ReportHistory
Monitoring --> SiteView
Monitoring --> RiskMap
UserManagement --> AddUsers
UserManagement --> RoleAssignment
@enduml
```