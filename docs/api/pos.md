# Position updates

Position updates are sent every 5 seconds.



## Pilots ##

Aircraft updates (both outgoing and incoming) are prefixed with `@S` or `@N`. The distinction between the two is unclear:

```
@S:(callsign):(squawk):(rating):(lat):(lon):(alt):(groundspeed):(num1):(num2) 
```

```
@N:(callsign):(squawk):(rating):(lat):(lon):(alt):(groundspeed):(num1):(num2) 
```

The meaning of the following fields is unclear:

* `(num1)` is a 10-digit number.  It seems to begin with 4.
* `(num2)` is an integer. There seems to be a wide range of values, anywhere between 1 and 3 digits, and can be positive or negative.



## ATC ##

ATC updates are prefixed with `%`:

```
%(callsign):(freq):(altitude):100:1:(lat):(lon)
```

ATC stations and observers also have a location and altitude associated with them.