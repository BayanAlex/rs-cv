# Oleksandr Shyhyda

## Contact Info
>- **Address:** Mykolaiv, Ukraine
>- **E-mail:** bayanalex@gmail.com
>- **LinkedIn:** [OleksandrShyhyda](https://www.linkedin.com/in/oleksandr-shyhyda-1150aa139)
>- **Telegram:** [@CyberAlex](https://t.me/CyberAlex)

---

## Summary

---

## Code example
**codewars kata:** [Binomial Expansion](https://www.codewars.com/kata/540d0fdd3b6532e5c3000b5b)
```javascript
function expand(expr) {
    const a = +(expr.match(/(?<=\()-?\d*/).toString().replace(/-(?!\d)/, '-1') || '1');
    const b = +expr.match(/-?\d+(?=\))/).toString();
    const x = expr.match(/\w(?=[-+])/).toString();
    const n = +expr.match(/(?<=\^)\d+/).toString();
    let result = [];
    for(let k = n; k >= 0; k--) {
        let c = '' + (fact(n) / (fact(k) * fact(n - k))) * a**k * b**(n - k);
        if(c == '0')
            continue;  
        if(k != 0) {
            if(c == '1')
                c = '';
            else if (c == '-1')
                c = '-';
            c += k == 1 ? x : `${x}^${k}`;
        }
        result.push(c);
    }
    return result.join('+').replace(/\+-/g, '-');
  
    function fact(n) {
        if(n == 0)
            return 1;
        return n * fact(n - 1);
    }
}
```

---

## Education

---

## Skills

---

## Experience

---

## Courses

---

## Languages
>- **Ukrainian** Native
>- **Russian** Fluent
>- **_English_** Upper Intermediate