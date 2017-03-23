# Date Extensions


## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`DayNameStyle`**](#daynamestyle) | Enum | 8+ | 9+ | 3+ | 10.10+ |
| [**`MonthNameStyle`**](#monthnamestyle) | Enum | 8+ | 9+ | 3+ | 10.10+ |
| [**`calendar`**](#calendar) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`era`**](#era) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`year`**](#year) | Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`quarter`**](#quarter) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`month`**](#month) | Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`weekOfYear`**](#weekofyear) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`weekOfMonth`**](#weekofmonth) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`weekday`**](#weekday) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`day`**](#day) | Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`hour`**](#hour) | Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`minute`**](#minute) | Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`second`**](#second) | Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`nanosecond`**](#nanosecond) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isInFuture`**](#isinfuture) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isInPast`**](#isinpast) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isInToday`**](#isintoday) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isInYesterday`**](#isinyesterday) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isInTomorrow`**](#isintomorrow) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`iso8601String`**](#iso8601string) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`nearestFiveMinutes`**](#nearestfiveminutes) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`nearestTenMinutes`**](#nearesttenminutes) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`nearestQuarterHour`**](#nearestquarterhour) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`nearestHalfHour`**](#nearesthalfhour) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`nearestHour`**](#nearesthour) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`timeZone`**](#timezone) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`unixTimestamp`**](#unixtimestamp) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`adding(component: Calendar.Component, value: Int)`**](#adding_-component-calendarcomponent-value-int) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`add(component: Calendar.Component, value: Int)`**](#add_-component-calendarcomponent-value-int) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`changing(_ component: Calendar.Component, value: Int)`**](#changing_-component-calendarcomponent-value-int) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`beginning(of component: Calendar.Component)`**](#beginningof-component-calendarcomponent) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`end(of component: Calendar.Component)`**](#endof-component-calendarcomponent) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`dateString(ofStyle style: DateFormatter.Style)`**](#datestringofstyle-style-dateformatterstyle--medium) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`dateTimeString(ofStyle style: DateFormatter.Style)`**](#datetimestringofstyle-style-dateformatterstyle--medium) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`isInCurrent(_ component: Calendar.Component)`**](#isincurrent_-component-calendarcomponent) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`timeString(ofStyle style: DateFormatter.Style)`**](#timestringofstyle-style-dateformatterstyle--medium) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`dayName(ofStyle style: DayNameStyle)`**](#daynameofstyle-style-daynamestyle--full) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`monthName(ofStyle style: MonthNameStyle)`**](#monthnameofstyle-style-monthnamestyle--full) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`init?(calendar: Calendar?, timeZone: TimeZone?, era: Int?, year: Int?, month: Int?, day: Int?, hour: Int?, minute: Int?, second: Int?, nanosecond: Int?)`**](#initcalendar-calendar--calendarcurrent-timezone-timezone--timezonecurrent-era-int--dateera-year-int--dateyear-month-int--datemonth-day-int--dateday-hour-int--datehour-minute-int--dateminute-second-int--datesecond-nanosecond-int--datenanosecond) | Optional Initializer  | 8+ | 9+ | 3+ | 10.10+ |
| [**`init?(iso8601String: String)`**](#initiso8601string-string) | Optional Initializer  | 8+ | 9+ | 3+ | 10.10+ |
| [**`init(unixTimestamp: Double)`**](#initunixtimestamp-double) | Initializer  | 8+ | 9+ | 3+ | 10.10+ |

--


## `DayNameStyle `
Day name format.

 - **type**: Enum.
 - **cases**:
 	- **threeLetters**: 3 letter day abbreviation of day name.
 	- **oneLetter**: 1 letter day abbreviation of day name.
 	- **full**: Full day name.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


--


## `MonthNameStyle `
Day name format.

 - **type**: Enum.
 - **cases**:
 	- **threeLetters**: 3 letter month abbreviation of month name.
 	- **oneLetter**: 1 letter month abbreviation of month name.
 	- **full**: Full day name.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


--


## `calendar`
User’s current calendar.

 - **type**: Read-Only Property.
 - **return type**: Calendar
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


--


## `era`
Era.

 - **type**: Read-Only Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().era -> 1
```


--


## `year`
Year.

 - **type**: Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().year -> 2017

var someDate = Date()
someDate.year = 2000 // sets someDate's year to 2000

```


--


## `quarter`
Quarter.

 - **type**: Read-Only Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


--


## `month`
Month.

 - **type**: Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().month -> 1

var someDate = Date()
someDate.year = 10 // sets someDate's month to 10.

```


--


## `weekOfYear`
Week of year.

 - **type**: Read-Only Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().weekOfYear -> 2 // second week in the current year.
```


--


## `weekOfMonth`
Week of month.

 - **type**: Read-Only Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().weekOfMonth -> 2 // second week in the current month.
```


--


## `weekday`
Weekday.

 - **type**: Read-Only Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().weekOfMonth -> 5 // fifth day in the current week.
```


--


## `day`
Day.

 - **type**: Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().day -> 12

var someDate = Date()
someDate.day = 1 // sets someDate's day of month to 1.

```


--


## `hour`
Hour.

 - **type**: Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().hour -> 17 // 5 pm

var someDate = Date()
someDate.day = 13 // sets someDate's hour to 1 pm.

```


--


## `minute`
Minutes.

 - **type**: Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().minute -> 39

var someDate = Date()
someDate.minute = 10 // sets someDate's minutes to 10.

```


--


## `second`
Seconds.

 - **type**: Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().second -> 55

var someDate = Date()
someDate. second = 15 // sets someDate's seconds to 15.

```


--


## `nanosecond`
Nanoseconds.

 - **type**: Read-Only Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().nanosecond -> 981379985
```


--


## `isInFuture`
Check if date is in future.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date(timeInterval: 100, since: Date()).isInFuture -> true
```


--


## `isInPast`
Check if date is in past.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date(timeInterval: -100, since: Date()).isInPast -> true
```


--


## `isInToday`
Check if date is in today.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().isInToday -> true
```


--


## `isInYesterday`
Check if date is in yesterday.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().isInYesterday -> false
```


--


## `isInTomorrow`
Check if date is in tomorrow.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().isInTomorrow -> false
```


--


## `iso8601String`
ISO8601 string of format (yyyy-MM-dd'T'HH:mm:ss.SSS) from date.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().iso8601String -> "2017-01-12T14:51:29.574Z"
```


--


## `nearestFiveMinutes`
Nearest five minutes to date.

 - **type**: Read-Only Property.
 - **return type**: Date
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
var date = Date() // "5:54 PM"
date.minute = 32 // "5:32 PM"
date.nearestFiveMinutes // "5:30 PM"

date.minute = 44 // "5:44 PM"
date.nearestFiveMinutes // "5:45 PM"
```


--


## `nearestTenMinutes`
Nearest ten minutes to date.

 - **type**: Read-Only Property.
 - **return type**: Date
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
var date = Date() // "5:57 PM"
date.minute = 34 // "5:34 PM"
date.nearestTenMinutes // "5:30 PM"

date.minute = 48 // "5:48 PM"
date.nearestTenMinutes // "5:50 PM"
```


--


## `nearestQuarterHour`
Nearest quarter hour to date.

 - **type**: Read-Only Property.
 - **return type**: Date
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
var date = Date() // "5:57 PM"
date.minute = 34 // "5:34 PM"
date.nearestQuarterHour // "5:30 PM"

date.minute = 40 // "5:40 PM"
date.nearestQuarterHour // "5:45 PM"
```


--


## `nearestHalfHour`
Nearest half hour to date.

 - **type**: Read-Only Property.
 - **return type**: Date
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
var date = Date() // "6:07 PM"
date.minute = 41 // "6:41 PM"
date.nearestHalfHour // "6:30 PM"

date.minute = 51 // "6:51 PM"
date.nearestHalfHour // "7:00 PM"
```


--


## `nearestHour`
Nearest hour to date.

 - **type**: Read-Only Property.
 - **return type**: Date
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
var date = Date() // "6:17 PM"
date.nearestHour // "6:00 PM"

date.minute = 36 // "6:36 PM"
date.nearestHour // "7:00 PM"
```


--


## `timeZone`
Time zone used by system.

 - **type**: Read-Only Property.
 - **return type**: TimeZone
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().timeZone -> Europe/Istanbul (current)
```


--


## `unixTimestamp`
UNIX timestamp from date.

 - **type**: Read-Only Property.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


Example

```swift
Date().unixTimestamp -> 1484233862.826291
```


--


## `adding(_ component: Calendar.Component, value: Int)`
Date by adding multiples of calendar component.

 - **type**: Method.
 - **return type**: Date
 - **parameters**:
   - **component**: component type.
   - **value**: multiples of components to add.
 - **returns**: original date + multiples of component added.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let date = Date() // "Jan 12, 2017, 7:07 PM"
let date2 = date.adding(.minute, value: -10) // "Jan 12, 2017, 6:57 PM"
let date3 = date.adding(.day, value: 4) // "Jan 16, 2017, 7:07 PM"
let date4 = date.adding(.month, value: 2) // "Mar 12, 2017, 7:07 PM"
let date5 = date.adding(.year, value: 13) // "Jan 12, 2030, 7:07 PM"
```


--


## `add(_ component: Calendar.Component, value: Int)`
Add calendar component to date.

 - **type**: Mutating Method.
 - **return type**: Date
 - **parameters**:
   - **component**: component type.
   - **value**: multiples of components to add.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
var date = Date() // "Jan 12, 2017, 7:07 PM"
date.add(.minute, value: -10) // "Jan 12, 2017, 6:57 PM"
date.add(.day, value: 4) // "Jan 16, 2017, 7:07 PM"
date.add(.month, value: 2) // "Mar 12, 2017, 7:07 PM"
date.add(.year, value: 13) // "Jan 12, 2030, 7:07 PM"
```


--


## `changing(_ component: Calendar.Component, value: Int)`
Date by changing value of calendar component.

 - **type**: Method.
 - **return type**: Date
 - **parameters**:
   - **component**: component type.
   - **value**: multiples of components to add.
 - **returns**: original date after changing given component to given value.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let date = Date() // "Jan 12, 2017, 7:07 PM"
let date2 = date.changing(.minute, value: 10) // "Jan 12, 2017, 6:10 PM"
let date3 = date.changing(.day, value: 4) // "Jan 4, 2017, 7:07 PM"
let date4 = date.changing(.month, value: 2) // "Feb 12, 2017, 7:07 PM"
let date5 = date.changing(.year, value: 2000) // "Jan 12, 2000, 7:07 PM"
```


--


## `beginning(of component: Calendar.Component)`
Data at the beginning of calendar component.

 - **type**: Method.
 - **return type**: Date?
 - **parameters**:
   - **component**: calendar component to get date at the beginning of.
 - **returns**: date at the beginning of calendar component (if applicable).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let date = Date() // "Jan 12, 2017, 7:14 PM"
let date2 = date.beginning(of: .hour) // "Jan 12, 2017, 7:00 PM"
let date3 = date.beginning(of: .month) // "Jan 1, 2017, 12:00 AM"
let date4 = date.beginning(of: .year) // "Jan 1, 2017, 12:00 AM"
```


--


## `end(of component: Calendar.Component)`
Date at the end of calendar component.

 - **type**: Method.
 - **return type**: Date?
 - **parameters**:
   - **component**: calendar component to get date at the end of.
 - **returns**: date at the end of calendar component (if applicable).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let date = Date() // "Jan 12, 2017, 7:27 PM"
let date2 = date.end(of: .day) // "Jan 12, 2017, 11:59 PM"
let date3 = date.end(of: .month) // "Jan 31, 2017, 11:59 PM"
let date4 = date.end(of: .year) // "Dec 31, 2017, 11:59 PM"
```


--


## `dateString(ofStyle style: DateFormatter.Style = .medium)`
Date string from date.

 - **type**: Method.
 - **return type**: String
 - **parameters**:
   - **style**: DateFormatter style (default is .medium).
 - **returns**: date string.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Date().dateString(ofStyle: .short) -> "1/12/17"
Date().dateString(ofStyle: .medium) -> "Jan 12, 2017"
Date().dateString(ofStyle: .long) -> "January 12, 2017"
Date().dateString(ofStyle: .full) -> "Thursday, January 12, 2017"
```


--


## `dateTimeString(ofStyle style: DateFormatter.Style = .medium)`
Date and time string from date.

 - **type**: Method.
 - **return type**: String
 - **parameters**:
   - **style**: DateFormatter style (default is .medium).
 - **returns**: date and time string.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Date().dateTimeString(ofStyle: .short) -> "1/12/17, 7:32 PM"
Date().dateTimeString(ofStyle: .medium) -> "Jan 12, 2017, 7:32:00 PM"
Date().dateTimeString(ofStyle: .long) -> "January 12, 2017 at 7:32:00 PM GMT+3"
Date().dateTimeString(ofStyle: .full) -> "Thursday, January 12, 2017 at 7:32:00 PM GMT+03:00"
```


--


## `isInCurrent(_ component: Calendar.Component)`
Check if date is in current given calendar component.

 - **type**: Method.
 - **return type**: Bool
 - **parameters**:
   - **component**: calendar component to check.
 - **returns**: true if date is in current given calendar component.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Date().isInCurrent(.day) -> true
Date().isInCurrent(.year) -> true
```


--


## `timeString(ofStyle style: DateFormatter.Style = .medium)`
Time string from date.

 - **type**: Method.
 - **return type**: String
 - **parameters**:
   - **style**: DateFormatter style (default is .medium).
 - **returns**: time string.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Date().timeString(ofStyle: .short) -> "7:37 PM"
Date().timeString(ofStyle: .medium) -> "7:37:02 PM"
Date().timeString(ofStyle: .long) -> "7:37:02 PM GMT+3"
Date().timeString(ofStyle: .full) -> "7:37:02 PM GMT+03:00"
```


--


## `dayName(ofStyle style: DayNameStyle = .full)`
Day name from date.

 - **type**: Method.
 - **return type**: String
 - **parameters**:
   - **style**: style of day name (default is DayNameStyle.full).
 - **returns**: day name string (example: W, Wed, Wednesday).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Date().dayName(ofStyle: .oneLetter) -> "T"
Date().dayName(ofStyle: .threeLetters) -> "Thu"
Date().dayName(ofStyle: .full) -> "Thursday"
```


--


## `monthName(ofStyle style: MonthNameStyle = .full)`
Month name from date.

 - **type**: Method.
 - **return type**: String
 - **parameters**:
   - **style**: style of month name (default is MonthNameStyle.full).
 - **returns**: month name string (example: D, Dec, December).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Date().monthName(ofStyle: .oneLetter) -> "J"
Date().monthName(ofStyle: .threeLetters) -> "Jan"
Date().monthName(ofStyle: .full) -> "January"
```


--


## `init?(calendar: Calendar? = Calendar.current, timeZone: TimeZone? = TimeZone.current, era: Int? = Date().era, year: Int? = Date().year, month: Int? = Date().month, day: Int? = Date().day, hour: Int? = Date().hour, minute: Int? = Date().minute, second: Int? = Date().second, nanosecond: Int? = Date().nanosecond)`
Create a new date form calendar components.

 - **type**: Optional Initializer.
 - **return type**: Date?
 - **parameters**:
   - **calendar**: Calendar (default is current).
   - **timeZone**: TimeZone (default is current).
   - **era**: Era (default is current era).
   - **year**: Year (default is current year).
   - **month**: Month (default is current month).
   - **day**: Day (default is today).
   - **hour**: Hour (default is current hour).
   - **minute**: Minute (default is current minute).
   - **second**: Second (default is current second).
   - **nanosecond**: Nanosecond (default is current nanosecond).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let date = Date(year: 2010, month: 1, day: 12) // "Jan 12, 2010, 7:45 PM"
```


--


## `init?(iso8601String: String)`
Create date object from ISO8601 string.

 - **type**: Optional Initializer.
 - **return type**: Date?
 - **parameters**:
   - **iso8601String**: iso8601String: ISO8601 string of format (yyyy-MM-dd'T'HH:mm:ss.SSSZ).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let date = Date(iso8601String: "2017-01-12T16:48:00.959Z") // "Jan 12, 2017, 7:48 PM"
```


--


## `init(unixTimestamp: Double)`
Create new date object from UNIX timestamp.

 - **type**: Initializer.
 - **return type**: Date
 - **parameters**:
   - **unixTimestamp**: UNIX timestamp.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let date = Date(unixTimestamp: 1484239783.922743) // "Jan 12, 2017, 7:49 PM"
```


--
