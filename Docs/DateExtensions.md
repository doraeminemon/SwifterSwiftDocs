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


