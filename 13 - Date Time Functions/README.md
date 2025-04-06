# 1 - DateTime

DateTime class: The DateTime class is the core class for working with dates and times in Dart. You can use it to represent a specific point in time.

Creating a DateTime instance:

```
// Current date and time
DateTime now = DateTime.now(); 

// Specific date (year, month, day)
DateTime specificDate = DateTime(2023, 7, 5);

// Specific date and time (year, month, day, hour, minute, second)
DateTime specificDateTime = DateTime(2023, 7, 5, 12, 30, 45);
```

# 2 - Formatting dates

Formatting dates: You can format DateTime objects into strings using the `intl` package or built-in methods.

Using the built-in methods:

```
DateTime now = DateTime.now();

String formattedDate = "${now.year}-${now.month}-${now.day}"; // Custom format

String formattedTime = "${now.hour}:${now.minute}:${now.second}"; // Custom format
```

Using the `intl` package:

```
import 'package:intl/intl.dart';

DateTime now = DateTime.now();

String formattedDate = DateFormat('yyyy-MM-dd').format(now);

String formattedTime = DateFormat('HH:mm:ss').format(now);
```

# 3 - Adding and Subtracting time

Adding/Subtracting time: You can perform operations to add or subtract time intervals from a DateTime object.

```
DateTime now = DateTime.now();

// Adding 7 days
DateTime nextWeek = now.add(Duration(days: 7));

// Subtracting 30 days
DateTime lastMonth = now.subtract(Duration(days: 30));
```

# 4 - Comparing dates

Comparing dates: You can compare two DateTime objects to check their relationship.

```
DateTime firstDate = DateTime(2023, 7, 5);
DateTime secondDate = DateTime(2023, 7, 10);

bool isBefore = firstDate.isBefore(secondDate); // true

bool isAfter = firstDate.isAfter(secondDate); // false

bool isSame = firstDate.isAtSameMomentAs(secondDate); // false
```

# 5 - Parsing dates

Parsing dates: You can parse date strings into DateTime objects.

```
String dateString = '2023-07-05';

DateTime parsedDate = DateTime.parse(dateString);
```

# 6 - Timezone support

Timezone support: Dart's DateTime class does not inherently support timezones, but you can use external libraries like timezone to work with timezones.

```
import 'package:timezone/timezone.dart' as tz;

// Get the current timezone
tz.Location timeZone = tz.getLocation('America/New_York');

// Convert a DateTime to a TZDateTime (timezone-aware DateTime)
DateTime now = DateTime.now();
tz.TZDateTime timeZoneDateTime = tz.TZDateTime.from(now, timeZone);

// Convert a TZDateTime to a specific timezone
tz.TZDateTime specificTimeZoneDateTime = timeZoneDateTime.toLocal();
```

# 7 - Date arithmetic

Date arithmetic: Dart's DateTime class allows you to perform various arithmetic operations on dates.

```
DateTime startDate = DateTime(2023, 7, 5);
DateTime endDate = DateTime(2023, 7, 15);

// Difference between two dates in days
int daysDifference = endDate.difference(startDate).inDays;

// Difference between two dates in hours
int hoursDifference = endDate.difference(startDate).inHours;

// Difference between two dates in minutes
int minutesDifference = endDate.difference(startDate).inMinutes;
```

# 8 - Date formatting using `intl` package

Date formatting using `intl` package: The intl package provides a powerful and flexible way to format dates and times.

```
import 'package:intl/intl.dart';

DateTime now = DateTime.now();

// Formatted date with full month name and weekday
String formattedFullDate = DateFormat('EEEE, MMMM d, y').format(now);

// Formatted time with AM/PM indicator
String formattedTimeWithAmPm = DateFormat('hh:mm a').format(now);
```

# 9 - Duration

Duration: Dart's Duration class represents a span of time, allowing you to work with time intervals.

```
// Create a duration
Duration duration = Duration(hours: 2, minutes: 30);

// Adding a duration to a DateTime
DateTime now = DateTime.now();
DateTime futureDateTime = now.add(duration);

// Subtracting a duration from a DateTime
DateTime pastDateTime = now.subtract(duration);

// Difference between two DateTimes as a Duration
Duration difference = futureDateTime.difference(now);
```

# 10 - Weekday and month enumeration

Weekday and month enumeration: Dart's DateTime class provides constants for weekdays and months.

```
DateTime date = DateTime(2023, 7, 5);

// Day of the month (1 to 31)
int day = date.day;

// Month (1 to 12)
int month = date.month;

// Year
int year = date.year;

// Weekday index (1 to 7, Monday to Sunday)
int weekDayIndex = date.weekday;

// Weekday name (e.g., Monday)
String weekDayName = DateFormat('EEEE').format(date);

// Full month name (e.g., July)
String monthName = DateFormat('MMMM').format(date);

// Abbreviated month name (e.g., Jul)
String abbreviatedMonthName = DateFormat('MMM').format(date);
```

# 11 - Date parsing using intl package

Date parsing using intl package: The intl package can also be used to parse date strings into DateTime objects.

```
import 'package:intl/intl.dart';

String dateString = '2023-07-05';
DateTime parsedDate = DateFormat('yyyy-MM-dd').parse(dateString);
```