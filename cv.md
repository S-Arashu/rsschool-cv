# **Anastasiya Tomasheva**
***
## _Contacts_
\
**Phone:** +375447202103\
**Email:** siha.sole@gmail.com\
**Telegram:** @arashu_siha\
**Skype:** siha.sole\
[LinkedIn](https://www.linkedin.com/feed/)\
[GitHub](https://github.com/S-Arashu)\
[Instagram](https://www.instagram.com/_s_i_h_a_/)\
[TikTok](https://www.tiktok.com/@happyreading03)\
[TikTok](https://www.tiktok.com/@_arashu_?is_from_webapp=1&sender_device=pc)

***

## _About me_
\
I started studying the Front about two years ago, but, unfortunately, with interruptions, since the priorities were different and I had to interrupt often. I completed the FrontEnd Developer course and received a certificate, but I still don’t have enough experience. Now it is only related to testing mailings - better than nothing, but I would like more. This area interests me very much, and I do not plan to stop only at the Front; after completing the course I will continue my studies and expand my area of ​​knowledge. In my opinion, it’s incredibly interesting to create something new and visually designed from a set of symbols. It’s like writing a book, but in code language. ✨Magically✨ 😊

***

## _Skills_

   * HTML, CSS
   * JavaScript
   * Git, GitHub
   * VS Code
   * Adobe Photoshop
   * Figma
   * React (beginner)
   * PHP (beginner)

***

## _Code examples_
   * ### **Task**
```
Your task in order to complete this Kata is to write a function which formats a duration, given as a number of seconds, in a human-friendly way.

The function must accept a non-negative integer. If it is zero, it just returns "now". Otherwise, the duration is expressed as a combination of years, days, hours, minutes and seconds.

It is much easier to understand with an example:

* For seconds = 62, your function should return 
    "1 minute and 2 seconds"
* For seconds = 3662, your function should return
    "1 hour, 1 minute and 2 seconds"
For the purpose of this Kata, a year is 365 days and a day is 24 hours.

Note that spaces are important.

Detailed rules
The resulting expression is made of components like 4 seconds, 1 year, etc. In general, a positive integer and one of the valid units of time, separated by a space. The unit of time is used in plural if the integer is greater than 1.

The components are separated by a comma and a space (", "). Except the last component, which is separated by " and ", just like it would be written in English.

A more significant units of time will occur before than a least significant one. Therefore, 1 second and 1 year is not correct, but 1 year and 1 second is.

Different components have different unit of times. So there is not repeated units like in 5 seconds and 1 second.

A component will not appear at all if its value happens to be zero. Hence, 1 minute and 0 seconds is not valid, but it should be just 1 minute.

A unit of time must be used "as much as possible". It means that the function should not return 61 seconds, but 1 minute and 1 second instead. Formally, the duration specified by of a component must not be greater than any valid more significant unit of time.
```
   * ### **Solution**
```
const { assert } = require('chai');

describe("Tests", () => {
  
  function dotest(input, expected) {
    assert.strictEqual(formatDuration(input), expected, `Incorrect answer for seconds=${input}`);
  }
  
  it("Fixed tests", () => {
    dotest(0, "now");
    
    dotest(1, "1 second");
    dotest(62, "1 minute and 2 seconds");
    dotest(120, "2 minutes");
    dotest(3600, "1 hour");
    dotest(3662, "1 hour, 1 minute and 2 seconds");

    dotest(15731080, "182 days, 1 hour, 44 minutes and 40 seconds");
    dotest(132030240, "4 years, 68 days, 3 hours and 4 minutes");
    dotest(205851834, "6 years, 192 days, 13 hours, 3 minutes and 54 seconds");
    dotest(253374061, "8 years, 12 days, 13 hours, 41 minutes and 1 second");
    dotest(242062374, "7 years, 246 days, 15 hours, 32 minutes and 54 seconds");
    dotest(101956166, "3 years, 85 days, 1 hour, 9 minutes and 26 seconds");
    dotest(33243586, "1 year, 19 days, 18 hours, 19 minutes and 46 seconds");
  });


  it("random tests", () => {
    
    function sol(seconds) {
      if (seconds == 0) return 'now';
      function formatComponents(x) {
        let firsts = x.slice(0, -1).join(', ');
        return (firsts && firsts + ' and ') + x[x.length - 1];
      }

      let components = ["year", "day", "hour", "minute", "second"];
      let times = [31536000, 86400, 3600, 60, 1];

      return formatComponents(
        times.map((secondsByUnit, i) => {
          let value = (seconds / secondsByUnit) | 0;
          seconds %= secondsByUnit;
          return value == 0 ? '' : value + ' ' + components[i] + (value > 1 ? 's' : '');
        }).filter(Boolean));
    }
    
    for (let i = 0; i < 100; i++) {
      const n = Math.floor(Math.random() * 10000000);
      dotest(n, sol(n));
    }
  });
});
```

***

## _My works_
\
[Store-or-something-like-](https://github.com/S-Arashu/Store-or-something-like-) (HTML, CSS, JavaScript)\
[The-Dark-Pictures](https://github.com/S-Arashu/The-Dark-Pictures) (HTML, CSS)\
[Exam_1](https://github.com/S-Arashu/Exam_1) (HTML, CSS)\
[Final-Project-For-ITSchool](https://github.com/S-Arashu/Final-Project-For-ITSchool) (HTML, CSS, JavaScript, React)\
[Quotes](https://github.com/stars/S-Arashu/lists/%D1%86%D0%B8%D1%82%D0%B0%D1%82%D1%8B) (CSS - will be supplemented)

***

## _Education_
* **Mogilev State A. Kuleshov University**
  * Faculty of Slavic Philology, print media journalist
* **MyItSchool**
  * Frontend developer
* **Stepik**
  * In process

***

## _English level_
\
I only have a little practice when talking to friends.