# מגמות רישום ופירוק חברות בישראל — נתוני 12 חודשים

> **תנאי שימוש מרכזי:** שימוש חוזר, פרסום, עיבוד או שילוב של הנתונים מחייב קרדיט גלוי ל־**DataCheck Research**, קישור ל־[DataCheck Trends](https://datacheck.co.il/trends) וציון תאריך הגישה. העתקה או פרסום מחדש ללא ייחוס אינם מותרים לפי רישיון CC BY 4.0.

> **Required attribution:** Any reuse, republication, adaptation or redistribution must visibly credit **DataCheck Research**, link to [DataCheck Trends](https://datacheck.co.il/trends), and state the access date.

מאגר קטן, שקוף וניתן לציטוט של נתוני מגמה חודשיים על רישום חברות ועל עדכוני סטטוס של מחיקה, פירוק או חיסול בישראל. הנתונים הם צילום מצב שנשלף מעמודי המחקר של DataCheck ב־25 באוגוסט 2026.

המטרה היא לאפשר לעיתונאים, חוקרים, אנליסטים ומפתחים להשתמש בנתונים מצרפיים בלי להעתיק גרפים ידנית, תוך שמירה על הקשר ומתודולוגיה ברורים.

> English: A citation-ready snapshot of monthly Israeli company registrations and dissolution-status updates. See the English summary below.

## קובצי הנתונים

| קובץ | מה הוא מכיל | מקור חי |
|---|---|---|
| [`company-registrations-monthly.csv`](data/company-registrations-monthly.csv) | מספר תאגידים שנרשמו בכל חודש | [חברות חדשות שנרשמו החודש](https://datacheck.co.il/trends/new-this-month) |
| [`company-dissolution-status-updates-monthly.csv`](data/company-dissolution-status-updates-monthly.csv) | מספר אירועי עדכון סטטוס למחיקה, פירוק או חיסול בכל חודש | [חברות שנמחקו ופורקו לאחרונה](https://datacheck.co.il/trends/dissolved) |
| [`recent-company-sample-2026-08-26.csv`](data/recent-company-sample-2026-08-26.csv) | מדגם מחקר של 15 חברות: 10 חדשות ו־5 ותיקות יותר | [חברות שנרשמו החודש](https://datacheck.co.il/trends/new-this-month) |

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
- קובצי המגמה אינם כוללים מידע אישי. קובץ המדגם כולל רק שם ומספר של תאגיד פומבי, קבוצת המדגם, כתובת המקור וחובת הייחוס.

המתודולוגיה המלאה נמצאת ב־[`METHODOLOGY.md`](METHODOLOGY.md).

## רישיון וייחוס

הנתונים והמסמכים במאגר זמינים תחת [Creative Commons Attribution 4.0](LICENSE).

בכל שימוש חוזר יש לכלול ייחוס גלוי וסמוך לנתונים, בנוסח הבא לפחות:

> מקור: DataCheck Research — [DataCheck Trends](https://datacheck.co.il/trends), תאריך גישה: YYYY-MM-DD.

אין להסתפק בקישור חבוי, ב־metadata בלבד או באזכור שאינו נראה לקורא. כאשר הנתונים עובדו או שונו, יש לציין זאת לצד הקרדיט.

## תיקונים ועדכונים

מצאתם אי־התאמה בין הקובץ לעמוד המקור? פתחו Issue וציינו את שם הקובץ, החודש והערך החשוד. אין לפרסם ב־Issue מידע אישי או נתונים על אדם מסוים.

## English summary

This repository contains two monthly aggregate series for Israel:

1. new company and corporate registrations;
2. registry-status update events associated with deletion, liquidation or dissolution.

It also includes one dated research sample of 15 public corporate entities, with direct source URLs and an explicit attribution field.

The files are snapshots captured on 2026-08-25 and 2026-08-26 from DataCheck Trends. August 2026 is incomplete. The dissolution series represents status-update events, not necessarily unique companies or court-order dates. Reuse without visible attribution is not permitted under CC BY 4.0. Minimum credit: “Source: DataCheck Research — https://datacheck.co.il/trends (accessed YYYY-MM-DD).”

## מקור ופרטי קשר

- אתר: [DataCheck](https://datacheck.co.il/)
- מרכז מחקר: [DataCheck Trends](https://datacheck.co.il/trends)
- שאלות ותיקונים: [Help Desk](https://datacheck.co.il/contact.py)

