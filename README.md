# sumDays
> 📆 Function to add days from a date

## Arguments
The first argument is the date, the second is the number of days
```javascript
sumDays('09/25/2017',5);
// Sat Sep 30 2017 00:00:00 GMT-0300 (-03)
```
```javascript
sumDays(new Date(),2);
// Wed Sep 27 2017 10:29:33 GMT-0300 (-03)
```
## Code
```javascript
const sumDays = (currentDate, days) => {
  currentDate = new Date(currentDate);
  const dayTimeStamp = 86400000;
  const daycurrentTimeStamp = currentDate.getTime();
  return new Date(daycurrentTimeStamp+(dayTimeStamp*days))
};
 ```
