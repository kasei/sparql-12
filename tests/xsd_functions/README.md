# SPARQL 1.2: Possible XSD Functions and Operators

This is a list of XSD functions and operators that might be included in SPARQL 1.2.
Checkboxes indicate whether there is (at least minimal) test coverage in the included
[tests](../) directory.

## [8 Functions and operators on durations](https://www.w3.org/TR/xpath-functions/#durations)

### [8.2 Comparison operators on durations](https://www.w3.org/TR/xpath-functions/#comp.duration)

@@ TODO: should these be supported?

### [8.3 Component extraction functions on durations](https://www.w3.org/TR/xpath-functions/#component-extraction-durations)

@@ TODO: should these be supported?

### [8.4 Arithmetic operators on durations](https://www.w3.org/TR/xpath-functions/#duration-arithmetic)

@@ TODO: should these be supported?

## [9 Functions and operators on dates and times](https://www.w3.org/TR/xpath-functions/#dates-times)

### [9.4 Comparison operators on duration, date and time values](https://www.w3.org/TR/xpath-functions/#comp.datetime)

@@ TODO: Should `gYear`, `gMonth`, and `gDay` be supported?

- [ ] `op:date-equal`
- [ ] `op:date-less-than`
- [ ] `op:date-greater-than`
- [ ] `op:time-equal`
- [ ] `op:time-less-than`
- [ ] `op:time-greater-than`
- [ ] `op:gYearMonth-equal`
- [ ] `op:gYear-equal`
- [ ] `op:gMonthDay-equal`
- [ ] `op:gMonth-equal`
- [ ] `op:gDay-equal`

### [9.5 Component extraction functions on dates and times](https://www.w3.org/TR/xpath-functions/#component-extraction-dateTime)

- [x]	`fn:year-from-date`
- [x]	`fn:month-from-date`
- [x]	`fn:day-from-date`
- [ ]	`fn:timezone-from-date`
- [x]	`fn:hours-from-time`
- [x]	`fn:minutes-from-time`
- [x]	`fn:seconds-from-time`
- [ ]	`fn:timezone-from-time`

### [9.6 Timezone adjustment functions on dates and time values](https://www.w3.org/TR/xpath-functions/#timezone.functions)

- [ ] `fn:adjust-dateTime-to-timezone`
- [ ] `fn:adjust-date-to-timezone`
- [ ] `fn:adjust-time-to-timezone`

### [9.7 Arithmetic operators on durations, dates and times](https://www.w3.org/TR/xpath-functions/#dateTime-arithmetic)

- [x] op:subtract-dateTimes,
- [x] op:subtract-dates,
- [x] op:subtract-times
- [x] op:add-yearMonthDuration-to-dateTime,
- [x] op:add-yearMonthDuration-to-date
- [x] op:add-dayTimeDuration-to-dateTime,
- [x] op:add-dayTimeDuration-to-date,
- [x] op:add-dayTimeDuration-to-time
- [x] op:subtract-yearMonthDuration-from-dateTime,
- [x] op:subtract-yearMonthDuration-from-date
- [x] op:subtract-dayTimeDuration-from-dateTime,
- [x] op:subtract-dayTimeDuration-from-date,
- [x] op:subtract-dayTimeDuration-from-time

### [9.8 Formatting dates and times](https://www.w3.org/TR/xpath-functions/#formatting-dates-and-times)

- [ ] `fn:format-dateTime`
- [ ] `fn:format-date`
- [ ] `fn:format-time`

### [9.9 Parsing dates and times](https://www.w3.org/TR/xpath-functions/#parsing-dates-and-times)

@@ TODO: Should the XSD parsing algorithm be supported, or is casting using SPARQL's [XPath Constructor Function](https://www.w3.org/TR/sparql11-query/#FunctionMapping) style sufficient?

- [x]	`xsd:date`
- [x]	`xsd:time`
- [x]	`xsd:duration`

## TODO

* Support for timezones in xsd:date
* Support for timezones in xsd:time
* Correct construction of xsd:dateTime `1999-12-31T24:00:00`
