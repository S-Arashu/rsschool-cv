# Anastasiya Tomasheva

![my photo](https://scontent-waw1-1.cdninstagram.com/v/t51.2885-15/26224528_186196198797718_7535920042416799744_n.jpg?stp=dst-jpg_e35&_nc_ht=scontent-waw1-1.cdninstagram.com&_nc_cat=110&_nc_ohc=KdlEjeNU1bgAX9rGp0m&edm=ABmJApABAAAA&ccb=7-5&ig_cache_key=MTcwNDU5MjIxMTU4ODI0OTMzNA%3D%3D.2-ccb7-5&oh=00_AfD48ikLBurrpw-b8zhSOVh6IpLWndE7dzZ25MYOvRCZLA&oe=6427D2A5&_nc_sid=6136e7)

### Contacts

##### Phone number, Skype, Telegram, Viber, WhatsApp: +375(44)7-202-103
##### E-mail: Siha.sole@gmail.com
##### [LinkedIn](https://www.linkedin.com/in/s-arashu/)

* Social:

     + [TikTok](https://www.tiktok.com/@happyreading03?_t=8b1AlakRHIT&_r=1)
     + [TikTok](https://www.tiktok.com/@_arashu_?_t=8b1Ak8mhrKo&_r=1)
     + [VK](https://vk.com/arashu)
     + [Instagram](https://instagram.com/_s_i_h_a_?igshid=YmMyMTA2M2Y=)

***
## About me

For me everything about programming has always seemed like magic. But one day, about ten years ago, a friend offered me to try testing (she already worked in this specialty at EPAM and offered to try me). I wasn’t hired, but in preparation for my interview, I got to know a little bit of HTML, and that’s when that little piece of magic became a reality. When I thought about changing jobs in the future, it was this episode that came to mind, and the decision was made. 

Now I am far from a professional, but I can do much more than at the beginning of last year (although, I will not hide, there are bouts of desperation =) ). Based on the above, we can conclude that my work experience it`s learning. To understand how inspired I am by it, I can give you an example of my training. Now, in addition to RS, I am completing paid Frontend courses. Since October last year I have studied, I have two jobs, in my spare time I only sleep, eat and sometimes go for walks) All this time nerves could fail only about the lack of understanding of any intricacies of learning, and never - because of lack of free time. Of course, I do not plan to always exclude for myself the rest, but also realized that and to learn I will never stop =)

***

## Skills and Proficiency

* HTML, CSS
* JavaScript
* Git, GitHub
* VS Code
* Adobe Photoshop, Figma
* React
* Bootstrap
    
***
## Code example

### Task from Codewars

> You probably know the "like" system from Facebook and other pages. People can "like" blog posts, pictures or other items. We want to create the text that should be displayed next to such an item. Implement the function which takes an array containing the names of people that like an item. It must return the display text as shown in the examples:

```
[]                                -->  "no one likes this"
["Peter"]                         -->  "Peter likes this"
["Jacob", "Alex"]                 -->  "Jacob and Alex like this"
["Max", "John", "Mark"]           -->  "Max, John and Mark like this"
["Alex", "Jacob", "Mark", "Max"]  -->  "Alex, Jacob and 2 others like this"
```

> Note: For 4 or more names, the number in "and 2 others" simply increases.

### Solution

```
function likes(names) {
  if(names.length === 0){
    return 'no one likes this'
  }
  else if(names.length ===1){
    return `${names[0]} likes this`
  }
  else if(names.length ===2){
    return `${names[0]} and ${names[1]} like this`
  }
  else if(names.length ===3){
    return `${names[0]}, ${names[1]} and ${names[2]} like this`
  }
  else if(names.length > 3){
    return `${names[0]}, ${names[1]} and ${names.length-2} others like this`
  }
}

```

***

## Study projects

* [Site](https://github.com/S-Arashu/The-Dark-Pictures)
* [Store](https://github.com/S-Arashu/Store-or-something-like-)
