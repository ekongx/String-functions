#### String.fromCharCode()
String对象提供的静态方法（即定义在对象本身，而不是定义在对象实例的方法），主要是fromCharCode()。该方法的参数是一系列Unicode码点，返回对应的字符串。

#### charAt()
charAt方法返回指定位置的字符，参数是从0开始编号的位置。
```
var s = new String('abc');
s.charAt(1) // "b"
s.charAt(s.length - 1) // "c"
```

#### charCodeAt()
charCodeAt方法返回给定位置字符的Unicode码点（十进制表示），相当于String.fromCharCode()的逆操作。
```
'abc'.charCodeAt(1) // 98
```

#### concat()
concat方法用于连接两个字符串，返回一个新字符串，不改变原字符串。

```
var s1 = 'abc';
var s2 = 'def';

s1.concat(s2) // "abcdef"
s1 // "abc"
```

#### slice()
slice方法用于从原字符串取出子字符串并返回，不改变原字符串。
```
'JavaScript'.slice(0, 4) // "Java"
```

#### indexOf()，lastIndexOf()
这两个方法用于确定一个字符串在另一个字符串中的位置，都返回一个整数，表示匹配开始的位置。如果返回-1，就表示不匹配。两者的区别在于，indexOf从字符串头部开始匹配，lastIndexOf从尾部开始匹配。

```javascript
'hello world'.indexOf('o') // 4
'JavaScript'.indexOf('script') // -1

'hello world'.lastIndexOf('o') // 7
```

#### trim()
trim方法用于去除字符串两端的空格，返回一个新字符串，不改变原字符串。

#### toLowerCase()，toUpperCase()
toLowerCase方法用于将一个字符串全部转为小写，toUpperCase则是全部转为大写。

#### localeCompare()
localeCompare方法用于比较两个字符串。它返回一个整数，如果小于0，表示第一个字符串小于第二个字符串；如果等于0，表示两者相等；如果大于0，表示第一个字符串大于第二个字符串。

#### match()
match方法用于确定原字符串是否匹配某个子字符串，返回一个数组，成员为匹配的第一个字符串。如果没有找到匹配，则返回null。

```
'cat, bat, sat, fat'.match('at') // ["at"]
'cat, bat, sat, fat'.match('xt') // null
```

#### search()
search方法的用法等同于match，但是返回值为匹配的第一个位置。如果没有找到匹配，则返回-1。

#### replace()
replace方法用于替换匹配的子字符串，一般情况下只替换第一个匹配（除非使用带有g修饰符的正则表达式）。

```
'aaa'.replace('a', 'b') // "baa"
```

#### split()
split方法按照给定规则分割字符串，返回一个由分割出来的子字符串组成的数组。

```
'a|b|c'.split('|') // ["a", "b", "c"]
```

