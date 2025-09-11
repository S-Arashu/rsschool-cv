# **Anastasiya Tomasheva**

---

## _Contacts_

**Phone:** +375447202103\
**Email:** siha.sole@gmail.com\
**Telegram:** @arashu*siha\
**Skype:** siha.sole\
[LinkedIn](https://www.linkedin.com/feed/)\
[GitHub](https://github.com/S-Arashu)\
[Instagram](https://www.instagram.com/_s_i_h_a*/)\
[TikTok](https://www.tiktok.com/@happyreading03)\
[TikTok](https://www.tiktok.com/@_arashu_?is_from_webapp=1&sender_device=pc)

---

## _About me_

Hello! Nice to meet you 😊 I\`m Anastasia, person who sometimes enormous creative and active, and sometimes just a snail, that don\`t want left my warm plaid 😊 I like either being it noisy company, sitting with good book near window, painting, embroidering, watching films or doing activities or sport 😊 I have a lot of beliefs, and one of them - not much things can be as beautiful as nature. That\`s why my socials full of photos of nature, but not me 😊 I really like share this beauty, so i discovering a lot of places and doing a lot of photos. But I have a flaw as well - i hard to me to stop. I covering tens of kilometers, and hardly imagine how to back home because of that 😊 That\`s why people scaring to cycling with me 😊 The same is about work - if I have a task, it\`s capture entire me, and others sent me to rest by the force 😊 I have been dreaming about work, that bring people absolute benefit, and awareness that I do exactly this kind of job giving me even more energy and inspiration. Financial side always make me a shy, but I realizing that it\`s very important. Because if a person don`t have enough money for qualitative food or relaxing - that, of course, involve on either quality of life and quality of work. All interconnected, finding ballance - is not easy work, but when we will find it, we will have ideal formula of productivity 😊

---

## _Skills_

- HTML, CSS
- JavaScript
- Git, GitHub
- VS Code
- Adobe Photoshop
- Figma
- React (beginner)
- PHP (beginner)

---

## _Code examples_

### **Task**

```
The purpose of this kata is to implement the undoRedo function.

This function takes an object and returns an object that has these actions to be performed on the object passed as a parameter:

set(key, value) Assigns the value to the key. If the key does not exist, creates it.

get(key) Returns the value associated to the key.

del(key) removes the key from the object.

undo() Undo the last operation (set or del) on the object. Throws an exception if there is no operation to undo.

redo() Redo the last undo operation (redo is only possible after an undo). Throws an exception if there is no operation to redo.

After set() or del() are called, there is nothing to redo.

All actions must affect to the object passed to undoRedo(object) function. So you can not work with a copy of the object.

Any set/del after an undo should disallow new redos.
```

### **Solution**

```
function undoRedo(obj) {
  const history = [];
  const undone = [];

  return {
    set: (key, value) => {
      history.push({ type: 'set', key, oldValue: obj[key], newValue: value });
      undone.length = 0;
      obj[key] = value;
    },
    get: (key) => obj[key],
    del: (key) => {
      history.push({ type: 'del', key, oldValue: obj[key] });
      undone.length = 0;
      delete obj[key];
    },
    undo: () => {
      if (history.length === 0) throw new Error('No operation to undo');
      const lastOperation = history.pop();
      undone.push(lastOperation);
      if (lastOperation.type === 'set') {
        obj[lastOperation.key] = lastOperation.oldValue;
        if (lastOperation.oldValue === undefined) delete obj[lastOperation.key];
      } else if (lastOperation.type === 'del') {
        obj[lastOperation.key] = lastOperation.oldValue;
      }
    },
    redo: () => {
      if (undone.length === 0) throw new Error('No operation to redo');
      const lastUndone = undone.pop();
      history.push(lastUndone);
      if (lastUndone.type === 'set') {
        obj[lastUndone.key] = lastUndone.newValue;
      } else if (lastUndone.type === 'del') {
        delete obj[lastUndone.key];
      }
    }
  };
}
```

---

## _My works_

[Store-or-something-like-](https://github.com/S-Arashu/Store-or-something-like-) (HTML, CSS, JavaScript)\
[The-Dark-Pictures](https://github.com/S-Arashu/The-Dark-Pictures) (HTML, CSS)\
[Exam_1](https://github.com/S-Arashu/Exam_1) (HTML, CSS)\
[Final-Project-For-ITSchool](https://github.com/S-Arashu/Final-Project-For-ITSchool) (HTML, CSS, JavaScript, React)\
[Quotes](https://github.com/stars/S-Arashu/lists/%D1%86%D0%B8%D1%82%D0%B0%D1%82%D1%8B) (CSS - will be supplemented)

---

## _Education_

- **Mogilev State A. Kuleshov University**
  - Faculty of Slavic Philology, print media journalist
- **MyItSchool**
  - Frontend developer
- **RSSchool**
  - In process

---

## _English level_

Intermediate(B1)
