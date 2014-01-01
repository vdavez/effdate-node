effdate-node
============

An effective date counter written in node.js

## What's this about?
Under [section 602(c) of the Home Rule Act](http://dccode.org/browser/#/1/1-206.02), most Council acts** must be transmitted to Congress for 30-day passive review. In 40 years of Home Rule, there have only been 3 instances where Congress has exercised its power under section 602(c) to disapprove of Council acts.

Making matters worse, Congress decided that 30 days would be too easy to calculate, so Congress defined the 30-day period as follows:  

> the 30-calendar-day period (excluding Saturdays, Sundays, and holidays, and any day on which neither House is in session because of an adjournment sine die, a recess of more than 3 days, or an adjournment of more than 3 days) beginning on the day such act is transmitted by the Chairman to the Speaker of the House of Representatives and the President of the Senate

Until now, calculating the 30-day period required reference to several calendars and hand counts. This counter actually computes the proper date with one caveat: it is only accurate retrospectively... 

That's because we can't actually know when Congress will be in recess (or not) before they go in recess (or don't). So,to write a program to let the public know when a bill actually would become a law would require a change in the Home Rule Act.

** The main exceptions are (1) acts affecting the criminal code, which have 60-day periods, and (2) Charter amendments, which have a 35-day count (though the counting method is slightly different).

## Usage
To run the counter, you need to do two steps:

The first time around:

    npm install

After that:

    node effdate.js

## Example

    > node effdate.js
	prompt: transmittal date, please?:  2013-01-16
	Effective Date: Friday, Mar. 01, 2013
	'Count: 2013/01/16,2013/01/17,2013/01/18,2013/01/22,2013/01/23,2013/01/24,2013/01/25,2013/01/28,2013/01/29,2013/01/30,2013/01/31,2013/02/01,2013/02/04,2013/02/05,2013/02/06,2013/02/07,2013/02/08,2013/02/11,2013/02/12,2013/02/13,2013/02/14,2013/02/15,2013/02/19,2013/02/20,2013/02/21,2013/02/22,2013/02/25,2013/02/26,2013/02/27,2013/02/28'

## License
This is public domain.