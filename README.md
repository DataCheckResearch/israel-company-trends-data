# מגמות רישום ופירוק חברות בישראל — נתוני 12 חודשים

מאגר קטן, שקוף וניתן לציטוט של נתוני מגמה חודשיים על רישום חברות ועל עדכוני סטטוס של מחיקה, פירוק או חיסול בישראל. הנתונים הם צילום מצב שנשלף מעמודי המחקר של DataCheck ב־25 באוגוסט 2026.

המטרה היא לאפשר לעיתונאים, חוקרים, אנליסטים ומפתחים להשתמש בנתונים מצרפיים בלי להעתיק גרפים ידנית, תוך שמירה על הקשר ומתודולוגיה ברורים.

> English: A citation-ready snapshot of monthly Israeli company registrations and dissolution-status updates. See the English summary below.

## קובצי הנתונים

| קובץ | מה הוא מכיל | מקור חי |
|---|---|---|
| [`company-registrations-monthly.csv`](data/company-registrations-monthly.csv) | מספר תאגידים שנרשמו בכל חודש | [חברות חדשות שנרשמו החודש](https://datacheck.co.il/trends/new-this-month) |
| [`company-dissolution-status-updates-monthly.csv`](data/company-dissolution-status-updates-monthly.csv) | מספר אירועי עדכון סטטוס למחיקה, פירוק או חיסול בכל חודש | [חברות שנמחקו ופורקו לאחרונה](https://datacheck.co.il/trends/dissolved) |

אוגוסט 2026 הוא חודש חלקי נכון למועד צילום הנתונים, ולכן אין להשוות אותו לחודש מלא בלי לציין זאת.

## שימוש מהיר

הקבצים הם CSV בקידוד UTF-8 וניתנים לפתיחה ב־Excel, ‏Google Sheets, ‏R או Python.

```python
import pandas as pd

registrations = pd.read_csv("data/company-registrations-monthly.csv")
dissolutions = pd.read_csv("data/company-dissolution-status-updates-monthly.csv")

print(registrations.tail())
print(dissolutions.tail())
```

## איך לצטט

נוסח מוצע:

> DataCheck Research, “מגמות רישום ופירוק חברות בישראל — נתוני 12 חודשים”, צילום נתונים מ־25.8.2026, על בסיס עמודי Trends של DataCheck.

יש לצרף קישור לעמוד המקור הרלוונטי ולציין את תאריך הגישה. קובץ [`CITATION.cff`](CITATION.cff) מאפשר גם יצירת ציטוט אוטומטי ב־GitHub ובכלים תומכים.

## מגבלות חשובות

- זהו צילום נתונים מצרפי, לא מאגר רשמי של רשות התאגידים.
- סדרת הפירוק מודדת אירועי עדכון סטטוס לפי חודש, ולא בהכרח מספר חברות ייחודיות או מועד מתן צו משפטי.
- מידע רישומי עשוי להתעדכן בדיעבד; לכן המספרים בעמודים החיים יכולים להשתנות לאחר צילום הקבצים.
- הנתונים אינם ציון סיכון ואינם תחליף לבדיקה של תאגיד מסוים.
- הקבצים אינם כוללים מידע אישי או רשומות ברמת חברה.

המתודולוגיה המלאה נמצאת ב־[`METHODOLOGY.md`](METHODOLOGY.md).

## רישיון וייחוס

הנתונים המצרפיים והמסמכים במאגר זמינים תחת [Creative Commons Attribution 4.0](LICENSE). שימוש חוזר מחייב ייחוס ל־DataCheck Research וקישור לעמוד המקור.

## תיקונים ועדכונים

מצאתם אי־התאמה בין הקובץ לעמוד המקור? פתחו Issue וציינו את שם הקובץ, החודש והערך החשוד. אין לפרסם ב־Issue מידע אישי או נתונים על אדם מסוים.

## English summary

This repository contains two monthly aggregate series for Israel:

1. new company and corporate registrations;
2. registry-status update events associated with deletion, liquidation or dissolution.

The files are a snapshot captured on 2026-08-25 from DataCheck Trends. August 2026 is incomplete. The dissolution series represents status-update events, not necessarily unique companies or court-order dates. Always cite the relevant source page and access date.

## מקור ופרטי קשר

- אתר: [DataCheck](https://datacheck.co.il/)
- מרכז מחקר: [DataCheck Trends](https://datacheck.co.il/trends)
- שאלות ותיקונים: [Help Desk](https://datacheck.co.il/contact.py)
