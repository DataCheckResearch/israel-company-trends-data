---
license: cc-by-4.0
language:
  - he
  - en
pretty_name: Israeli Company Registration and Dissolution Trends
tags:
  - tabular
  - timeseries
  - israel
  - company-registry
  - business-intelligence
  - open-data
size_categories:
  - n<1K
---

# מגמות רישום ופירוק חברות בישראל

מערך נתונים מצרפי קטן ובעל מתודולוגיה מפורשת, המבוסס על עמודי המחקר של DataCheck. הוא כולל שתי סדרות חודשיות: רישומי תאגידים חדשים ועדכוני סטטוס הקשורים למחיקה, פירוק או חיסול.

## קבצים

- `data/company-registrations-monthly.csv`
- `data/company-dissolution-status-updates-monthly.csv`

## מקור

- https://datacheck.co.il/trends/new-this-month
- https://datacheck.co.il/trends/dissolved

הנתונים צולמו ב־25 באוגוסט 2026. אוגוסט 2026 הוא חודש חלקי.

## משמעות הנתונים

סדרת הפירוק מייצגת אירועי עדכון סטטוס לפי חודש. אין לפרש אותה כמספר חברות ייחודיות, כמספר צווי פירוק או כתאריך החלטה שיפוטית. הנתונים מצרפיים ואינם כוללים מידע אישי או רשומות ברמת חברה.

## שימוש מיועד

המערך מתאים לניתוח סדרות זמן, גרפים, עיתונות נתונים, מחקר והדגמות. הוא אינו ציון סיכון ואינו תחליף לבדיקה משפטית או עסקית של חברה מסוימת.

## רישיון וציטוט

CC BY 4.0. יש לייחס ל־DataCheck Research, לקשר לעמוד המקור הרלוונטי ולציין את תאריך הגישה. פרטי המתודולוגיה נמצאים ב־`METHODOLOGY.md` והציטוט המובנה ב־`CITATION.cff`.

## English summary

Two monthly aggregate time series derived from DataCheck Trends: Israeli corporate registrations and registry status-update events associated with deletion, liquidation or dissolution. August 2026 is incomplete. The dissolution series does not necessarily represent unique companies or court-order dates.
