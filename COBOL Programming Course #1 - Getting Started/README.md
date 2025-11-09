# קורס תכנות COBOL #1 - תחילת עבודה

פרויקט זה הוא סט של חומרי הדרכה ומעבדות לקורס ברמת "תחילת עבודה" על COBOL. נעשה שימוש בכלי צד-לקוח חינמיים וזמינים לציבור כדי לתקשר עם סביבת המיינפריים, מה שמאפשר למשתתפים למנף בקלות טכנולוגיות אלו לאחר הקורס.

## איך להתחיל

כדי להתחיל, בחרו [גרסה](https://github.com/openmainframeproject/cobol-programming-course/releases) עדכנית של הקורס. תחת גרסה נתונה, אתם אמורים לראות שני נכסים.

- הנכס PDF של קורס תכנות COBOL #1 - תחילת עבודה מכיל את הוראות הקורס.
- נכס קוד המקור מכיל את כל מה שהיה בפרויקט בעת פרסום הגרסה.

להשלמת הקורס, תצטרכו גם לבצע אחת מהפעולות הבאות:
- בחרו [ספק](#ספקים) למטה ועקבו אחר תהליך ההרשמה שלהם. לאחר ההשלמה, אתם אמורים לקבל פרטי מערכת לשימוש בקורס.
- העלו את קוד המקור של הקורס (הנמצא בתיקיית המעבדות) לסביבת המיינפריים שלכם.

## ספקים

חומרים אלה משמשים ארגונים אחרים כדי לספק הדרכת COBOL לקהילה. פרויקט זה וגם פרויקט Open Mainframe אינם בודקים, מתחזקים או תומכים באף אחד מהספקים המסוימים הללו. אם אתם משתמשים בחומרים אלה בחומרי ההדרכה שלכם, אתם מוזמנים [לערוך ולהגיש בקשת משיכה](https://github.com/openmainframeproject/cobol-programming-course/edit/governance-docs/README.md) כדי לכלול אותה.

- IBM סיפקה [סביבה חינמית להשלמת מעבדה זו](https://ibm.biz/cobollabs).

## בנייה

ה-PDF נבנה באמצעות הפקודה הבאה של [pandoc](https://pandoc.org/). שימו לב: נדרש pdflatex. ניתן להתקין את [MiKTeX](https://miktex.org/) כדי להתאים זאת.

```
pandoc "COBOL Programming Course #1 - Getting Started.md" -o "COBOL Programming Course #1 - Getting Started.pdf" --number-sections --toc -B Front_Matter.tex --listings
```

`Front_Matter.tex` מכיל את התוכן שלפני תוכן העניינים. `COBOL Programming Course #1 - Getting Started.md` מכיל את הגוף. הפקודה משלבת את השניים, יוצרת את מספרי הסעיפים ותוכן העניינים עבור הגוף, ומוציאה את `COBOL Programming Course #1 - Getting Started.pdf`
