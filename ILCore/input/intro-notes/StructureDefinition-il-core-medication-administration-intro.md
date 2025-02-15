<div dir="rtl" markdown="1">

### כללי
משאב הבסיס MedicationAdministration נועד לתעד ביצוע של מתן תרופה למטופל, או צריכת התרופה על ידו. משאב זה משמש את כלל מסגרות הטיפול השונות (בית חולים, קופת חולים וכו') בהם יש לתעד את ביצוע מתן התרופה, כולל מתן עצמי של תרופות דרך הפה, זריקות, טיפול תוך ורידי, וכו'. ניתן להשתמש בו גם במרפאות חוץ כדי לתעד זריקות נגד אלרגיה ומתן תרופה אחרת שאינה חיסון. במקרים מסוימים, ניתן להשתמש במשאב זה גם לדיווח על מתן תרופה בתוך מסגרת ביתית, כגון מתן אינסולין בניהול עצמי או במכשיר. המשאב מאפשר לתעד קישור למשאבים הקשורים לאירוע זה כגון שורת המרשם בה נרשמה התרופה (MedicationRequest), או לביקור (Encounter) שבו בוצע המתן.

### גבולות וקשר לפרופילים אחרים 

MedicationAdministration מיועד למעקב אחר מתן תרופות שאינן חיסונים. לכן, מערכות המתייחסות לחיסונים כמתן תרופה רגילה צריכות להשתמש במשאב Immunization כדי לייצג אותם. במידה ומערכות אלו חייבות להשתמש במשאב MedicationAdministration כדי לתעד חיסון בגלל אופן העבודה המקומי, או מכל סיבה אחרת, יש עדיין ליצור בנוסף גם מופע של משאב Immunization לחיסון.

### הרחבות שנוספו בפרופיל 
בדומה לפרופיל MedicationRequest, הוחלט להוסיף הרחבות (extensions) ע"מ לתמוך בתרחישי שימוש שונים שעלו במהלך ההסדרה של פרופיל זה עם ארגוני הבריאות השונים. להלן ההרחבות שנוספו לפרופיל (כולן אופציונאליות):
-	narcotic – אינדיקציה ("דגל") האם התרופה היא תרופה נרקוטית. נדרש ע"מ לתמוך ברגולציה הקיימת להוראות לתרופות נרקוטיות. תרופות נרקוטיות יסומנו כ- true, ואלה שאינן נרקוטיות יסומנו כ- false
-	recorded – הזמן שבו תועד מתן התרופה במערכת

### שדות חובה 
בכל משאב התואם לפרופיל ILCoreMedicationAdministration חייבים להיות האלמנטים הבאים:
-	status – סטטוס הבקשה/הוראה
-	Medication – קוד התרופה
-	Subject – המידע על המטופל 
-	Effective – זמן המתן 


### Must Support

בנוסף לאלמנטים שהוגדרו כחובה, הכיתוב MS (Must Support) ליד כל אלמנט מציין שכל מערכת חייבת לתמוך גם באלמנט זה במידה והוא קיים במופע ה-MedicationAdministration שהתקבל. להלן האלמנטים שהוגדר להם MS:
-	dosage.text – זמן מתן הבקשה
-	dosage.dose – הוראות מינון 



</div>